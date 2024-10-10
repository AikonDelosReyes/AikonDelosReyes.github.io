<script>
    import { faFacebook, faGithub, faDiscord, faGoogle } from '@fortawesome/free-brands-svg-icons';
    import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
  
    let pageTitle = "Contact Me";
    let description = "The Best way to contact me is on gmail delosreyesaikon@gmail.com but Feel free to connect with me on any of the following platforms:";
</script>
  
<section class="flex flex-col items-center justify-center min-h-[40vh] bg-gray-100 text-gray-900">
    <div class="">
        <!-- Page Title -->
        <h1 class="text-5xl font-bold mb-4 text-green-950">
            {pageTitle}
        </h1>
        
        <!-- Description -->
        <p class="text-lg mb-6 leading-relaxed">
            {description}
        </p>
  
        <!-- Social Links -->
        <div class="flex gap-6 justify-center"> <!-- Horizontal layout for icons -->
            <!-- GitHub -->
            <a href="https://github.com/AikonDelosReyes" class="text-green-950 hover:text-gray-500">
                <FontAwesomeIcon icon={faGithub} class="w-10 h-10" />
            </a>
  
            <!-- Facebook -->
            <a href="https://facebook.com/Aikon Delos Reyes" class="text-green-950 hover:text-blue-600">
                <FontAwesomeIcon icon={faFacebook} class="w-10 h-10" />
            </a>

            <!-- Discord -->
            <a href="https://discord.com/users/konix17" class="text-green-950 hover:text-indigo-600">
                <FontAwesomeIcon icon={faDiscord} class="w-10 h-10" />
            </a>

            
        </div>
    </div>
</section>
  
