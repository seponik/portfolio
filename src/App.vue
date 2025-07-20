<template>
  <div class="min-h-screen bg-slate-950 text-white overflow-x-hidden">
    <!-- Navigation -->
    <nav
      class="fixed top-0 left-0 right-0 z-50 bg-slate-950/90 backdrop-blur-xl border-b border-slate-800/50"
    >
      <div class="max-w-6xl mx-auto px-6 py-4">
        <div class="flex justify-between items-center">
          <div class="text-xl font-bold text-slate-200">Sepehr Bostandoust</div>
          <div class="hidden md:flex space-x-8">
            <a
              href="#about"
              class="text-slate-400 hover:text-blue-300 transition-colors duration-300"
              >About</a
            >
            <a
              href="#skills"
              class="text-slate-400 hover:text-blue-300 transition-colors duration-300"
              >Skills</a
            >
            <a
              href="#stats"
              class="text-slate-400 hover:text-blue-300 transition-colors duration-300"
              >Stats</a
            >
            <a
              href="#contact"
              class="text-slate-400 hover:text-blue-300 transition-colors duration-300"
              >Contact</a
            >
          </div>
          <button @click="toggleMobileMenu" class="md:hidden text-slate-400">
            <i class="ri-menu-line text-2xl"></i>
          </button>
        </div>
      </div>

      <!-- Mobile Menu -->
      <div
        v-if="mobileMenuOpen"
        class="md:hidden bg-slate-950/95 border-t border-slate-800/50"
      >
        <div class="px-6 py-4 space-y-4">
          <a
            href="#about"
            @click="toggleMobileMenu"
            class="block text-slate-400 hover:text-blue-300 transition-colors duration-300"
            >About</a
          >
          <a
            href="#skills"
            @click="toggleMobileMenu"
            class="block text-slate-400 hover:text-blue-300 transition-colors duration-300"
            >Skills</a
          >
          <a
            href="#stats"
            @click="toggleMobileMenu"
            class="block text-slate-400 hover:text-blue-300 transition-colors duration-300"
            >Stats</a
          >
          <a
            href="#contact"
            @click="toggleMobileMenu"
            class="block text-slate-400 hover:text-blue-300 transition-colors duration-300"
            >Contact</a
          >
        </div>
      </div>
    </nav>

    <!-- Hero Section -->
    <section
      class="min-h-screen flex items-center justify-center relative pt-20"
    >
      <div
        class="absolute inset-0 bg-gradient-to-br from-blue-950/30 via-slate-950 to-indigo-950/20"
      ></div>
      <div class="relative z-10 text-center max-w-4xl mx-auto px-6">
        <div class="mb-8 relative">
          <div
            class="w-32 h-32 mx-auto rounded-full bg-gradient-to-r from-blue-600/50 to-indigo-600/50 p-1"
          >
            <div
              class="w-full h-full rounded-full bg-slate-950 flex items-center justify-center"
            >
              <img
                src="https://github.com/seponik.png"
                alt="SB"
                class="rounded-full text-3xl font-bold"
              />
            </div>
          </div>
          <div
            class="absolute -top-2 -right-2 w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center animate-bounce"
          >
            👋
          </div>
        </div>

        <h1
          class="text-5xl md:text-7xl font-bold mb-6 bg-gradient-to-r from-blue-300 via-blue-200 to-indigo-300 bg-clip-text text-transparent animate-fade-in"
        >
          Hi, I'm Sepehr
        </h1>

        <!-- <p
          class="text-xl md:text-2xl text-slate-300 mb-8 animate-fade-in-delay-1"
        >
          Backend Developer & DevOps Engineer
        </p> -->

        <div
          class="flex flex-wrap justify-center gap-4 mb-12 animate-fade-in-delay-2"
        >
          <span
            class="px-4 py-2 bg-blue-900/30 border border-blue-800/50 rounded-full text-blue-200"
          >
            <i class="ri-code-line mr-2"></i>Backend Developer
          </span>
          <span
            class="px-4 py-2 bg-indigo-900/30 border border-indigo-800/50 rounded-full text-indigo-200"
          >
            <i class="ri-settings-3-line mr-2"></i>DevOps Engineer
          </span>
          <span
            class="px-4 py-2 bg-slate-800/50 border border-slate-700/50 rounded-full text-slate-300"
          >
            <i class="ri-community-line mr-2"></i>Community Founder
          </span>
        </div>

        <div class="animate-bounce">
          <a href="#about" class="inline-block">
            <i
              class="ri-arrow-down-line text-3xl text-blue-400 hover:text-blue-200 transition-colors duration-300"
            ></i>
          </a>
        </div>
      </div>

      <!-- Floating Elements -->
      <div
        class="absolute top-1/4 left-10 w-2 h-2 bg-blue-500 rounded-full animate-float opacity-60"
      ></div>
      <div
        class="absolute top-1/3 right-20 w-3 h-3 bg-indigo-500 rounded-full animate-float-delay-1 opacity-40"
      ></div>
      <div
        class="absolute bottom-1/4 left-1/4 w-2 h-2 bg-blue-400 rounded-full animate-float-delay-2 opacity-50"
      ></div>
    </section>

    <!-- About Section -->
    <section id="about" class="py-20 relative">
      <div class="max-w-6xl mx-auto px-6">
        <h2
          class="text-4xl md:text-5xl font-bold text-center mb-16 bg-gradient-to-r from-blue-300 to-indigo-300 bg-clip-text text-transparent"
        >
          About Me
        </h2>

        <div class="grid md:grid-cols-2 gap-12 items-center">
          <div class="space-y-6">
            <div
              class="p-6 bg-slate-900/40 border border-slate-800/50 rounded-xl backdrop-blur-sm hover:border-blue-700/50 transition-all duration-500 transform hover:scale-[1.02]"
            >
              <i class="ri-heart-pulse-line text-3xl text-blue-400 mb-4"></i>
              <p class="text-slate-300 leading-relaxed">
                I'm a passionate developer focused on web development and cloud
                technologies, with expertise in Backend and DevOps.
              </p>
            </div>

            <div
              class="p-6 bg-slate-900/40 border border-slate-800/50 rounded-xl backdrop-blur-sm hover:border-indigo-700/50 transition-all duration-500 transform hover:scale-[1.02]"
            >
              <i class="ri-team-line text-3xl text-indigo-400 mb-4"></i>
              <p class="text-slate-300 leading-relaxed">
                Founder of the
                <strong class="text-blue-200">Eskişehir Linux community</strong
                >, enjoying connections with others in the field.
              </p>
            </div>

            <div
              class="p-6 bg-slate-900/40 border border-slate-800/50 rounded-xl backdrop-blur-sm hover:border-blue-700/50 transition-all duration-500 transform hover:scale-[1.02]"
            >
              <i class="ri-book-open-line text-3xl text-blue-400 mb-4"></i>
              <p class="text-slate-300 leading-relaxed">
                Lifelong learner, always exploring new technologies!
              </p>
            </div>

            <div
              class="p-6 bg-slate-900/40 border border-slate-800/50 rounded-xl backdrop-blur-sm hover:border-indigo-700/50 transition-all duration-500 transform hover:scale-[1.02]"
            >
              <i class="ri-open-source-line text-3xl text-indigo-400 mb-4"></i>
              <p class="text-slate-300 leading-relaxed">
                A lover of open-source contributions and community projects.
              </p>
            </div>
          </div>

          <div class="relative">
            <div
              class="w-full h-96 bg-gradient-to-br from-blue-900/20 to-indigo-900/20 rounded-2xl border border-slate-800/50 backdrop-blur-sm p-8 flex items-center justify-center"
            >
              <div class="text-center">
                <i
                  class="ri-terminal-line text-6xl text-blue-300 mb-6 animate-pulse"
                ></i>
                <h3 class="text-2xl font-bold mb-4 text-slate-200">
                  Always Coding
                </h3>
                <p class="text-slate-400">
                  Building the future, one line at a time
                </p>
              </div>
            </div>
            <div
              class="absolute -top-4 -left-4 w-6 h-6 bg-blue-500 rounded-full animate-pulse opacity-60"
            ></div>
            <div
              class="absolute -bottom-4 -right-4 w-4 h-4 bg-indigo-500 rounded-full animate-pulse opacity-40"
            ></div>
          </div>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section id="skills" class="py-20 bg-slate-900/30">
      <div class="max-w-6xl mx-auto px-6">
        <h2
          class="text-4xl md:text-5xl font-bold text-center mb-16 bg-gradient-to-r from-indigo-300 to-blue-300 bg-clip-text text-transparent"
        >
          Skills & Technologies
        </h2>

        <!-- Languages -->
        <div class="mb-16">
          <h3
            class="text-2xl font-bold text-center mb-8 text-slate-200 flex items-center justify-center"
          >
            <i class="ri-code-s-slash-line mr-3 text-blue-400"></i>
            Languages
          </h3>
          <div class="flex flex-wrap justify-center gap-6">
            <div v-for="lang in languages" :key="lang.name" class="group">
              <div
                class="w-20 h-20 bg-slate-800/50 rounded-xl border border-slate-700/50 flex items-center justify-center hover:border-blue-600/70 hover:bg-blue-900/20 transition-all duration-300 transform hover:scale-110"
              >
                <img
                  :src="lang.icon"
                  :alt="lang.name"
                  class="w-10 h-10 object-contain opacity-80 group-hover:opacity-100 transition-opacity duration-300"
                />
              </div>
              <p
                class="text-center text-sm text-slate-400 mt-2 group-hover:text-blue-300 transition-colors duration-300"
              >
                {{ lang.name }}
              </p>
            </div>
          </div>
        </div>

        <!-- Tools -->
        <div>
          <h3
            class="text-2xl font-bold text-center mb-8 text-slate-200 flex items-center justify-center"
          >
            <i class="ri-tools-line mr-3 text-indigo-400"></i>
            Tools & DevOps
          </h3>
          <div class="flex flex-wrap justify-center gap-6">
            <div v-for="tool in tools" :key="tool.name" class="group">
              <div
                class="w-20 h-20 bg-slate-800/50 rounded-xl border border-slate-700/50 flex items-center justify-center hover:border-indigo-600/70 hover:bg-indigo-900/20 transition-all duration-300 transform hover:scale-110"
              >
                <img
                  :src="tool.icon"
                  :alt="tool.name"
                  class="w-10 h-10 object-contain opacity-80 group-hover:opacity-100 transition-opacity duration-300"
                />
              </div>
              <p
                class="text-center text-sm text-slate-400 mt-2 group-hover:text-indigo-300 transition-colors duration-300"
              >
                {{ tool.name }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Stats Section -->
    <section id="stats" class="py-20">
      <div class="max-w-6xl mx-auto px-6">
        <h2
          class="text-4xl md:text-5xl font-bold text-center mb-16 bg-gradient-to-r from-blue-300 to-indigo-300 bg-clip-text text-transparent"
        >
          GitHub Stats
        </h2>

        <div class="grid md:grid-cols-2 gap-8 max-w-4xl mx-auto">
          <div
            class="bg-slate-900/40 border border-slate-800/50 rounded-xl p-6 hover:border-blue-700/50 transition-all duration-500 transform hover:scale-[1.02]"
          >
            <div class="text-center">
              <h3
                class="text-xl font-bold mb-4 text-slate-200 flex items-center justify-center"
              >
                <i class="ri-bar-chart-line mr-3 text-blue-400"></i>
                Most Used Languages
              </h3>
              <img
                src="https://github-readme-stats.vercel.app/api/top-langs?username=seponik&locale=en&hide_title=true&layout=compact&card_width=320&langs_count=5&theme=dark&hide_border=true&bg_color=0f172a&text_color=cbd5e1&title_color=e2e8f0"
                alt="Top Languages"
                class="mx-auto rounded-lg"
              />
            </div>
          </div>

          <div
            class="bg-slate-900/40 border border-slate-800/50 rounded-xl p-6 hover:border-indigo-700/50 transition-all duration-500 transform hover:scale-[1.02]"
          >
            <div class="text-center">
              <h3
                class="text-xl font-bold mb-4 text-slate-200 flex items-center justify-center"
              >
                <i class="ri-trophy-line mr-3 text-indigo-400"></i>
                GitHub Achievements
              </h3>
              <div class="space-y-3">
                <div
                  class="flex items-center justify-between p-3 bg-slate-800/30 rounded-lg group hover:bg-blue-900/20 transition-all duration-300"
                >
                  <span class="text-slate-300">Galaxy Brain</span>
                  <div class="flex items-center">
                    <span class="text-xs text-slate-400 mr-2"
                      >Problem Solver</span
                    >
                    <i class="ri-brain-line text-blue-400"></i>
                  </div>
                </div>
                <div
                  class="flex items-center justify-between p-3 bg-slate-800/30 rounded-lg group hover:bg-indigo-900/20 transition-all duration-300"
                >
                  <span class="text-slate-300">Pair Extraordinaire</span>
                  <div class="flex items-center">
                    <span class="text-xs text-slate-400 mr-2"
                      >Collaboration</span
                    >
                    <i class="ri-team-line text-indigo-400"></i>
                  </div>
                </div>
                <div
                  class="flex items-center justify-between p-3 bg-slate-800/30 rounded-lg group hover:bg-orange-900/20 transition-all duration-300"
                >
                  <span class="text-slate-300">YOLO</span>
                  <div class="flex items-center">
                    <span class="text-xs text-slate-400 mr-2">Risk Taker</span>
                    <i class="ri-rocket-line text-orange-400"></i>
                  </div>
                </div>
                <div
                  class="flex items-center justify-between p-3 bg-slate-800/30 rounded-lg group hover:bg-green-900/20 transition-all duration-300"
                >
                  <span class="text-slate-300">Pull Shark</span>
                  <div class="flex items-center">
                    <span class="text-xs text-slate-400 mr-2">PR Master</span>
                    <i class="ri-git-pull-request-line text-green-400"></i>
                  </div>
                </div>
                <div
                  class="flex items-center justify-between p-3 bg-slate-800/30 rounded-lg group hover:bg-yellow-900/20 transition-all duration-300"
                >
                  <span class="text-slate-300">Quickdraw</span>
                  <div class="flex items-center">
                    <span class="text-xs text-slate-400 mr-2"
                      >Fast Responder</span
                    >
                    <i class="ri-flashlight-line text-yellow-400"></i>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- Contact Section -->
    <section id="contact" class="py-20 bg-slate-900/30">
      <div class="max-w-4xl mx-auto px-6 text-center">
        <h2
          class="text-4xl md:text-5xl font-bold mb-8 bg-gradient-to-r from-indigo-300 to-blue-300 bg-clip-text text-transparent"
        >
          Let's Connect
        </h2>

        <p class="text-xl text-slate-300 mb-12">
          Feel free to reach out for collaborations, opportunities, or just to
          say hi!
        </p>

        <div class="flex flex-wrap justify-center gap-6">
          <a
            href="https://www.linkedin.com/in/seponik/"
            target="_blank"
            class="group flex items-center space-x-3 bg-blue-900/30 border border-blue-800/50 px-6 py-4 rounded-xl hover:bg-blue-900/50 hover:border-blue-700/70 transition-all duration-300 transform hover:scale-105"
          >
            <i
              class="ri-linkedin-line text-2xl text-blue-300 group-hover:text-blue-200"
            ></i>
            <span class="text-slate-200 group-hover:text-blue-100"
              >LinkedIn</span
            >
          </a>

          <a
            href="mailto:sepehr.bsn@gmail.com"
            target="_blank"
            class="group flex items-center space-x-3 bg-indigo-900/30 border border-indigo-800/50 px-6 py-4 rounded-xl hover:bg-indigo-900/50 hover:border-indigo-700/70 transition-all duration-300 transform hover:scale-105"
          >
            <i
              class="ri-mail-line text-2xl text-indigo-300 group-hover:text-indigo-200"
            ></i>
            <span class="text-slate-200 group-hover:text-indigo-100"
              >Email</span
            >
          </a>

          <a
            href="https://www.instagram.com/seponik"
            target="_blank"
            class="group flex items-center space-x-3 bg-slate-800/40 border border-slate-700/50 px-6 py-4 rounded-xl hover:bg-slate-800/60 hover:border-slate-600/70 transition-all duration-300 transform hover:scale-105"
          >
            <i
              class="ri-instagram-line text-2xl text-slate-300 group-hover:text-slate-200"
            ></i>
            <span class="text-slate-200 group-hover:text-slate-100"
              >Instagram</span
            >
          </a>

          <a
            href="https://github.com/seponik"
            target="_blank"
            class="group flex items-center space-x-3 bg-slate-800/40 border border-slate-700/50 px-6 py-4 rounded-xl hover:bg-slate-800/60 hover:border-slate-600/70 transition-all duration-300 transform hover:scale-105"
          >
            <i
              class="ri-github-line text-2xl text-slate-300 group-hover:text-slate-200"
            ></i>
            <span class="text-slate-200 group-hover:text-slate-100"
              >GitHub</span
            >
          </a>
        </div>
      </div>
    </section>

    <!-- Footer -->
    <footer class="py-8 border-t border-slate-800/50">
      <div class="max-w-6xl mx-auto px-6 text-center">
        <p class="text-slate-400">
          Designed with
          <i class="ri-heart-fill text-red-500 mx-1"></i>
          by Sepehr Bostandoust
        </p>
      </div>
    </footer>
  </div>
</template>

<script setup>
import { ref, onMounted } from "vue";

const mobileMenuOpen = ref(false);

const languages = ref([
  { name: "JavaScript", icon: "https://skillicons.dev/icons?i=javascript" },
  { name: "C++", icon: "https://skillicons.dev/icons?i=cpp" },
  { name: "Go", icon: "https://skillicons.dev/icons?i=go" },
  { name: "Bash", icon: "https://skillicons.dev/icons?i=bash" },
]);

const tools = ref([
  { name: "Linux", icon: "https://skillicons.dev/icons?i=linux" },
  { name: "Docker", icon: "https://skillicons.dev/icons?i=docker" },
  { name: "Kubernetes", icon: "https://skillicons.dev/icons?i=kubernetes" },
  { name: "Jenkins", icon: "https://skillicons.dev/icons?i=jenkins" },
  { name: "Ansible", icon: "https://skillicons.dev/icons?i=ansible" },
  { name: "Prometheus", icon: "https://skillicons.dev/icons?i=prometheus" },
  { name: "Git", icon: "https://skillicons.dev/icons?i=git" },
]);

const toggleMobileMenu = () => {
  mobileMenuOpen.value = !mobileMenuOpen.value;
};

onMounted(() => {
  document.querySelectorAll('a[href^="#"]').forEach((anchor) => {
    anchor.addEventListener("click", function (e) {
      e.preventDefault();
      const target = document.querySelector(this.getAttribute("href"));
      if (target) {
        target.scrollIntoView({
          behavior: "smooth",
          block: "start",
        });
      }
    });
  });
});
</script>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes float {
  0%,
  100% {
    transform: translateY(0px);
  }
  50% {
    transform: translateY(-15px);
  }
}

.animate-fade-in {
  animation: fade-in 1s ease-out;
}

.animate-fade-in-delay-1 {
  animation: fade-in 1s ease-out 0.3s both;
}

.animate-fade-in-delay-2 {
  animation: fade-in 1s ease-out 0.6s both;
}

.animate-float {
  animation: float 4s ease-in-out infinite;
}

.animate-float-delay-1 {
  animation: float 4s ease-in-out infinite 1.5s;
}

.animate-float-delay-2 {
  animation: float 4s ease-in-out infinite 3s;
}

html {
  scroll-behavior: smooth;
}

::-webkit-scrollbar {
  width: 6px;
}

::-webkit-scrollbar-track {
  background: #0f172a;
}

::-webkit-scrollbar-thumb {
  background: #475569;
  border-radius: 3px;
}

::-webkit-scrollbar-thumb:hover {
  background: #64748b;
}
</style>
