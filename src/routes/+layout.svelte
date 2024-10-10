<script lang="ts">
    import "../app.css";
    import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
    import { faHome, faUser, faEnvelope, faBriefcase } from '@fortawesome/free-solid-svg-icons'; // Import the necessary icons
</script>

<svelte:head>
  <!-- Google Fonts and Title -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin="anonymous">
  <link href="https://fonts.googleapis.com/css2?family=Kanit:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900&display=swap" rel="stylesheet">
  <title>My SvelteKit App</title>
</svelte:head>

<!-- Main container with background image -->
<div class="min-h-screen bg-cover bg-center flex flex-col items-center justify-between"
     style="background-image: url('/images/Bears.png');">
  
  <!-- Header with specified color and shadow -->
  <header class="w-full py-6" style="background-color: #FDF6B2; color: #8E4B10;">
    <div class="container mx-auto px-4 text-center">
      <h1 class="text-4xl font-extrabold">Aikon Delos Reyes</h1>
      <nav class="mt-4 flex justify-center space-x-4"> <!-- Added flex and space-x-4 for horizontal layout -->
        <a href="/" class="text-lg hover:text-gray-200 flex items-center">
          <FontAwesomeIcon icon={faHome} class="mr-2" /> Home
        </a>
        <a href="/about" class="text-lg hover:text-gray-200 flex items-center">
          <FontAwesomeIcon icon={faUser} class="mr-2" /> About
        </a>
        <a href="/contact" class="text-lg hover:text-gray-200 flex items-center">
          <FontAwesomeIcon icon={faEnvelope} class="mr-2" /> Contact
        </a>
        <a href="/portfolio" class="text-lg hover:text-gray-200 flex items-center">
          <FontAwesomeIcon icon={faBriefcase} class="mr-2" /> Portfolio
        </a>
      </nav>
    </div>
  </header>

  <!-- Main content with card-like structure -->
  <main class="flex-grow flex items-center justify-center py-8 w-auto">
    <div class="bg-white rounded-lg shadow-lg p-8 max-w-4xl w-auto mx-4 text-center">
      <slot></slot>
    </div>
  </main>

  <!-- Footer with specified color -->
  <footer class="w-full py-6" style="background-color: #5b3a29; color: #f5f5dc;">
    <div class="container mx-auto px-4 text-center">
      <p class="text-sm">© 2024 Aikon Delos Reyes - All rights reserved.</p>
      <nav class="mt-2">
       
      </nav>
    </div>
  </footer>
</div>
