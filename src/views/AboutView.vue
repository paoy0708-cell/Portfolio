<script>
export default {
  data() {
    return {
      activeTab: 1,
      tech: [
        {
          id: 1,
          name: "HTML",
          imageUrl: "https://cdn-icons-png.flaticon.com/512/1051/1051277.png",
          status: "Advanced",
        },
        {
          id: 2,
          name: "CSS",
          imageUrl: "https://cdn-icons-png.flaticon.com/512/732/732190.png",
          status: "Advanced",
        },
        {
          id: 3,
          name: "PHP",
          imageUrl:
            "https://cdn.iconscout.com/icon/free/png-256/free-php-2038871-1720084.png",
          status: "Advanced",
        },
        {
          id: 4,
          name: "Javascript",
          imageUrl:
            "https://cdn.icon-icons.com/icons2/2415/PNG/512/javascript_original_logo_icon_146455.png",
          status: "Advance",
        },
        {
          id: 5,
          name: "Laravel",
          imageUrl: "https://cdn.worldvectorlogo.com/logos/laravel-2.svg",
          status: "Advance",
        },
        {
          id: 6,
          name: "Codeigniter",
          imageUrl: "https://www.codeigniter.com/assets/icons/ci-logo.png",
          status: "Advance",
        },
        {
          id: 7,
          name: "VueJS",
          imageUrl:
            "https://cdn.iconscout.com/icon/free/png-256/free-vue-282497.png?f=webp",
          status: "Advance",
        },
        {
          id: 8,
          name: "AlpineJS",
          imageUrl:
            "https://avatars.githubusercontent.com/u/59030169?s=200&v=4",
          status: "Beginner",
        },
        {
          id: 9,
          name: "NodeJS",
          imageUrl:
            "https://cdn.iconscout.com/icon/free/png-256/free-node-js-1174925.png",
          status: "Advance",
        },
        {
          id: 10,
          name: "Tailwind",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/d/d5/Tailwind_CSS_Logo.svg",
          status: "Advance",
        },
        {
          id: 11,
          name: "Bootstrap",
          imageUrl:
            "https://getbootstrap.com/docs/5.2/assets/brand/bootstrap-logo-shadow.png",
          status: "Advance",
        },
        {
          id: 12,
          name: "ReactJS",
          imageUrl:
            "https://cdn4.iconfinder.com/data/icons/logos-3/600/React.js_logo-512.png",
          status: "Advance",
        },
        {
          id: 13,
          name: "Python",
          imageUrl:
            "https://s3.dualstack.us-east-2.amazonaws.com/pythondotorg-assets/media/community/logos/python-logo-only.png",
          status: "Advance",
        },
        {
          id: 14,
          name: "DeepLearning",
          imageUrl:
            "https://ai-dev.deeplearning.ai/images/sf/assets/deeplearning-logo.webp",
          status: "Advance",
        },
        {
          id: 15,
          name: "Ruby",
          imageUrl: "https://www.ruby-lang.org/images/header-ruby-logo.svg",
          status: "Advance",
        },
        {
          id: 16,
          name: "C++",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/1/18/ISO_C%2B%2B_Logo.svg/250px-ISO_C%2B%2B_Logo.svg.png",
          status: "Advance",
        },
        {
          id: 17,
          name: "C#",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Logo_C_sharp.svg/330px-Logo_C_sharp.svg.png?_=20221121173824",
          status: "Advance",
        },
        {
          id: 18,
          name: ".NET",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/7/7d/Microsoft_.NET_logo.svg/500px-Microsoft_.NET_logo.svg.png?_=20200524040737",
          status: "Advance",
        },
        {
          id: 19,
          name: "Angular",
          imageUrl:
            "https://angular.dev/assets/images/press-kit/angular_icon_gradient.gif",
          status: "Advance",
        },
        {
          id: 20,
          name: "Android",
          imageUrl:
            "https://developer.android.com/static/images/brand/android-head_flat.png",
          status: "Advance",
        },
        {
          id: 21,
          name: "Next.js",
          imageUrl:
            "https://icon.icepanel.io/Technology/png-shadow-512/Next.js.png",
          status: "Advance",
        },
        {
          id: 22,
          name: "OpenAI",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/thumb/6/66/OpenAI_logo_2025_%28symbol%29.svg/120px-OpenAI_logo_2025_%28symbol%29.svg.png",
          status: "Advance",
        },
        {
          id: 23,
          name: "MachineLearning",
          imageUrl:
            "https://upload.wikimedia.org/wikipedia/commons/d/d5/Hey_Machine_Learning_Logo.png?_=20180611150542",
          status: "Advance",
        },
        {
          id: 24,
          name: "Java",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Java.svg",
          status: "Advance",
        },
        {
          id: 25,
          name: "Flutter",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Flutter.svg",
          status: "Advance",
        },
        {
          id: 25,
          name: "GraphQL",
          imageUrl: "https://icon.icepanel.io/Technology/svg/GraphQL.svg",
          status: "Advance",
        },
        {
          id: 26,
          name: "Electron",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Electron.svg",
          status: "Advance",
        },
        {
          id: 27,
          name: "Go",
          imageUrl: "https://go.dev/images/go-logo-white.svg",
          status: "Advance",
        },
        {
          id: 28,
          name: "Spring",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Spring.svg",
          status: "Advance",
        },
        {
          id: 29,
          name: "Keras",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Keras.svg",
          status: "Advance",
        },
        {
          id: 30,
          name: "Django",
          imageUrl:
            "https://icon.icepanel.io/Technology/png-shadow-512/Django.png",
          status: "Advance",
        },
        {
          id: 31,
          name: "Flask",
          imageUrl:
            "https://icon.icepanel.io/Technology/png-shadow-512/Flask.png",
          status: "Advance",
        },
        {
          id: 32,
          name: "FastAPI",
          imageUrl: "https://icon.icepanel.io/Technology/svg/FastAPI.svg",
          status: "Advance",
        },
        {
          id: 33,
          name: "Nest.js",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Nest.js.svg",
          status: "Advance",
        },
        {
          id: 34,
          name: "TypeScript",
          imageUrl: "https://icon.icepanel.io/Technology/svg/TypeScript.svg",
          status: "Advance",
        },
      ],
      tools: [
        {
          id: 1,
          name: "Git",
          imageUrl:
            "https://git-scm.com/images/logos/downloads/Git-Icon-1788C.png",
          status: "Version Control",
        },
        {
          id: 2,
          name: "GitHub",
          imageUrl: "https://cdn-icons-png.flaticon.com/512/25/25231.png",
          status: "Git Hosting",
        },
        {
          id: 3,
          name: "NPM",
          imageUrl:
            "https://cdn.iconscout.com/icon/free/png-256/free-npm-3-1175132.png",
          status: "Package Manager",
        },
        {
          id: 4,
          name: "MySQL",
          imageUrl: "https://cdn-icons-png.flaticon.com/512/5968/5968313.png",
          status: "Database",
        },
        {
          id: 5,
          name: "MongoDB",
          imageUrl: "https://icon.icepanel.io/Technology/svg/MongoDB.svg",
          status: "Advance",
        },
        {
          id: 6,
          name: "Firebase",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Firebase.svg",
          status: "Advance",
        },
        {
          id: 7,
          name: "Jenkins",
          imageUrl: "https://icon.icepanel.io/Technology/svg/TypeScript.svg",
          status: "Advance",
        },
        {
          id: 8,
          name: "AWS",
          imageUrl:
            "https://icon.icepanel.io/Technology/png-shadow-512/AWS.png",
          status: "Advance",
        },
        {
          id: 9,
          name: "Azure",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Azure.svg",
          status: "Intermediate",
        },
        {
          id: 10,
          name: "GoogleCloud",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Google-Cloud.svg",
          status: "Advance",
        },
        {
          id: 11,
          name: "BitBucket",
          imageUrl: "https://icon.icepanel.io/Technology/svg/BitBucket.svg",
          status: "Advance",
        },
        {
          id: 12,
          name: "DegitalOcean",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Digital-Ocean.svg",
          status: "Advance",
        },
        {
          id: 13,
          name: "Docker",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Docker.svg",
          status: "Advance",
        },
        {
          id: 14,
          name: "PostgreSQL",
          imageUrl: "https://icon.icepanel.io/Technology/svg/PostgresSQL.svg",
          status: "Advance",
        },
        {
          id: 15,
          name: "Postman",
          imageUrl: "https://icon.icepanel.io/Technology/svg/Postman.svg",
          status: "Advance",
        },
      ],
    };
  },
};
</script>
<template>
  <div
    class="bg-[#1e1e1f] px-5 py-5 md:px-12 md:py-10 text-left border border-[#383838] rounded-3xl text-amber-50 mx-3 mb-5"
  >
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center"
        >
          About Me &nbsp;
          <div
            class="h-[1px] w-32 bg-amber-200 md:w-96 aos-init aos-animate"
            data-aos="zoom-in-left"
            data-aos-duration="600"
          ></div>
        </div>
      </header>

      <section
        class="text-sm md:text-lg text-justify flex flex-col gap-4 md:flex-row md:gap-8 md:justify-left md:items-center"
      >
        <div class="flex justify-center">
          <img
            class="w-9/12 rounded-full mb-3 fadein-up"
            src="https://i1.sndcdn.com/avatars-000214125831-5q6tdw-t500x500.jpg"
            alt="Foto"
          />
        </div>
        <div class="md:w-7/12">
          <p class="mb-3 md:mb-7 fadein-left fadeins-1">
            Hello everyone! <br />
            I am Akira Uchiyama. <br />
            I am a Full-Stack and AI/ML Engineer with 10+ years of experience
            designing and building scalable, cloud-native software solutions, as
            well as developing state-of-the-art LLM, Generative AI, and NLP
            systems. &nbsp; <br />I have a proven track record of collaborating
            with cross-functional teams to deliver production-grade
            applications, including microservices architectures, CI/CD
            pipelines, and real-time data platforms using technologies such as
            Django, React, Kubernetes, and Terraform. &nbsp; <br />
            My expertise includes integrating RAG architectures, LangChain,
            Hugging Face, GPT-3.5/4, and reinforcement learning techniques to
            optimize system performance, reduce operational costs, and enhance
            end-user experiences. &nbsp; <br />I am passionate about building
            end-to-end AI platforms that combine modern web technologies, deep
            learning, and robust DevOps practices to create impactful solutions
            for both startups and enterprise environments.
          </p>
        </div>
      </section>
    </article>
  </div>

  <div class="px-5 py-5 md:px-12 md:py-10 text-left text-amber-50 mx-3">
    <article data-page="about">
      <header>
        <div
          class="text-2xl font-bold text-white mb-5 fadein-bot title-section flex items-center"
        >
          <div
            class="h-[1px] w-10 bg-amber-200 md:w-20 aos-init aos-animate"
            data-aos="zoom-in-left"
            data-aos-duration="600"
          ></div>
          &nbsp; Skills
        </div>
      </header>
      <section>
        <div>
          <ul
            class="flex flex-wrap text-sm font-medium text-center text-gray-500 dark:text-gray-400 mb-5"
          >
            <li class="mr-2">
              <button
                class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{
                  'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 1,
                }"
                @click="activeTab = 1"
              >
                Tech Stack
              </button>
            </li>
            <li class="mr-2">
              <button
                class="inline-block px-4 py-3 rounded-lg hover:text-white"
                :class="{
                  'text-amber-200 bg-amber-200 bg-opacity-10': activeTab === 2,
                }"
                @click="activeTab = 2"
              >
                Tools
              </button>
            </li>
          </ul>
        </div>
        <div v-show="activeTab === 1">
          <div
            class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12"
          >
            <div v-for="item in tech" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3"
              >
                <div
                  class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in"
                >
                  <img
                    alt="HTML"
                    loading="lazy"
                    width="32"
                    height="32"
                    decoding="async"
                    data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]"
                    :src="item.imageUrl"
                    style="color: transparent"
                  />
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div
                    class="tech font-medium text-secondary transition-all duration-300 translate-y-0"
                  >
                    {{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm"
                  >
                    {{ item.status }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
        <div v-show="activeTab === 2">
          <div
            class="grid grid-cols-2 gap-4 pb-32 md:grid-cols-3 md:gap-8 xl:grid-cols-4 xl:gap-10 2xl:gap-12"
          >
            <div v-for="item in tools" :key="item.id">
              <div
                class="item-tech flex cursor-pointer items-center gap-2 rounded border border-amber-200 px-2 py-2 hover:bg-amber-200 hover:bg-opacity-10 md:gap-3 lg:px-3"
              >
                <div
                  class="flex h-12 w-12 items-center justify-center p-0 lg:h-16 lg:w-16 lg:p-2 zoom-in"
                >
                  <img
                    alt="HTML"
                    loading="lazy"
                    width="32"
                    height="32"
                    decoding="async"
                    data-nimg="1"
                    class="img-tech drop-shadow-xl transition-all duration-300 h-[65%] w-[65%] lg:h-[85%] lg:w-[85%]"
                    :src="item.imageUrl"
                    style="color: transparent"
                  />
                </div>
                <div class="flex items-center text-sm md:text-base lg:text-lg">
                  <div
                    class="tech font-medium text-secondary transition-all duration-300 translate-y-0"
                  >
                    {{ item.name }}
                  </div>
                  <div
                    class="status-tech opacity-0 absolute mt-5 text-[10px] text-amber-200 transition-all duration-300 md:text-xs lg:text-sm"
                  >
                    {{ item.status }}
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </section>
    </article>
  </div>
</template>

<style>
.fadein-left {
  opacity: 0;
  animation: fadeInLeft 0.5s ease-out forwards;
}

@keyframes fadeInLeft {
  0% {
    opacity: 0;
    transform: translateX(100%);
  }

  100% {
    opacity: 1;
    transform: translateX(0);
  }
}

.fadeins-1 {
  animation-delay: 500ms;
}

.fadeins-2 {
  animation-delay: 800ms;
}

.img-tech,
.tech {
  transition: transform 0.3s ease;
}

.item-tech:hover .img-tech {
  transform: scale(1.3);
}

.item-tech:hover .tech {
  transform: translateY(-12px);
}

.item-tech:hover .status-tech {
  opacity: 1;
}
</style>
