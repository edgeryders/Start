<template>
  <div class="self-start flex items-center w-full w-auto h-12 overflow-hidden author">
    <div class="w-12 h-12 md:h-12 bg-cover shadow-lg" :style="{ backgroundImage: 'url(' + avatar + ')' }"></div>
    <a class="ml-3 mt-1 mr-2 font-bold text-white" :href="'https://edgeryders.eu/u/' + username" target="_blank">{{text}} @{{username}}</a>
  </div>
</template>

<script>

export default {
  data() {
    return {
      username: null,
      avatar: null
    }
  },
  components: {
  },
  props: ["data", "text", "userid"],
  mounted: function() {
      this.username = this.data.username;
      this.avatar = this.data.avatar;
  }
};
</script>

<style type="text/css" lang="scss">
  .author {
  background: rgba(0,0,0,0.8) !important;


}
.speech-bubble {
  position: relative;
  background: #fff;
  border-radius: .4em;
}

.speech-bubble:after {
  content: '';
  position: absolute;
  left: 0;
  top: 50%;
  width: 0;
  height: 0;
  border: 20px solid transparent;
  border-right-color: #fff;
  border-left: 0;
  border-top: 0;
  margin-top: -10px;
  margin-left: -20px;

}

</style>
