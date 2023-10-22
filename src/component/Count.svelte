<!-- Counts.svelte -->

<script>
    import { onMount } from 'svelte';
  
    let counters = [
      { label: 'Clients', start: 0, end: 14 },
      { label: 'Projects', start: 0, end: 5000 },
      { label: 'Hours Of Support', start: 0, end: 100000 },
      { label: 'Hard Workers', start: 0, end: 35 },
    ];
  
    function startCounters() {
      counters.forEach((counter, index) => {
        const duration = 500;
        const step = (counter.end - counter.start) / duration;
  
        let currentValue = counter.start;
        let updateInterval;
  
        updateInterval = setInterval(() => {
          if (currentValue < counter.end) {
            currentValue += step;
          } else {
            currentValue = counter.end;
            clearInterval(updateInterval);
          }
  
          // Update the counter values
          counters[index] = { ...counter, currentValue };
        }, 1);
      });
    }
  
    // Start the counters when the component is mounted
    onMount(() => {
      startCounters();
    });
  </script>
  
  <main class="style-73">
    <div class="style-74">
      <div class="style-75">
        {#each counters as counter (counter.label)}
          <div class="style-76">
            <span data-purecounter-start={counter.start} data-purecounter-end={counter.end} class="style-77">
              {Math.round(counter.currentValue)}
            </span>
            <p class="style-78">{counter.label}</p>
          </div>
        {/each}
      </div>
    </div>
  </main>
  