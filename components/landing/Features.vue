<script setup>
const features = [
  {
    title: "Bring Your Own Framework",
    description:
      "Flexibility to construct your own framework tailored to your unique project needs, we provide customizable tools and resources to facilitate seamless development and innovation",
    icon: "bx:bxs-briefcase",
  },
  {
    title: "100% Static HTML, No JS",
    description:
      "ROATA renders your entire page to static HTML, removing all JavaScript from your final build by default.",
    icon: "bx:bxs-window-alt",
  },
  {
    title: "On-Demand Components",
    description:
      "Streamlining your design process with on-demand components, we offer a diverse library of customizable elements ready to integrate seamlessly into your project, ensuring efficiency and adaptability.",
    icon: "bx:bxs-data",
  },
  {
    title: "Broad Integration",
    description:
      "ROATA supports TypeScript, Scoped CSS, CSS Modules, Sass, Tailwind, Markdown, MDX, and any other npm packages.",
    icon: "bx:bxs-bot",
  },
  {
    title: "SEO Enabled",
    description:
      "Automatic sitemaps, RSS feeds, pagination and collections take the pain out of SEO and syndication. It just works!",
    icon: "bx:bxs-file-find",
  },
  {
    title: "Community",
    description:
      "Fostering a vibrant and collaborative community, we provide a platform for UX designers to connect, share insights, and collectively elevate their craft through knowledge exchange and support.",
    icon: "bx:bxs-user",
  },
];
</script>

<template>
  <div class="mt-16 md:mt-0">
    <h2 class="text-4xl lg:text-5xl font-bold lg:tracking-tight">
      Catering to your users needs
    </h2>
    <p class="text-lg mt-4 text-slate-600">
      We specialize in crafting Seamless User Experiences: Empowering Digital Interactions with UX Design Expertise
    </p>
  </div>

  <div class="grid sm:grid-cols-2 md:grid-cols-3 mt-16 gap-16">
    <div v-for="item of features" class="flex gap-4 items-start">
      <div class="mt-1 bg-black rounded-full p-2 w-8 h-8 shrink-0">
        <Icon class="text-white" :name="item.icon" />
      </div>
      <div>
        <h3 class="font-semibold text-lg">{{ item.title }}</h3>
        <p class="text-slate-500 mt-2 leading-relaxed">
          {{ item.description }}
        </p>
      </div>
    </div>
  </div>
</template>
