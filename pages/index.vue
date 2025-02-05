<template>
    <nav class="p-4 bg-[#0F1735] overflow-hidden z-10">
        <div class="absolute
                w-56
                h-56
                top-[-15%]
                left-[-10%]
                bg-[#e8f99253]
                rounded-full
                blur-3xl
                z-11"></div>
        <ul class="flex justify-center w-full">
            <li @click="scrollToSection('about')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer mx-5">About</li>
            <li @click="scrollToSection('skills')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer mx-5">Skills</li>
            <li @click="scrollToSection('projects')" class="text-lg font-semibold text-white hover:text-gray-300 cursor-pointer mx-5">Projects</li>
        </ul>
    </nav>

    <section class="flex h-130 rounded-b-[50px] bg-[#0F1735] overflow-hidden justify-center relative z-10">
        <img class="h-35 absolute left-0 bottom-30" src="/assets/Vector2.png" alt="">
        <img class="h-10 absolute right-0 top-0" src="/assets/Vector3.png" alt="">
        <div class="flex h-full w-full max-w-6xl relative">
            <div class="mx-10 mt-10 w-full relative">
                <div>
                    <h1 class="text-5xl sm:text-6xl md:text-8xl font-extrabold mb-4 text-white text-center md:text-left">I'm <span class="text-[#E8F992] italic">Nicolás Gómez</span></h1>
                    <p class="text-2xl md:text-3xl font-semibold text-white text-center md:text-left">A Backend Developer and Software Engineer</p>
                </div>
                
                <div class="hidden md:block">
                    
                    <div class="text-white text-md max-w-xl">
                        Hi, I'm Nicolas Gomez, a passionate and dedicated software engineer with 5 years of experience specializing in backend development.
                    </div>
                </div>
                <div class="hidden
                absolute
                justify-between
                w-full
                mt-10
                space-y-4
                items-center
                bottom-35
                sm:flex
                md:static
                md:justify-normal
                md:flex-row
                md:space-x-4
                md:space-y-0
                ">
                    <button @click="scrollToSection('projects')" class="cursor-pointer mt-8 px-6 py-2 border-2 text-black rounded-full bg-[#E8F992] hover:bg-[#9ca861] hover:text-[#0F1735] transition duration-300">
                        View Projects
                    </button>
                    <button @click="scrollToSection('contact')" class="cursor-pointer mt-8 px-6 py-2 border-2 border-white text-white rounded-full bg-transparent hover:bg-white hover:text-[#0F1735] transition duration-300">
                        Contact Me
                    </button>
                </div>
                <div class="absolute
                bottom-30
                hidden
                lg:block
                lg:bottom-10">
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
            </div>
            <div class="flex justify-center h-76 md:h-76 bottom-0 md:right-0 left-1/2 md:left-auto -translate-x-1/2 md:translate-x-0 absolute flex-none">
                <!-- Background Blur Circle -->
                <div class="absolute
                w-76
                h-76
                bottom-[-20%]
                bg-[#e8f99284]
                rounded-full
                blur-3xl"></div>

                <!-- Image (Appears Above the Div) -->
                <img class="relative
                h-70
                z-10
                min-w-[403px]
                sm:min-w-[427px]
                sm:h-76
                sm:bottom-0
                bottom-[-10%]" src="/picture.png" alt="">
                
            </div>
        </div>
        <img class="h-25 md:h-35 absolute right-0 bottom-60 md:bottom-30" src="/assets/Vector.png" alt="">
    </section>
    <section id="about" class="relative z-0">
        <div class="absolute
                w-76
                h-76
                top-[-10%]
                left-[-12%]
                bg-[#e8f99243]
                rounded-full
                blur-3xl
                z-2">
        </div>
        <img class="h-20 absolute right-0 top-0" src="/assets/Vector4.png" alt="">
        <div class="mt-8 p-14 z-4">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">About <span class="text-[#E8F992] italic">Me</span></h2>
            <p class="text-lg text-white text-center">
                I'm a software engineer with five years of experience in building high-quality, impactful software solutions. Passionate about creating efficient and user-friendly products, I continuously explore new technologies and refine my skills to adapt to evolving challenges. My goal is to develop software that enhances everyday life, streamlines processes, and drives meaningful improvements.
            </p>
        </div>
    </section>
    <section class="rounded-[50px] bg-[#0F1735] z-10 relative">
        <div class="mt-8 text-white p-14">
            <h2 class="text-4xl font-bold mb-10"> My <span class="text-[#E8F992] italic">Experience</span></h2>
            <div class="absolute
                w-76
                h-76
                left-[-20%]
                bottom-15
                bg-[#e8f99243]
                rounded-full
                blur-3xl
                z-2"></div>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4">
                <div v-for="item in companies" class="bg-white/10 p-4 rounded-3xl border-1 text-white min-w-[250px]">
                    <img class="h-14 w-14 mb-4" :src="item.image" alt="">
                    <h3 class="text-2xl mb-4">{{ item.role }}</h3>
                    <p class="text-md text-white mb-4">{{ item.from }} - {{ item.to }}</p>
                </div>
            </div>
            <img class="h-20 absolute right-0 bottom-25" src="/assets/Vector5.png" alt="">
        </div>
    </section>
    <section id="skills" class="relative z-0">
        <div class="absolute
                w-96
                h-96
                left-[-35%]
                bottom-[-20%]
                bg-[#e8f9926a]
                rounded-full
                blur-3xl
                z-2"></div>
        <div class="mt-8 text-white py-14">
            <h2 class="text-4xl font-bold mb-10 text-center">Programming <span class="text-[#E8F992] italic">Languages & Technologies</span></h2>
                
            <div class="md:overflow-hidden overflow-x-auto px-14 [&::-webkit-scrollbar]:hidden [-ms-overflow-style:none] [scrollbar-width:none] z-5 pr-14">
                <div class="grid
                grid-rows-[repeat(3,minmax(0,1fr))]
                auto-cols-[minmax(300px,1fr)]
                grid-flow-col
                md:grid-flow-row
                md:grid-cols-2
                md:grid-rows-auto
                lg:auto-cols-auto
                lg:grid-cols-3
                gap-4
                pb-4">
                    <div v-for="item in languages" class="bg-white/10 p-4 rounded-3xl border-1 text-white flex min-w-[250px] max-w-[400px] h-[130px]">
                        <img class="h-20 w-20 mr-4" :src="item.image" alt="">
                        <div>
                            <h3 class="text-2xl font-semibold mr-3">{{item.name}}</h3>
                            <div class="flex items-center">
                                <img class="w-4 h-4 mr-1" v-for="i in item.rating" src="/assets/star.png" alt="">
                                <img class="w-4 h-4 mr-1" v-for="i in (5 - item.rating)" index="i" src="/assets/star-border.png" alt="">
                                ({{ item.rating }}/5)
                            </div>
                            <p class="text-lg text-white">{{ item.description }}</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
    <section class="rounded-[50px] bg-[#0F1735] relative z-10 overflow-hidden" id="projects" >
        <div class="mt-8 p-14">
            <h2 class="text-4xl font-bold mb-10 text-white "> Projects I've <span class="text-[#E8F992] italic">Worked On</span></h2>
            <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
                
                <div v-for="item in projects" class="bg-[#ffffffcc] rounded-lg z-11 project-card min-w-[250px]">
                    <img :src="item.image" alt="Project 1" class="w-full h-48 object-cover object-top rounded-t-lg cursor-pointer" @click="goToProject(item.url)">
                    <div class="px-4 py-2">
                        <h3 class="text-xl font-semibold">{{ item.name }}</h3>
                        <p class="text-sm">{{ item.description }}</p>
                        <div class="flex flex-wrap">
                            <span v-for="tech in item.technologies" class="text-xs bg-gray-200 px-2 py-1 rounded-full mr-2 mt-1">{{ tech }}</span>
                        </div>
                        <a v-if="item.github" :href="item.github" target="_blank" class="text-xs bg-[#E8F992] px-2 py-1 rounded-full mr-2 mt-1 font-bold"><\></a>
                    </div>
                </div>
            </div>
            <div class="absolute
                w-96
                h-96
                left-[-25%]
                bottom-[-20%]
                bg-[#e8f9926a]
                rounded-full
                blur-3xl
                z-2"></div>
        </div>
    </section>
    <section id="contact" class="rounded-[50px] bg-[#0F1735] p-14 mt-8">
        <div class="mt-8">
            <h2 class="text-4xl font-bold mb-2 text-white text-center">Nicolás <span class="text-[#E8F992]">Gómez</span></h2>
            <div class="flex flex-row">
                
            </div>
            <div class="flex flex-col md:flex-row w-full justify-center items-center md:space-x-6 space-y-4 md:space-y-0 my-5">
                <p class="text-lg text-white rounded-full outline outline-white pl-1 pr-3 py-1 flex items-center w-[200px] mx-5 my-3">
                    <img src="/assets/phone.png" alt="Phone" class="h-8 w-8 mr-1">
                    +57 3194396360
                </p>
                <p class="text-lg text-white rounded-full outline outline-white pl-1 pr-3 py-1 flex items-center w-[270px] mx-5 my-3">
                    <img src="/assets/mail.png" alt="Email" class="h-8 w-8 mr-1">
                    nicolas.gm243@gmail.com
                </p>
                <p class="text-lg text-white rounded-full outline outline-white pl-1 pr-3 py-1 flex items-center w-[200px] mx-5 my-3">
                    <img src="/assets/location.png" alt="Location" class="h-8 w-8 mr-1">
                    Bogotá, Colombia
                </p>
            </div>
            
            <div class="flex flex-row justify-center w-full space-x-4 my-5">
                <a href="https://linkedin.com/in/nicolas-g" target="_blank" class="bg-white rounded-full p-2 hover:text-gray-900 h-10 w-10 mx-5 min-w-10">
                    <img src="/assets/linkedin.png" alt="LinkedIn" class="h-6 w-6">
                </a>
                <a href="https://github.com/jnicolasgomez" target="_blank" class="bg-white rounded-full p-2 hover:text-gray-900 h-10 w-10 mx-5 min-w-10">
                    <img src="/assets/github.png" alt="GitHub" class="h-6 w-6">
                </a>
                <a href="https://instagram.com/jnicolas_g_" target="_blank" class="bg-white rounded-full p-2 hover:text-gray-900 h-10 w-10 mx-5 min-w-10">
                    <img src="/assets/instagram.png" alt="Instagram" class="h-6 w-6">
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
                name: 'NodeJs',
                image: '/assets/js.png',
                description: '',
                rating: 5
            },
            {
                name: 'Typescript',
                image: '/assets/TypeScript.png',
                rating: 4
            },
            {
                name: 'Vue',
                image: '/assets/Vue.png',
                rating: 4
            },
            {
                name: 'Clojure',
                image: '/assets/Clojure.png',
                rating: 3
            },
            {
                name: 'Python',
                image: '/assets/python.png',
                rating: 3
            },
            {
                name: 'SQL',
                image: '/assets/sql.png',
                rating: 4
            },
            {
                name: 'AWS',
                image: '/assets/AWS.png',
                rating: 3
            },
            {
                name: 'Docker',
                image: '/assets/Docker.png',
                rating: 3
            },
            {
                name: 'Kubernetes',
                image: '/assets/Kubernetes.png',
                rating: 3
            },
            {
                name: 'Git',
                image: '/assets/Git.png',
                rating: 5
            }
        ],
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
        ],
        projects: [
            {
                name: 'Fullstack Songs and Chords App',
                image: '/assets/project-api.png',
                description: 'An app that allows you to store and edit your favorite songs and chords.',
                technologies: ['Node.js', 'Express', 'Firebase Auth','Firestore', 'MongoDB',  'Vue.js', 'Jest', 'Google Cloud'],
                url: 'https://proyectovertigo.com/chords',
                github: 'https://github.com/jnicolasgomez/songs-chords-api'
            },
            {
                name: 'Vertigo Band Website',
                image: '/assets/project-vertigo.png',
                description: 'A website for a band that also allows you to store your favorite songs and chords.',
                technologies: ['Vue.js', 'Firebase Auth', 'Jest'],
                url: 'https://proyectovertigo.com'
            },
            {
                name: 'Random Chords App',
                image: '/assets/project-random.jpg',
                description: 'A simple app that generates random chords and plays them with a metronome.',
                technologies: ['Vue.js', 'Quasar', 'Vite', 'Vue Router', 'Pinia'],
                url: 'https://randomchords.vercel.app/'
            },
            {
                name: 'Portfolio',
                image: '/assets/project-portfolio.png',
                description: 'My software engineer portfolio.',
                technologies: ['Vue.js', 'Nuxt.js', 'Tailwind CSS', 'Vite', 'Vue Router', 'Pinia', 'Vercel'],
                url: 'https://jnicolasgomez.vercel.app/'
            },
        ]
    }),
    methods: {
        scrollToSection(section) {
            const el = document.getElementById(section);
            el.scrollIntoView({ behavior: 'smooth' });
        },
        goToProject(url) {
            window.open(url, '_blank');
        }
    }
}
</script>

<style scoped>
    .project-card {
        transition: transform 0.3s ease;
    }
    .project-card:hover {
        transform: scale(1.05);
    }
</style>