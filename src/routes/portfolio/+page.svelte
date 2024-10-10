<script>
    import { FontAwesomeIcon } from '@fortawesome/svelte-fontawesome';
    import { faCamera, faGamepad, faGuitar, faBook } from '@fortawesome/free-solid-svg-icons';

    let pageTitle = "My Portfolio";
    let description = "Explore my professional work and personal hobbies. Here are some of my projects and what I enjoy doing in my free time.";

    // gallery images
    const images = [
        { title: 'Cactus', description: 'A Custom plant Designed using Photoshop.', src: '/images/cactus.png', pdf: '/pdf/1.pdf' },
        { title: 'Character 6 sides', description: 'Custom Character using Photoshop.', src: '/images/character.png', pdf: '/pdf/2.pdf' },
        { title: 'Getter&Setter', description: 'Getter&Setter using Netbeans.', src: '/images/getter&setter.png', pdf: '/pdf/3.pdf' },
        { title: 'Class Dog Constructor', description: 'A Class Dog Constructor using Netbeans.', src: '/images/constructor.png', pdf: '/pdf/4.pdf' },
        { title: 'Class Dog AnimalTester', description: 'A Class Dog AnimalTester using Netbeans.', src: '/images/animaltester.png', pdf: '/pdf/5.pdf' },
        { title: 'Simple Calculator', description: 'Python Simple Gui Calculator.', src: '/images/calculator.png', pdf: '/pdf/6.pdf' },
        { title: 'Asyncio', description: 'Asyncio using vscode.', src: '/images/async.png', pdf: '/pdf/7.pdf' },
        { title: 'Week 2 Activity', description: 'My week 2 lab activity for business analytics.', src: '/images/week2.png', pdf: '/pdf/8.pdf' },
        { title: 'Lecture Harvest', description: 'My Project mock up for Object Oriented Programming.', src: '/images/lectureharvest.png', pdf: '/pdf/9.pdf' },
        
    ];
</script>

<section class="min-h-screen flex flex-col items-center justify-center bg-gray-200 text-gray-900">
    <div class="max-w-4xl w-full p-6 text-center">
        <!-- Page Title -->
        <h1 class="text-5xl font-bold mb-8 text-green-950">
            {pageTitle}
        </h1>
        
        <!-- Description -->
        <p class="text-lg mb-12 leading-relaxed">
            {description}
        </p>

        <!-- Assignments Section -->
        <div class="mb-16">
            <h2 class="text-3xl font-semibold mb-6 text-green-950">Assignments</h2>
            <div class="grid gap-3 grid-cols-2 md:grid-cols-3"> <!-- Adjusted gap here -->
                {#each images as image}
                    <a href={image.pdf} target="_blank" rel="noopener noreferrer" class="relative group m-2"> <!-- Added margin for spacing -->
                        <img src={image.src} alt={image.title} class="rounded-lg shadow-md object-cover h-full w-full transform transition-transform duration-300 ease-in-out group-hover:scale-105" />
                        <!-- Image title and description on hover -->
                        <div class="absolute inset-0 flex flex-col justify-center items-center bg-black text-white opacity-0 transition-opacity duration-300 ease-in-out group-hover:opacity-80">
                            <h3 class="text-lg font-bold mb-2">{image.title}</h3>
                            <p class="text-sm text-center">{image.description}</p>
                        </div>
                    </a>
                {/each}
            </div>
        </div>
</section>

<style>
    /* Ensures the hover effect scales and shows text */
    .group-hover\:scale-105 {
        transform: scale(1.05);
    }

    /* Makes images fixed and fitted within their containers */
    img {
        object-fit: cover; 
        width: 100%;
        height: 100%;
    }
</style>

