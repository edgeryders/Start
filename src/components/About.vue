<template>
  <div class="bg-white pt-8 md:pt-0 md:bg-gray-200">
    <h2 class="font-display text-4xl font-bold text-center md:text-5xl mt-0 md:ml-8 md:pr-0 mb-1 md:mt-0 md:pt-0 md:ml-0 leading-tight md:leading-normal font-medium w-full">The Mission</h2>
    <h3 class="font-body text-xl md:text-2xl">
      A dense network of co-created solutions to the big issues.
    </h3>

    <div class="w-full flex flex-col md:flex-row items-start justify-between">
      <div class="w-full font-body text-left md:text-left md:w-1/2 mt-4 px-6 md:pt-0 md:px-10 text-left md:leading-relaxed">
        <p class="text-lg md:text-xl border-t pt-4 md:border-none">
          Our theory of change is building dense networks around people trying
          to tackle messy socialecological, economic and political challenges.
          Having a dense network around you is one of the hallmarks of social
          capital, and gives you access to expertise, resources, skill sharing
          and financing. In a dense network, there are many ways for you to get
          from one point to another. A key challenge here is for people with
          aligned interests to find each other, and as a community we’re out to
          solve just that.
        </p>
      </div>
      <div
        class="w-full md:w-1/2 px-4 md:px-8 mt-6 md:mt-8 mb-8 md:pt-0 text-left text-xl border-l border-gray leading-normal"
      >
        <div class="w-full flex items-start">
          <Video
            sources="https://mirror.eu.oneandone.net/projects/media.ccc.de/events/camp2019/h264-sd/camp19-10204-eng-pol-Participatory_art_event_tools_co-creation_and_silk_road_networks_sd.mp4"
            poster="video_poster.jpeg"
            :skip-backward="-20"
            :skip-forward="55"
            :auto-play="false"
          >
          </Video>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
  import Video from "@/components/Video.vue";

  export default {
    components: {
      Video
    },
    props: ["data"]
  };
</script>

<style type="text/css" lang="scss">

 
</style>