<template>
    <nav class="bg-transparent p-4 ">
        <ul class="flex space-x-20 justify-center">
            <li><a href="#about" class="text-lg font-semibold text-white hover:text-gray-300">About Me</a></li>
            <li><a href="#skills" class="text-lg font-semibold text-white hover:text-gray-300">Skills</a></li>
            <li><a href="#projects" class="text-lg font-semibold text-white hover:text-gray-300">Projects</a></li>
        </ul>
    </nav>
    <section class="h-150 rounded-b-3xl bg-[#0F1735] ">
        <div class="flex justify-center items-center">
            <div>
                <h1 class="text-5xl font-extrabold mb-4 text-white">I'm <span class="text-[#E8F992]">Nicolás Gómez</span></h1>
                <p class="text-2xl font-semibold text-white">A Backend Developer and Software Engineer</p>
            </div>
            <div class=" w-96 h-96 bg-[#e8f992a9] rounded-full blur-3xl"></div>
        </div>
        
        <div class="flex space-x-4 justify-center items-center">
            <button class="mt-8 px-6 py-3 border-2 border-white text-white rounded-full bg-transparent hover:bg-white hover:text-[#0F1735] transition duration-300">
            Contact Me
        </button>
        <button class="mt-8 px-6 py-3 border-2 text-black rounded-full bg-[#E8F992] hover:bg-[#9ca861] hover:text-[#0F1735] transition duration-300">
            View my projects
        </button>
        </div>
    </section>
    <section>
        <div class="mt-8">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">About <span class="text-[#E8F992]">Me</span></h2>
            <p class="text-lg text-white text-center">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer nec odio. Praesent libero. Sed cursus ante dapibus diam. Sed nisi. Nulla quis sem at nibh elementum imperdiet. Duis sagittis ipsum. Pra
            </p>
        </div>
    </section>
    <section class="rounded-b-3xl bg-[#0F1735]">
        <div class="mt-8 text-white">
            <h2 class="text-4xl font-bold mb-2">Experience</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div class="bg-white/10 p-4 rounded-lg border-1 text-white">
                    <h3 class="text-2xl font-semibold">Company D</h3>
                    <p class="text-lg text-white">From: March 2022 - To: Present</p>
                    <p class="text-lg text-white">Role: Lead Developer</p>
                </div>
                <div class="bg-white/10 p-4 rounded-lg border-1 text-white">
                    <h3 class="text-2xl font-semibold">Company A</h3>
                    <p class="text-lg text-white">From: January 2020 - To: December 2021</p>
                    <p class="text-lg text-white">Role: Software Engineer</p>
                </div>
                <div class="bg-white/10 p-4 rounded-lg border-1 text-white">
                    <h3 class="text-2xl font-semibold">Company B</h3>
                    <p class="text-lg text-white">From: February 2018 - To: December 2019</p>
                    <p class="text-lg text-white">Role: Frontend Developer</p>
                </div>
                <div class="bg-white/10 p-4 rounded-lg border-1 text-white">
                    <h3 class="text-2xl font-semibold">Company C</h3>
                    <p class="text-lg text-white">From: June 2016 - To: January 2018</p>
                    <p class="text-lg text-white">Role: Junior Developer</p>
                </div>
            </div>
        </div>
    </section>
    <section>
        <div class="mt-8">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">Projects</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div class="bg-gray-100 p-4 rounded-lg">
                    <img src="" alt="Project 1" class="w-full h-48 object-cover rounded-t-lg">
                    <h3 class="text-2xl font-semibold mt-2">Project 1</h3>
                    <p class="text-lg text-white">Description of project 1.</p>
                </div>
                <div class="bg-gray-100 p-4 rounded-lg">
                    <img src="" alt="Project 2" class="w-full h-48 object-cover rounded-t-lg">
                    <h3 class="text-2xl font-semibold mt-2">Project 2</h3>
                    <p class="text-lg text-white">Description of project 2.</p>
                </div>
                <div class="bg-gray-100 p-4 rounded-lg">
                    <img src="" alt="Project 3" class="w-full h-48 object-cover rounded-t-lg">
                    <h3 class="text-2xl font-semibold mt-2">Project 3</h3>
                    <p class="text-lg text-white">Description of project 3.</p>
                </div>
            </div>
        </div>
    </section>
    <section class="rounded-3xl bg-[#0F1735]">
        <div class="mt-8">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">Nicolás <span class="text-[#E8F992]">Gómez</span></h2>
            <p class="text-lg text-white">Phone: (123) 456-7890</p>
            <p class="text-lg text-white">Email: nicolasgomez@example.com</p>
            <p class="text-lg text-white">Location: City, Country</p>
            <div class="flex space-x-4 mt-4">
                <a href="https://twitter.com/yourprofile" target="_blank" class="text-white hover:text-gray-900">
                    <i class="fab fa-twitter text-2xl">
                        nsdajdnajs
                    </i>
                </a>
                <a href="https://linkedin.com/in/yourprofile" target="_blank" class="text-white hover:text-gray-900">
                    <i class="fab fa-linkedin text-2xl">
                        Linkedin
                    </i>
                </a>
                <a href="https://github.com/yourprofile" target="_blank" class="text-white hover:text-gray-900">
                    <i class="fab fa-github text-2xl">
                        GitHub
                    </i>
                </a>
            </div>
        </div>
    </section>
</template>