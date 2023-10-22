<script>
      function scrollToSection(targetId) {
    const targetElement = document.querySelector(targetId);
    if (targetElement) {
      targetElement.scrollIntoView({ behavior: 'smooth' });
    }
  }
</script>

<header class="style-1">
    <div class="style-2">
        <h1 class="style-3"><a href="index.html" class="style-4">MPS</a></h1>
        <!-- Uncomment below if you prefer to use an image logo -->
        <!-- <img src="assets/img/logo.png" alt="" class="img-fluid" /> -->

        <nav class="style-5">
            <ul class="style-6">
                <li class="style-7"><a class="style-8" href="#hero" on:click={() => scrollToSection("hero")}>Home</a></li>
                <li class="style-9"><a class="style-10" href="#about" on:click={() => scrollToSection("about")}>About</a></li>
                <li class="style-11"><a class="style-12" href="#services" on:click={() => scrollToSection("services")}>Services</a></li>
                <li class="style-13"><a class="style-14" href="#portfolio" on:click={() => scrollToSection("portfolio")}>Portfolio</a></li>
                <li class="style-15"><a class="style-16" href="#team" on:click={() => scrollToSection("team")}>Team</a></li>
                <li class="style-17"><a class="style-18" href="#contact" on:click={() => scrollToSection("contact")}>Contact</a></li>
                <li class="style-19"><a class="style-20" href="#about" on:click={() => scrollToSection("about")}>Get Started</a></li>
              </ul>              
            <i class="style-21"></i>
        </nav><!-- .navbar -->
    </div>
</header><!-- End Header -->
