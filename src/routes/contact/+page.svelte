<script>
    import { GithubSolid, FacebookSolid, DiscordSolid } from 'flowbite-svelte-icons';

    let pageTitle = "Contact Me";
    let description = "The best way to contact me is via email at delosreyesaikon@gmail.com, but feel free to connect with me on any of the following platforms:";
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
                <GithubSolid class="w-10 h-10" />
            </a>
  
            <!-- Facebook -->
            <a href="https://facebook.com/AikonDelosReyes" class="text-green-950 hover:text-blue-600">
                <FacebookSolid class="w-10 h-10" />
            </a>

            <!-- Discord -->
            <a href="https://discord.com/users/konix17" class="text-green-950 hover:text-indigo-600">
                <DiscordSolid class="w-10 h-10" />
            </a>
        </div>
    </div>
</section>
