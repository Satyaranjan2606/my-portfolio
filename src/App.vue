<template>
  <div class="min-h-screen bg-zinc-950 text-zinc-100 font-sans">

    <!-- Fixed Navbar -->
    <nav class="fixed top-0 left-0 right-0 z-50 bg-zinc-950/80 backdrop-blur-md border-b border-zinc-800/70">
      <div class="max-w-7xl mx-auto px-5 sm:px-8 py-4 flex items-center justify-between">
        <div class="flex items-center gap-3">
          <div
            class="w-10 h-10 bg-yellow-500 rounded-xl flex items-center justify-center font-bold text-zinc-950 text-xl shadow-md">
            SM
          </div>
          <span class="text-xl font-semibold tracking-tight">Satyaranjan Mohanty</span>
        </div>

        <div class="hidden md:flex items-center gap-8 text-sm font-medium">
          <a href="#summary" class="hover:text-yellow-400 transition-colors">Summary</a>
          <a href="#experience" class="hover:text-yellow-400 transition-colors">Experience</a>
          <a href="#projects" class="hover:text-yellow-400 transition-colors">Projects</a>
          <a href="#education" class="hover:text-yellow-400 transition-colors">Education</a>
          <a href="#skills" class="hover:text-yellow-400 transition-colors">Skills</a>
        </div>

        <a href="https://www.linkedin.com/in/satyaranjan-mohanty-0650981aa/" target="_blank"
          class="flex items-center gap-2 bg-yellow-500 hover:bg-yellow-400 text-zinc-950 px-5 py-2.5 rounded-full font-medium transition-colors">
          <i class="fa-brands fa-linkedin"></i>
          LinkedIn
        </a>
      </div>
    </nav>

    <!-- Hero / Header -->
    <header class="pt-28 pb-16 md:pt-36 md:pb-24 bg-gradient-to-b from-zinc-900 to-zinc-950">
      <div class="max-w-6xl mx-auto px-5 sm:px-8 text-center">
        <div class="inline-flex items-center gap-3 mb-6">
          <img src="/profile.png" alt="Profile"
            class="w-20 h-20 rounded-full object-cover border-4 border-yellow-500/30">
          <div class="text-left">
            <h1 class="text-4xl md:text-5xl font-bold tracking-tight">SATYARANJAN MOHANTY</h1>
            <p class="text-xl text-yellow-400 font-medium">Software Engineer</p>
          </div>
        </div>

        <div class="flex flex-wrap justify-center gap-x-6 gap-y-3 text-zinc-300 mt-6">
          <div class="flex items-center gap-2">
            <i class="fa-regular fa-envelope text-yellow-400"></i>
            <a href="mailto:satyaranjan2606@gmail.com" class="hover:text-yellow-400">satyaranjan2606@gmail.com</a>
          </div>
          <div class="flex items-center gap-2">
            <i class="fa-solid fa-phone text-yellow-400"></i>
            <span>+91 73770 73494</span>
          </div>
          <div class="flex items-center gap-2">
            <i class="fa-solid fa-location-dot text-yellow-400"></i>
            <span>Bhubaneswar, India</span>
          </div>
        </div>
      </div>
    </header>

    <main class="max-w-6xl mx-auto px-5 sm:px-8 pb-24 space-y-24">

      <!-- SUMMARY -->
      <section id="summary">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">SUMMARY</h2>
        <div class="prose prose-invert max-w-none text-lg leading-relaxed text-zinc-300">
          <p>
            Developed and deployed scalable Laravel web applications using MVC architecture, improving maintainability
            and reducing deployment time by 20%.
            Designed and implemented 10+ RESTful APIs and integrated 5+ payment gateways (PayPal, Stripe, Razorpay,
            CCAvenue, Dodo Payments), supporting 50,000+ monthly transactions.
            Implemented secure authentication, authorization, and RBAC across 3+ applications.
            Optimized MySQL queries through indexing, query tuning, and Eloquent ORM best practices, reducing execution
            time by 25%.
            Improved backend performance by 30% via code refactoring, query optimization, and efficient Laravel Eloquent
            usage.
            Collaborated in Agile/Scrum teams for debugging, production support, and feature enhancements, achieving 15%
            faster sprint completion.
          </p>
        </div>
      </section>

      <!-- EXPERIENCE -->
      <section id="experience">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">EXPERIENCE</h2>
        <div class="bg-zinc-900/60 rounded-2xl p-8 border border-zinc-800">
          <div class="flex flex-col sm:flex-row sm:justify-between sm:items-start gap-4 mb-6">
            <div>
              <h3 class="text-2xl font-semibold">Software Engineer</h3>
              <p class="text-yellow-400">Sybrant Technologies</p>
              <p class="text-zinc-400 text-sm">Venkata Rathinam Nagar, Adyar, Chennai, Tamil Nadu</p>
            </div>
            <div class="text-right">
              <time class="text-zinc-400">Mar 2023 – Present</time>
            </div>
          </div>
          <div class="prose prose-invert max-w-none text-zinc-300">
            <p>
              Results-driven Software Engineer with 3+ years of experience in PHP and Laravel MVC development. Expert in
              building scalable web applications, designing RESTful APIs, payment gateway integrations (Razorpay,
              Stripe, PayPal, CCAvenue), and optimizing MySQL and Oracle databases. Skilled in backend architecture,
              RBAC (Role-Based Access Control), secure authentication & authorization, and production performance
              tuning. Proven track record delivering secure, high-performance solutions in Agile/Scrum environments.
            </p>
          </div>
        </div>
      </section>

      <!-- PROJECTS -->
      <section id="projects">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">PROJECTS</h2>
        <div class="grid md:grid-cols-2 gap-8">
          <div v-for="project in projects" :key="project.title"
            class="bg-zinc-900/60 rounded-2xl p-7 border border-zinc-800 hover:border-yellow-500/50 transition-colors">
            <h3 class="text-2xl font-semibold text-yellow-400 mb-3">
              {{ project.title }}
              <a v-if="project.url" :href="project.url" target="_blank" class="text-yellow-300 hover:underline">
                ({{ project.url }})
              </a>
            </h3>
            <p class="text-zinc-300 leading-relaxed">{{ project.description }}</p>
          </div>
        </div>
      </section>

      <!-- EDUCATION -->
      <section id="education">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">EDUCATION</h2>
        <div class="space-y-10">
          <div v-for="edu in education" :key="edu.degree" class="bg-zinc-900/40 rounded-xl p-7 border border-zinc-800">
            <h3 class="text-2xl font-semibold">{{ edu.degree }}</h3>
            <p class="text-yellow-400 mt-1">{{ edu.institution }}</p>
            <p class="text-zinc-400 text-sm">{{ edu.period }}</p>
            <p class="mt-4 text-zinc-300">{{ edu.details }}</p>
          </div>
        </div>
      </section>

      <!-- SKILLS -->
      <section id="skills">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">SKILLS</h2>
        <div class="flex flex-wrap gap-3">
          <span v-for="skill in skills" :key="skill"
            class="px-5 py-2.5 bg-zinc-800 rounded-full text-sm font-medium border border-zinc-700 hover:border-yellow-500/50 transition-colors">
            {{ skill }}
          </span>
        </div>
      </section>

      <!-- LANGUAGES -->
      <section>
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">LANGUAGES</h2>
        <div class="flex flex-wrap gap-6 text-lg">
          <span v-for="lang in languages" :key="lang" class="flex items-center gap-2">
            <i class="fa-solid fa-language text-yellow-400"></i> {{ lang }}
          </span>
        </div>
      </section>

    </main>

    <!-- Footer -->
    <footer class="bg-black py-12 border-t border-zinc-800">
      <div class="max-w-6xl mx-auto px-5 sm:px-8 text-center text-zinc-400">
        <p>© {{ new Date().getFullYear() }} Satyaranjan Mohanty • Made with Laravel passion & Vue</p>
        <a href="https://www.linkedin.com/in/satyaranjan-mohanty-0650981aa/" target="_blank"
          class="inline-flex items-center gap-2 mt-4 text-yellow-400 hover:text-yellow-300">
          <i class="fa-brands fa-linkedin text-xl"></i>
          Connect on LinkedIn
        </a>
      </div>
    </footer>

  </div>
</template>

<script setup>
import { ref } from 'vue'

const projects = ref([
  { title: "CIMFR", description: "Dynamic report generation system for mining operations and personnel services, built using Laravel + MySQL.", url: 'https://cimfr.res.in/' },
  { title: "Morsh Golf", description: "E-commerce web application with product management, order processing, and secure payment gateway integration (Razorpay + Stripe).", url: 'https://www.morshgolf.com/' },
  { title: "Dry Fruits (Online Store)", description: "E-commerce platform with catalog management, secure payment processing, and admin dashboard, built using Laravel.", url: '' },
  { title: "Delvein", description: "Corporate data platform with company search, director info retrieval, and optimized backend performance in Laravel + MySQL.", url: 'https://delvein.in/' }
])

const education = ref([
  { degree: "Master of Computer Applications (MCA)", institution: "Trident Academy of Technology, Bhubaneswar", period: "2019 – 2022", details: "Data Structures, DBMS, Software Engineering, Web Technologies" },
  { degree: "B.Sc. Chemistry (Honours)", institution: "Utkal University, Bhubaneswar", period: "2015 – 2018", details: "Graduated with Honours" }
])

const skills = ref([
  "Laravel Framework", "PHP", "RESTful APIs", "Vue.js", "JavaScript",
  "MySQL", "Oracle (Design & Optimization)", "Eloquent ORM",
  "Unit Testing", "Agile Methodology", "MVC Architecture", "OOP",
  "RBAC", "Payment Gateways Integration"
])

const languages = ref(["English", "Hindi", "Odia"])
</script>