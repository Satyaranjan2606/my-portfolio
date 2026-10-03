<template>
  <div class="min-h-screen bg-zinc-950 text-zinc-100 font-sans">
    <!-- Fixed Navbar -->
    <nav
      class="fixed top-0 left-0 right-0 z-50 bg-zinc-950/80 backdrop-blur-md border-b border-zinc-800/70"
    >
      <div
        class="max-w-7xl mx-auto px-5 sm:px-8 py-4 flex items-center justify-between"
      >
        <div class="flex items-center gap-3">
          <div
            class="w-10 h-10 bg-yellow-500 rounded-xl flex items-center justify-center font-bold text-zinc-950 text-xl shadow-md"
          >
            SM
          </div>
          <span class="text-xl font-semibold tracking-tight"
            >Satyaranjan Mohanty</span
          >
        </div>

        <div class="hidden md:flex items-center gap-8 text-sm font-medium">
          <a href="#summary" class="hover:text-yellow-400 transition-colors"
            >Summary</a
          >
          <a href="#experience" class="hover:text-yellow-400 transition-colors"
            >Experience</a
          >
          <a href="#projects" class="hover:text-yellow-400 transition-colors"
            >Projects</a
          >
          <a href="#education" class="hover:text-yellow-400 transition-colors"
            >Education</a
          >
          <a href="#skills" class="hover:text-yellow-400 transition-colors"
            >Skills</a
          >
        </div>

        <a
          href="https://www.linkedin.com/in/satyaranjan-mohanty-0650981aa/"
          target="_blank"
          class="flex items-center gap-2 bg-yellow-500 hover:bg-yellow-400 text-zinc-950 px-5 py-2.5 rounded-full font-medium transition-colors"
        >
          <i class="fa-brands fa-linkedin"></i>
          LinkedIn
        </a>
      </div>
    </nav>

    <!-- Hero / Header -->
    <header
      class="pt-28 pb-16 md:pt-36 md:pb-24 bg-gradient-to-b from-zinc-900 to-zinc-950"
    >
      <div class="max-w-6xl mx-auto px-5 sm:px-8 text-center">
        <div class="inline-flex items-center gap-3 mb-6">
          <img
            src="/profile.png"
            alt="Profile"
            class="w-20 h-20 rounded-full object-cover border-4 border-yellow-500/30"
          />
          <div class="text-left">
            <h1 class="text-4xl md:text-5xl font-bold tracking-tight">
              SATYARANJAN MOHANTY
            </h1>
            <p class="text-xl text-yellow-400 font-medium">
              Software Engineer | Backend &amp; Full-Stack Developer
            </p>
            <p class="text-sm text-zinc-400 mt-1">PHP · Laravel · REST APIs</p>
          </div>
        </div>

        <div
          class="flex flex-wrap justify-center gap-x-6 gap-y-3 text-zinc-300 mt-6"
        >
          <div class="flex items-center gap-2">
            <i class="fa-regular fa-envelope text-yellow-400"></i>
            <a
              href="mailto:satyaranjan2606@gmail.com"
              class="hover:text-yellow-400"
              >satyaranjan2606@gmail.com</a
            >
          </div>
          <div class="flex items-center gap-2">
            <i class="fa-solid fa-phone text-yellow-400"></i>
            <span>+91 73770 73494</span>
          </div>
          <div class="flex items-center gap-2">
            <i class="fa-solid fa-location-dot text-yellow-400"></i>
            <span>Bhubaneswar, Odisha, India</span>
          </div>
          <a
            href="https://satyaranjan2606.github.io/my-portfolio/"
            target="_blank"
            class="flex items-center gap-2 hover:text-yellow-400"
          >
            <i class="fa-solid fa-globe text-yellow-400"></i>
            <span>Portfolio</span>
          </a>
        </div>
      </div>
    </header>

    <main class="max-w-6xl mx-auto px-5 sm:px-8 pb-24 space-y-24">
      <!-- SUMMARY -->
      <section id="summary">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          SUMMARY
        </h2>
        <div
          class="prose prose-invert max-w-none text-lg leading-relaxed text-zinc-300"
        >
          <p>
            Backend-focused Software Engineer with 3+ years of professional
            experience building scalable Laravel/PHP web applications and
            high-throughput REST APIs. Proven track record integrating 5+
            payment gateways that process 50,000+ monthly transactions, and
            optimizing MySQL and Oracle queries to cut execution time by 25%.
            Experienced in engineering enterprise AI applications using Python,
            Retrieval-Augmented Generation (RAG), and local Large Language
            Models (LLMs).
          </p>
        </div>
      </section>

      <!-- EXPERIENCE -->
      <section id="experience">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          EXPERIENCE
        </h2>
        <div class="bg-zinc-900/60 rounded-2xl p-8 border border-zinc-800">
          <div
            class="flex flex-col sm:flex-row sm:justify-between sm:items-start gap-4 mb-6"
          >
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
            <li>
              Developed and deployed scalable Laravel applications using MVC
              architecture, improving maintainability, reducing deployment lead
              times by 20%, and boosting backend performance by 30%
            </li>
            <li>
              Designed and implemented 10+ high-throughput RESTful APIs and
              integrated 5+ secure payment gateways (PayPal, Stripe, Razorpay,
              CCAvenue, Dodo Payments), processing 50,000+ monthly financial
              transactions
            </li>
            <li>
              Engineered secure user authentication, authorization, and
              Role-Based Access Control (RBAC) across 3+ enterprise applications
            </li>
            <li>
              Optimized complex MySQL and Oracle queries using indexing
              strategies, query tuning, and Eloquent ORM best practices, cutting
              execution latency by 25%
            </li>
            <li>
              Collaborated in cross-functional Agile/Scrum teams on debugging,
              production support, and continuous integration, accelerating
              sprint completion by 15%
            </li>
          </ul>
        </div>
      </section>

      <!-- PROJECTS -->
      <section id="projects">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          PROJECTS
        </h2>
        <div class="grid md:grid-cols-2 gap-8">
          <div
            v-for="project in projects"
            :key="project.title"
            class="bg-zinc-900/60 rounded-2xl p-7 border border-zinc-800 hover:border-yellow-500/50 transition-colors flex flex-col"
          >
            <h3 class="text-2xl font-semibold text-yellow-400 mb-3">
              {{ project.title }}
            </h3>
            <ul
              class="list-disc list-inside space-y-2 text-zinc-300 leading-relaxed mb-4"
            >
              <li v-for="point in project.points" :key="point">{{ point }}</li>
            </ul>
            <div class="mt-auto flex flex-wrap gap-2">
              <span
                v-for="tech in project.stack"
                :key="tech"
                class="text-xs px-3 py-1 bg-zinc-800 rounded-full border border-zinc-700 text-zinc-300"
              >
                {{ tech }}
              </span>
            </div>
          </div>
        </div>
      </section>

      <!-- EDUCATION -->
      <section id="education">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          EDUCATION
        </h2>
        <div class="space-y-10">
          <div
            v-for="edu in education"
            :key="edu.degree"
            class="bg-zinc-900/40 rounded-xl p-7 border border-zinc-800"
          >
            <h3 class="text-2xl font-semibold">{{ edu.degree }}</h3>
            <p class="text-yellow-400 mt-1">{{ edu.institution }}</p>
            <p class="text-zinc-400 text-sm">{{ edu.period }}</p>
            <p class="mt-4 text-zinc-300">{{ edu.details }}</p>
          </div>
        </div>
      </section>

      <!-- SKILLS -->
      <section id="skills">
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          SKILLS
        </h2>
        <div class="space-y-6">
          <div v-for="group in skillGroups" :key="group.label">
            <h4
              class="text-yellow-400 text-sm font-semibold uppercase tracking-wide mb-3"
            >
              {{ group.label }}
            </h4>
            <div class="flex flex-wrap gap-3">
              <span
                v-for="skill in group.items"
                :key="skill"
                class="px-5 py-2.5 bg-zinc-800 rounded-full text-sm font-medium border border-zinc-700 hover:border-yellow-500/50 transition-colors"
              >
                {{ skill }}
              </span>
            </div>
          </div>
        </div>
      </section>

      <!-- LANGUAGES -->
      <section>
        <h2 class="text-4xl font-bold mb-8 border-l-4 border-yellow-500 pl-5">
          LANGUAGES
        </h2>
        <div class="flex flex-wrap gap-6 text-lg">
          <span
            v-for="lang in languages"
            :key="lang"
            class="flex items-center gap-2"
          >
            <i class="fa-solid fa-language text-yellow-400"></i> {{ lang }}
          </span>
        </div>
      </section>
    </main>

    <!-- Footer -->
    <footer class="bg-black py-12 border-t border-zinc-800">
      <div class="max-w-6xl mx-auto px-5 sm:px-8 text-center text-zinc-400">
        <p>
          © {{ new Date().getFullYear() }} Satyaranjan Mohanty • Made with
          Laravel passion &amp; Vue
        </p>
        <a
          href="https://www.linkedin.com/in/satyaranjan-mohanty-0650981aa/"
          target="_blank"
          class="inline-flex items-center gap-2 mt-4 text-yellow-400 hover:text-yellow-300"
        >
          <i class="fa-brands fa-linkedin text-xl"></i>
          Connect on LinkedIn
        </a>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref } from "vue";

const projects = ref([
  {
    title: "AI Resume Screening Application",
    points: [
      "Automated resume evaluation against job descriptions using locally hosted LLMs and RAG pipelines",
      "Automated candidate shortlisting, interview scheduling, and notification workflows",
      "Containerized AI models, pipelines, and microservices with Docker for reliable multi-environment deployment",
    ],
    stack: [
      "Laravel",
      "Python",
      "Docker",
      "Ollama",
      "Qwen 2.5",
      "LangChain",
      "REST APIs",
    ],
  },
  {
    title: "Leadztree – Global Business Intelligence Platform",
    points: [
      "High-volume company and contact discovery platform with multi-parameter filtering across MCA records for USA, Canada, and India",
      "Decoupled architecture: Laravel client communicating with custom PHP REST APIs",
      "AI-driven data enrichment pipeline to cleanse, standardize, and process enterprise contact records at scale",
    ],
    stack: ["Laravel", "PHP", "REST APIs", "Python", "AI Data Enrichment"],
  },
  {
    title: "BizNow – Local Business Directory with AI Search",
    points: [
      "Business directory with AI-powered semantic search",
      "Dynamic ranking algorithms to surface sponsored listings",
    ],
    stack: ["Laravel", "MySQL", "Ollama", "Qwen 2.5", "REST APIs"],
  },
  {
    title: "DelveIn – Corporate Data Platform",
    points: [
      "Corporate search and director profile retrieval workflows",
      "High-performance SQL query optimization and indexing",
    ],
    stack: ["Laravel", "MySQL", "REST APIs", "Database Indexing"],
  },
  {
    title: "Morsh Golf – E-Commerce Web Application",
    points: [
      "Full-stack e-commerce platform with product catalog management and order processing",
      "Payment gateway integration via Razorpay and Stripe",
    ],
    stack: ["Laravel", "MySQL", "Razorpay", "Stripe", "REST APIs"],
  },
  {
    title: "CIMFR – Dynamic Mining Report System",
    points: [
      "Dynamic report generation engine for mining operations and personnel management",
      "Automated regulatory reporting workflows",
    ],
    stack: ["Laravel", "MySQL"],
  },
  {
    title: "The Samaja TMS – Time Management System",
    points: [
      "Internal operational management system for daily time tracking, employee reporting, and workflow tracking",
    ],
    stack: ["Laravel", "MySQL", "Agile"],
  },
]);

const education = ref([
  {
    degree: "Master of Computer Applications (MCA)",
    institution: "Trident Academy of Technology, Bhubaneswar, Odisha",
    period: "2019 – 2022",
    details:
      "Relevant coursework: Data Structures & Algorithms, Database Management Systems (DBMS), Software Engineering, Web Technologies",
  },
  {
    degree: "B.Sc. Chemistry (Honours)",
    institution: "Utkal University, Bhubaneswar, Odisha",
    period: "2015 – 2018",
    details: "Graduated with Honours",
  },
]);

const skillGroups = ref([
  {
    label: "Backend Development",
    items: [
      "PHP",
      "Laravel",
      "RESTful APIs",
      "Microservices",
      "MVC Architecture",
      "OOP",
      "Eloquent ORM",
      "Authentication",
      "Authorization",
      "RBAC",
    ],
  },
  {
    label: "AI & Data Engineering",
    items: [
      "Python",
      "RAG",
      "LLMs",
      "LangChain",
      "Ollama",
      "Qwen 2.5",
      "Web Scraping",
    ],
  },
  {
    label: "Databases & Architecture",
    items: [
      "MySQL",
      "PostgreSQL",
      "Oracle DB",
      "RDBMS",
      "Schema Design",
      "Database Indexing",
      "Query Optimization",
    ],
  },
  {
    label: "Payment Gateways & Integrations",
    items: [
      "Stripe",
      "PayPal",
      "Razorpay",
      "CCAvenue",
      "Dodo Payments",
      "Third-Party API Integration",
    ],
  },
  {
    label: "Frontend Development",
    items: ["JavaScript", "Vue.js", "HTML5", "CSS3", "Responsive Web Design"],
  },
  {
    label: "Tools, DevOps & Methodologies",
    items: [
      "Docker",
      "Containerization",
      "Git",
      "GitHub",
      "Unit Testing",
      "Agile",
      "Scrum",
      "SDLC",
      "Debugging",
      "Production Support",
    ],
  },
]);

const languages = ref([
  "English (Professional Working)",
  "Hindi (Full Professional)",
  "Odia (Native)",
]);
</script>
