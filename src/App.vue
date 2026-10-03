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
            <p class="text-sm text-zinc-400 mt-1">3+ Years Experience · Laravel · PHP · REST APIs</p>
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
            <span>Bhubaneswar, Odisha, India</span>
          </div>
          <a href="https://satyaranjan2606.github.io/my-portfolio/" target="_blank"
            class="flex items-center gap-2 hover:text-yellow-400">
            <i class="fa-solid fa-globe text-yellow-400"></i>
            <span>Portfolio</span>
          </a>
        </div>
      </div>
    </header>

    <main class="max-w-6xl mx-auto px-5 sm:px-8 pb-24 space-y-24">

      <!-- SUMMARY -->
      <section id="summary">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">SUMMARY</h2>
        <div class="prose prose-invert max-w-none text-lg leading-relaxed text-zinc-300">
          <p>
            Backend-focused Software Engineer with 3+ years of experience building scalable Laravel/PHP web
            applications and high-throughput REST APIs. Experienced in integrating multiple payment gateways
            (Razorpay, Stripe, PayPal, CCAvenue, Dodo Payments) handling 50,000+ monthly transactions, and
            optimizing MySQL and Oracle queries to reduce execution time by 25%. Skilled in authentication,
            RBAC, microservices, query optimization, and production performance tuning. Additionally
            experienced in engineering enterprise AI solutions using Python, RAG pipelines, and local LLMs;
            proficient with Docker, Vue.js, and agile development.
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
              <p class="text-zinc-400 text-sm">Chennai, Tamil Nadu, India</p>
            </div>
            <div class="text-right">
              <time class="text-zinc-400">Mar 2023 – Present</time>
            </div>
          </div>
          <ul class="list-disc list-inside space-y-2 text-zinc-300">
            <li>Developed and deployed scalable Laravel applications utilizing MVC architecture, improving codebase maintainability and reducing deployment lead times by 20%</li>
            <li>Designed and implemented 10+ high-throughput RESTful APIs and integrated 5+ secure payment gateways (PayPal, Stripe, Razorpay, CCAvenue, Dodo Payments), processing 50,000+ monthly financial transactions</li>
            <li>Engineered secure user authentication, authorization, and Role-Based Access Control (RBAC) protocols across multiple enterprise applications</li>
            <li>Optimized complex MySQL and Oracle database queries using indexing strategies, query tuning, and Eloquent ORM best practices, cutting execution latency by 25%</li>
            <li>Collaborated within cross-functional Agile/Scrum engineering teams on debugging, production support, and continuous integration, accelerating sprint completion rates by 15%</li>
          </ul>
        </div>
      </section>

      <!-- PROJECTS -->
      <section id="projects">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">PROJECTS</h2>
        <div class="grid md:grid-cols-2 gap-8">
          <div v-for="project in projects" :key="project.title"
            class="bg-zinc-900/60 rounded-2xl p-7 border border-zinc-800 hover:border-yellow-500/50 transition-colors flex flex-col">
            <h3 class="text-2xl font-semibold text-yellow-400 mb-3">{{ project.title }}</h3>
            <ul class="list-disc list-inside space-y-2 text-zinc-300 leading-relaxed mb-4">
              <li v-for="point in project.points" :key="point">{{ point }}</li>
            </ul>
            <div class="mt-auto flex flex-wrap gap-2">
              <span v-for="tech in project.stack" :key="tech"
                class="text-xs px-3 py-1 bg-zinc-800 rounded-full border border-zinc-700 text-zinc-300">
                {{ tech }}
              </span>
            </div>
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
        <div class="space-y-6">
          <div v-for="group in skillGroups" :key="group.label">
            <h4 class="text-yellow-400 text-sm font-semibold uppercase tracking-wide mb-3">{{ group.label }}</h4>
            <div class="flex flex-wrap gap-3">
              <span v-for="skill in group.items" :key="skill"
                class="px-5 py-2.5 bg-zinc-800 rounded-full text-sm font-medium border border-zinc-700 hover:border-yellow-500/50 transition-colors">
                {{ skill }}
              </span>
            </div>
          </div>
        </div>
      </section>

      <!-- ACHIEVEMENTS -->
      <section id="achievements">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">ACHIEVEMENTS</h2>
        <div class="bg-zinc-900/60 rounded-2xl p-8 border border-zinc-800">
          <h3 class="text-2xl font-semibold text-yellow-400 mb-3">Key Achievements</h3>
          <ul class="list-disc list-inside space-y-2 text-zinc-300">
            <li v-for="item in achievements" :key="item">{{ item }}</li>
          </ul>
        </div>
      </section>

      <!-- EXTRA-CURRICULAR -->
      <section id="extra">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">EXTRA-CURRICULAR ACTIVITIES</h2>
        <div class="bg-zinc-900/60 rounded-2xl p-8 border border-zinc-800">
          <h3 class="text-2xl font-semibold text-yellow-400 mb-3">{{ extra.title }}</h3>
          <p class="text-zinc-300 leading-relaxed">{{ extra.description }}</p>
        </div>
      </section>

      <!-- HOBBIES -->
      <section id="hobbies">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">HOBBIES</h2>
        <div class="flex flex-wrap gap-3">
          <span v-for="hobby in hobbies" :key="hobby"
            class="px-5 py-2.5 bg-zinc-800 rounded-full text-sm font-medium border border-zinc-700">
            {{ hobby }}
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
        <p>© {{ new Date().getFullYear() }} Satyaranjan Mohanty • Made with Laravel passion &amp; Vue</p>
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
  {
    title: "AI Resume Screening Application",
    points: [
      "Architected an automated resume evaluation application using locally hosted LLMs and RAG pipelines to analyze applicant profiles against target job descriptions",
      "Automated candidate shortlisting, interview scheduling, and notification workflows to streamline hiring operations",
      "Containerized AI models, processing pipelines, and microservices using Docker for consistent multi-environment deployment"
    ],
    stack: ["Laravel", "Python", "Docker", "Ollama", "Qwen 2.5", "LangChain", "RAG"]
  },
  {
    title: "DelveIn",
    points: [
      "Implemented a corporate data platform offering detailed insights into company records, including directors and financial metrics, with client-specific filtering",
      "Implemented filtering functionality to support timely retrieval of relevant business data"
    ],
    stack: ["Laravel", "MySQL", "REST APIs", "Query Optimization"]
  },
  {
    title: "Morsh Golf – E-Commerce Web Application",
    points: [
      "Developed a full-stack e-commerce platform with product catalog management, order processing systems, and payment gateway integrations (Razorpay, Stripe) to ensure smooth transactions and improved user experience"
    ],
    stack: ["Laravel", "MySQL", "Razorpay", "Stripe"]
  },
  {
    title: "Leadztree – Global Business Intelligence Platform",
    points: [
      "Developed a high-volume company and contact discovery platform featuring multi-parameter filtering across MCA records for USA, Canada, and India",
      "Implemented a decoupled architecture with a Laravel client communicating with custom PHP REST APIs, and integrated an AI-driven data enrichment pipeline to cleanse and standardize enterprise contact records"
    ],
    stack: ["Laravel", "PHP", "REST APIs", "Python", "AI Data Enrichment"]
  },
  {
    title: "BizNow – Local Business Directory with AI Search",
    points: [
      "Built a business directory featuring AI-powered semantic search and dynamic ranking algorithms to surface sponsored listings"
    ],
    stack: ["Laravel", "MySQL", "Ollama", "Qwen 2.5"]
  },
  {
    title: "CIMFR – Dynamic Mining Report System",
    points: [
      "Built a dynamic mining report generation system to schedule mining operations, compile detailed reports on partners and executives, and automate regulatory reporting workflows"
    ],
    stack: ["Laravel", "MySQL"]
  },
  {
    title: "The Samaja TMS – Time Management System",
    points: [
      "Engineered an internal time tracking and operational management system to streamline employee reporting and workflow tracking"
    ],
    stack: ["Laravel", "MySQL", "Agile"]
  },
])

const education = ref([
  { degree: "MCA | Computers", institution: "Trident Academy of Technology, Bhubaneswar", period: "2022", details: "Marks: 81%" },
  { degree: "B.Sc | Chemistry", institution: "Utkal University", period: "2018", details: "Marks: 59%" },
  { degree: "12th", institution: "Odisha, English", period: "2015", details: "Marks: 63%" },
  { degree: "10th", institution: "Odisha, Oriya", period: "2013", details: "Marks: 79%" }
])

const skillGroups = ref([
  { label: "Backend", items: ["Laravel PHP Framework", "PHP", "RESTful APIs", "Eloquent ORM", "Payment Gateways", "Query Optimization"] },
  { label: "Databases", items: ["MySQL", "Oracle", "PostgreSQL"] },
  { label: "AI & Data", items: ["Python", "Retrieval Augmented Generation", "Large Language Models"] },
  { label: "Frontend & DevOps", items: ["JavaScript", "Vue.js", "Docker"] },
])

const achievements = ref([
  "Integrated 5+ payment gateways supporting 50,000+ monthly transactions and reduced database query latency by 25% through indexing and optimization"
])

const extra = ref({
  title: "Technical Writing",
  description: "Authored technical notes and project documentation for internal projects and AI prototypes to improve knowledge transfer and onboarding."
})

const hobbies = ref(["Technical Blogging", "Open Source Contribution", "Competitive Coding"])

const languages = ref(["English", "Hindi", "Odia"])
</script>