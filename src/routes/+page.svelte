<script>
    let pageTitle = "Hey there! 👋 Welcome to my portfolio. Take a look around and check out what I've been working on!";
    let description = "Feel free to explore my projects, skills, and everything else I love doing. 😊";
</script>

<section class="flex flex-col items-center justify-center min-h-[60vh] bg-gray-100 text-gray-900">
    <div class="">
        <!-- Page Title -->
        <h1 class="text-5xl font-bold mb-4 text-green-950">
            {pageTitle}
        </h1>
        
        <!-- Description -->
        <p class="text-lg mb-6 leading-relaxed">
            {description}
        </p>

        <!-- Image -->
        <div class="flex justify-center mb-6">
            <div class="rounded-full overflow-hidden w-32 h-32 border-4 border-green-950 shadow-md">
                <img src="/images/Profile.jpg" alt="Aikon Delos Reyes" class="object-cover w-full h-full">
            </div>
        </div>

        
    </div>
</section>
