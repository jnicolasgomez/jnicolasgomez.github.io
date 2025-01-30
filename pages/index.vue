<template>
    <nav class="p-4 bg-[#0F1735]">
        <ul class="flex space-x-20 justify-center">
            <li @click="scrollToSection('about')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer">About Me</li>
            <li @click="scrollToSection('skills')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer">Skills</li>
            <li @click="scrollToSection('projects')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer">Projects</li>
        </ul>
    </nav>

    <section class="flex h-130 rounded-b-[50px] bg-[#0F1735] overflow-hidden justify-center">
        <div class="flex h-full max-w-6xl relative">
            <div class="m-17 w-full">
                <h1 class="text-8xl font-extrabold mb-4 text-white">I'm <span class="text-[#E8F992]">Nicolás Gómez</span></h1>
                <p class="text-3xl font-semibold text-white">A Backend Developer and Software Engineer</p>
                <div class="text-white text-md max-w-xl">
                    Hi, I'm Nicolas Gomez, a passionate and dedicated software engineer with 5 years of experience specializing in backend development.
                </div>
                <div class="flex space-x-4  items-center">
                    <button @click="scrollToSection('contact')" class="cursor-pointer mt-8 px-6 py-2 border-2 border-white text-white rounded-full bg-transparent hover:bg-white hover:text-[#0F1735] transition duration-300">
                        Contact Me
                    </button>
                    <button @click="scrollToSection('projects')" class="cursor-pointer mt-8 px-6 py-2 border-2 text-black rounded-full bg-[#E8F992] hover:bg-[#9ca861] hover:text-[#0F1735] transition duration-300">
                        View my projects
                    </button>
                </div>
                <div class="flex space-x-4 my-4">
                    <img class="w-4 h-4" src="/assets/star.png" alt="">
                    <img class="w-4 h-4" src="/assets/star.png" alt="">
                    <img class="w-4 h-4" src="/assets/star.png" alt="">
                    <img class="w-4 h-4" src="/assets/star.png" alt="">
                    <img class="w-4 h-4" src="/assets/star.png" alt="">
                </div>
                <div class="text-white text-4xl">
                    5 Years
                </div>
                <div class="text-white text-md">
                    Experience
                </div>
            </div>
            <div class="flex justify-center h-76 bottom-0 right-0 absolute min-w-100">
                <!-- Background Blur Circle -->
                <div class="absolute w-76 h-76 bottom-[-20%] bg-[#e8f99284] rounded-full blur-3xl"></div>

                <!-- Image (Appears Above the Div) -->
                <img class="relative h-76 z-10 min-w-110" src="/picture.png" alt="">
            </div>
            
        </div>
    </section>
    <section id="about">
        <div class="mt-8 p-14">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">About <span class="text-[#E8F992]">Me</span></h2>
            <p class="text-lg text-white text-center">
                I'm a software engineer with five years of experience in building high-quality, impactful software solutions. Passionate about creating efficient and user-friendly products, I continuously explore new technologies and refine my skills to adapt to evolving challenges. My goal is to develop software that enhances everyday life, streamlines processes, and drives meaningful improvements.
            </p>
        </div>
    </section>
    <section class="rounded-[50px] bg-[#0F1735]">
        <div class="mt-8 text-white p-14">
            <h2 class="text-4xl font-bold mb-10">Experience</h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div v-for="item in companies" class="bg-white/10 p-4 rounded-3xl border-1 text-white">
                    <img class="h-14 w-14 mb-4" :src="item.image" alt="">
                    <h3 class="text-2xl mb-4">{{ item.role }}</h3>
                    <p class="text-md text-white mb-4">{{ item.from }} - {{ item.to }}</p>
                </div>
            </div>
        </div>
    </section>
    <section id="skills">
        <div class="mt-8 text-white p-14">
            <h2 class="text-4xl font-bold mb-10 text-center">Programming <span class="text-[#E8F992]">Languages</span></h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div v-for="item in languages" class="bg-white/10 p-4 rounded-3xl border-1 text-white flex">
                    <img class="h-20 w-20" src="/assets/js.png" alt="">
                    <div>
                        <div class="flex">
                        <h3 class="text-2xl font-semibold">{{item.name}}</h3>
                        <img class="w-4 h-4" v-for="i in item.rating" src="/assets/star.png" alt="">
                        <img class="w-4 h-4" v-for="i in (5 - item.rating)" index="i" src="/assets/star-border.png" alt="">
                    </div>
                    <p class="text-lg text-white">{{ item.description }}</p>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="rounded-[50px] bg-[#0F1735]" id="projects" >
        <div class="mt-8 p-14">
            <h2 class="text-4xl font-bold mb-10 text-white text-center">Projects</h2>
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
    <section id="contact" class="rounded-[50px] bg-[#0F1735]">
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

<script>
export default {
    data: () => ({
        languages: [
            {
                name: 'JavaScript',
                image: '/assets/js.png',
                description: 'bla bla',
                rating: 5
            },
            {
                name: 'Python',
                image: '/assets/python.png',
                rating: 3
            },
            {
                name: 'Java',
                image: '/assets/java.png',
                rating: 3
            }],
        companies: [
            {
                name: 'Nubank',
                from: 'February 2024',
                to: 'Present',
                role: 'Software Developer',
                image: '/assets/nubank_logo.png'
            },
            {
                name: 'Cafeto',
                from: 'July 2021',
                to: 'July 2023',
                role: 'Integrations Engineer',
                image: '/assets/cafeto_logo.png'
            },
            {
                name: 'Masiv',
                from: 'Jan 2020',
                to: 'July 2021',
                role: 'Software Developer',
                image: '/assets/masiv_logo.png'
            },
            {
                name: 'IBM',
                from: 'July 2019',
                to: 'Dec 2019',
                role: 'Software Intern',
                image: '/assets/ibm_logo.png'
            },
        ]
    }),
    methods: {
        scrollToSection(section) {
            const el = document.getElementById(section);
            el.scrollIntoView({ behavior: 'smooth' });
        }
    }
}
</script>