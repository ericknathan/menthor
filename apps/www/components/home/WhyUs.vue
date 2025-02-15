<script setup lang="ts">
const stacks: { logo: string; name: string; link: string }[] = [
  {
    logo: "/logos/vue.svg",
    name: "Vue",
    link: "https://vuejs.org/",
  },
  {
    logo: "/logos/tailwind.svg",
    name: "Tailwind",
    link: "https://tailwindcss.com/",
  },
  {
    logo: "/logos/supabase.svg",
    name: "Supabase",
    link: "https://supabase.com/",
  },
  {
    logo: "/logos/vercel.svg",
    name: "Vercel",
    link: "https://vercel.com/",
  },
  {
    logo: "/logos/github.svg",
    name: "GitHub",
    link: "https://github.com/",
  },
  {
    logo: "/logos/playwright.svg",
    name: "Playwright",
    link: "https://playwright.dev/",
  },
  {
    logo: "/logos/nuxt.svg",
    name: "Nuxt",
    link: "https://nuxt.com/",
  },
  {
    logo: "/logos/turborepo.svg",
    name: "Turborepo",
    link: "https://turbo.build/repo",
  },
];
</script>

<template>
  <section id="why_us" class="my-20 md:my-32">
    <div class="container">
      <h2
        class="mx-auto mb-6 max-w-[664px] text-3xl font-bold md:text-center md:text-4xl"
      >
        Porque a menthor?
      </h2>
      <p
        class="mx-auto mb-10 max-w-[664px] text-zinc-700 md:text-center md:text-lg"
      >
        Nós acreditamos que todo tipo de ensino deve ser gratuito e queremos
        fornecer a melhor experiência de ensino para nossos alunos.
      </p>
      <div
        class="space-y-6 sm:grid sm:grid-cols-[repeat(auto-fill,_minmax(320px,_1fr))] sm:gap-6 sm:space-y-0"
      >
        <div>
          <div
            class="group mb-6 hidden overflow-hidden rounded-lg border border-solid border-zinc-200 px-8 pb-4 pt-10 text-3xl font-semibold md:block"
          >
            <h3>Gratuito para</h3>
            <div class="flex items-center" aria-hidden>
              <div
                class="animation-text-left !pause group-hover:!start flex min-w-full"
                v-for="i in 2"
                :key="i"
              >
                <p class="-translate-x-[300px] text-zinc-300">
                  eeeeeeeeeeeeeeeee<strong class="font-semibold text-zinc-900"
                    >sempre</strong
                  >eeeeeeeeeeeeeeeeeeeee
                </p>
              </div>
            </div>
            <div class="flex items-center" aria-hidden>
              <div
                class="animation-text-right !pause group-hover:!start flex min-w-full"
                v-for="i in 2"
                :key="i"
              >
                <p class="-translate-x-[300px] text-zinc-300">
                  eeeeeeeeeeeeeeeeeeeee<strong
                    class="font-semibold text-zinc-900"
                    >sempre</strong
                  >eeeeeeeeee
                </p>
              </div>
            </div>
            <div class="flex items-center" aria-hidden>
              <div
                class="animation-text-left !pause group-hover:!start flex min-w-full"
                v-for="i in 2"
                :key="i"
              >
                <p class="-translate-x-[300px] text-zinc-300">
                  eeeeeeeeeeeeeeeeeeeeeeee<strong
                    class="font-semibold text-zinc-900"
                    >sempre</strong
                  >eeeeeeeeeeeeee
                </p>
              </div>
            </div>
          </div>
          <div
            class="group min-h-[258px] overflow-hidden rounded-lg border border-solid border-zinc-200 px-8 pb-6 pt-10 text-3xl font-semibold"
          >
            <h3 class="mb-6">Tecnologias modernas</h3>
            <div class="-ml-8 mb-2 flex gap-2">
              <div
                class="group-hover:!pause animation-stacks-left flex min-w-full gap-2"
                v-for="i in 2"
                :key="i"
              >
                <nuxt-link
                  v-for="stack in stacks.slice(0, 4)"
                  :key="stack.link"
                  :to="stack.link"
                  target="_blank"
                  class="flex h-[40px] min-w-fit items-center gap-2 rounded-full border border-solid border-zinc-200 px-4 py-2 hover:border-blue-500"
                >
                  <nuxt-img
                    :src="stack.logo"
                    class="h-[16px] w-auto"
                    width="26"
                    height="16"
                    :alt="stack.name"
                  />
                  <span class="text-sm font-semibold">{{ stack.name }}</span>
                </nuxt-link>
              </div>
            </div>
            <div class="-ml-8 mb-2 flex gap-2">
              <div
                class="group-hover:!pause animation-stacks-right flex min-w-full gap-2"
                v-for="i in 2"
                :key="i"
              >
                <nuxt-link
                  v-for="stack in stacks.slice(4)"
                  :key="stack.link"
                  :to="stack.link"
                  target="_blank"
                  class="flex h-[40px] min-w-fit items-center gap-2 rounded-full border border-solid border-zinc-200 px-4 py-2 hover:border-blue-500"
                >
                  <nuxt-img
                    :src="stack.logo"
                    class="h-[16px] w-auto"
                    width="26"
                    height="16"
                    :alt="stack.name"
                  />
                  <span class="text-sm font-semibold">{{ stack.name }}</span>
                </nuxt-link>
              </div>
            </div>
          </div>
        </div>
        <div
          class="group relative h-full overflow-hidden rounded-lg border border-solid border-zinc-200 px-8 pb-6 pt-10 text-3xl font-semibold"
        >
          <div
            class="absolute -left-[34px] top-[94px] flex h-full w-full justify-center"
          >
            <div
              class="mask-radial h-full max-h-[651px] w-full max-w-[1314px] bg-pattern"
            ></div>
          </div>
          <div class="relative flex h-full flex-col">
            <h3 class="mb-9 w-full">Terminal integrado</h3>
            <div class="h-full min-w-[calc(100%_+_32px)] flex-1">
              <nuxt-img
                loading="lazy"
                src="/vectors/terminal.svg"
                alt="Menthor terminal"
                height="380"
                width="334"
                class="block h-full w-full rounded-l-lg border border-zinc-200 border-r-transparent object-cover object-left-top shadow-lg transition-all group-hover:-translate-y-2 group-hover:shadow-2xl"
              />
            </div>
          </div>
        </div>
        <div class="col-span-1 md:col-span-2 lg:col-span-1">
          <div
            class="relative mb-6 min-h-[258px] overflow-hidden rounded-lg border border-solid border-zinc-200 px-8 pb-6 pt-10 text-3xl font-semibold"
          >
            <nuxt-img
              loading="lazy"
              src="/vectors/world_map.svg"
              height="264"
              alt="Menthor mapa mundial"
              width="810"
              class="absolute -top-[8px] left-[62px] h-[264px] w-[810px]"
            />
            <h3 class="relative mb-6">Networking com todo o Brasil</h3>
          </div>
          <div
            class="relative hidden min-h-[200px] overflow-hidden rounded-lg border border-solid border-zinc-200 py-6 px-8 text-3xl font-semibold lg:flex items-end text-right"
          >
            <div class="absolute top-0 left-0 w-full h-[99px]">
              <nuxt-img
                loading="lazy"
                src="/vectors/courses.svg"
                alt="Lista de cursos da plataforma menthor.io"
                width="354"
                height="99"
                class="w-full h-full object-cover object-center"
              />
            </div>
            <h3 class="block text-3xl font-semibold">
              Cursos escritos por devs experientes
            </h3>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
#why_us {
  --gap: 0.5rem;
  --duration: 30s;
  --scroll-start: 0;
  --scroll-end: calc(-100%);
}

.animation-text-left {
  flex-shrink: 0;
  min-width: 100%;
  animation: scroll-left var(--duration) linear infinite;
}

.animation-stacks-left {
  --duration: 20s;
  --scroll-end: calc(-100% - var(--gap));
  flex-shrink: 0;
  min-width: 100%;
  animation: scroll-left var(--duration) linear infinite;
}

.animation-text-right {
  flex-shrink: 0;
  min-width: 100%;
  animation: scroll-right var(--duration) linear infinite;
}

.animation-stacks-right {
  --duration: 20s;
  --scroll-end: calc(-100% - var(--gap));
  flex-shrink: 0;
  min-width: 100%;
  animation: scroll-right var(--duration) linear infinite;
}

@keyframes scroll-left {
  from {
    transform: translateX(var(--scroll-start));
  }
  to {
    transform: translateX(var(--scroll-end));
  }
}

@keyframes scroll-right {
  from {
    transform: translateX(var(--scroll-end));
  }
  to {
    transform: translateX(var(--scroll-start));
  }
}

@media (prefers-reduced-motion: reduce) {
  .animation-text-left {
    animation-play-state: paused;
  }
  .animation-stacks-left {
    animation-play-state: paused;
  }
  .animation-text-right {
    animation-play-state: paused;
  }
  .animation-stacks-right {
    animation-play-state: paused;
  }
}
</style>
