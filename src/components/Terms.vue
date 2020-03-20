<template>
  <div class="w-full md:flex bg-black p-6 md:p-10 text-left">
    <div class="md:w-3/4 md:px-4 md:pr-20">
      <h1 class="text-white font-bold">TERMS OF PARTICIPATION & PRIVACY POLICY</h1>
      <p class="text-white mt-2">The Edgeryders online platform and activities are intended for people to cooperate within and across projects trying to build a better world. The word "better" has here a fairly broad range of meaning. These <a class="underline" href='https://edgeryders.eu/t/netiquette/45' target='_blank'>Community Guidelines</a> are here to help you understand what it means to be a member of Edgeryders. Don’t forget that your use of Edgeryders is subject to these Community Guidelines and our <a class="underline" href='https://edgeryders.eu/t/id/44' targert='_blank'>Terms of Service</a>.</p>
    </div>

    <div class="md:w-1/4 pt-4 md:p-6 md:px-10 border-gray-100 md:border-l">
      <h1 class="text-white font-bold">Contact Us</h1>
      <p class="text-white mt-2">
        <a class="underline" href='mailto:contact@edgeryders.eu' target="_blank">Email</a><br />
        <a class="underline" href='https://twitter.com/edgeryders' target="_blank">Twitter</a><br />
        <a class="underline" href='https://facebook.com/edgeryders' target="_blank">Facebook</a>

      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {};
  },
  components: {},
  props: ["data"],
  mounted: function() {}
};
</script>

<style type="text/css" lang="scss">
@import url('https://fonts.googleapis.com/css?family=Permanent+Marker&display=swap');
.social {
  width: 5rem;
  height: 5rem;
  border-radius: 10px;
  background-color: #ddd;
  margin-right: 1rem;
  background-position: center center !important;
  background-repeat: no-repeat !important;
 &:hover {
 background-color: rgba(0,0,0,0.14);
} 
}

.twitter {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Cpath fill='%231DA1F2' d='M459 152l1 13c0 139-106 299-299 299-59 0-115-17-161-47a217 217 0 0 0 156-44c-47-1-85-31-98-72l19 1c10 0 19-1 28-3-48-10-84-52-84-103v-2c14 8 30 13 47 14A105 105 0 0 1 36 67c51 64 129 106 216 110-2-8-2-16-2-24a105 105 0 0 1 181-72c24-4 47-13 67-25-8 24-25 45-46 58 21-3 41-8 60-17-14 21-32 40-53 55z'/%3E%3C/svg%3E");
  background-size: 40%;
}
.facebook {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 320 512'%3E%3Cpath fill='%234267B2' d='M279 288l14-93h-89v-60c0-25 13-50 53-50h40V6s-37-6-72-6c-73 0-121 44-121 125v70H23v93h81v224h100V288z'/%3E%3C/svg%3E");
  background-size: 20%;
}
.email {
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 512 512'%3E%3Cpath fill='rgba(0,0,0,0.7)' d='M502 191c4-3 10 0 10 5v204c0 27-21 48-48 48H48c-26 0-48-21-48-48V196c0-5 6-8 10-5l154 114c21 15 56 47 92 47s72-33 92-47l154-114zM256 320c23 0 57-29 73-41 133-97 143-105 174-129 6-5 9-12 9-19v-19c0-26-22-48-48-48H48C22 64 0 86 0 112v19c0 7 3 14 9 19 31 24 41 32 174 129 16 12 50 41 73 41z'/%3E%3C/svg%3E");
  background-size: 35%;
}
.arrow {
  background-image: url("data:image/svg+xml, %3Csvg xmlns='http://www.w3.org/2000/svg' width='367.3' height='367.3'%3E%3Cpath fill='rgba(0,0,0,0.2)' d='M337.6 1A473.5 473.5 0 0 0 298.4 21c-11.6 6.1-25.7 12.3-35.5 21.4-5.5 5 0 15.3 7.4 12.9 0 0 .6 0 .6-.6 1.8 1.2 3 2.4 4.9 4.3 0 .6.6 1.8.6 2.4.6 1.2 1.8 2.5 3 3.7-17.7 33-34.2 66-55 96.7a166.4 166.4 0 0 1-20.8 25.7c-19.6-31.2-51.4-67.3-90-60.6-50.8 9.2-23.3 63.7 3 82 31.3 22.7 58.2 21.4 85.1 0 12.3 20.8 20.8 44 19.6 66.7-1.8 54.5-50.8 63.7-91.8 49.6 6.1-16 8-34.3 4.3-50.2-6.1-28.8-50.2-54.5-75.9-34.3-25 20.2 22 71.6 37.3 82 4.3 3.1 9.2 6.2 14.1 8.6-.6.6-.6 1.2-1.2 1.8-28.2 44.1-65.5 6.2-82.6-25-2.5-5-9.2-.7-7.4 4.2C32.2 345 61 382.8 99.5 360.8a63.5 63.5 0 0 0 22.7-23.3c33.6 13.5 72.8 13.5 97.3-17.1 29.4-36.7 11-84.5-8.6-120l1.2-1.2c35-33.6 56.3-81.4 78.4-124.2 4.3 3 9.1 6.1 13.4 9.2 3 1.8 7.4 1.2 9.8-1.3a150.2 150.2 0 0 0 35.5-73.4c1.9-6.7-4.9-11.6-11.6-8.6zM178.5 207.7c-23.3 13.5-46.5-3-63.7-19-22.6-20.8-16.5-54.5 18.4-47.7 17.7 3.7 31.8 19.6 43.4 32.4 6.2 6.7 12.3 14.7 17.8 23.3-5 4.3-10.4 8-16 11zM116 319.2s-.6 0 0 0A99.5 99.5 0 0 1 67.7 261c-6.1-20.8 27-10.4 35.5-6 23.3 12.8 21.4 42.1 12.8 64.2zM306.4 67c-.6 0-.6-.6-1.2-.6 0-1.8-1.3-3.7-3.7-4.9-4.3-1.8-8.6-4.3-12.9-6.7-1.8-1.2-5.5-5-5.5-3.7 0-.6-.6-1.2-1.2-1.2 6.7-3.7 13.5-8.6 20.2-12.2 8.6-5 17.7-9.8 27-14.7a131.3 131.3 0 0 1-22.7 44z'/%3E%3C/svg%3E%0A");
  background-size: cover;
  width: 120px;
  height: 120px;
  position: absolute;
  bottom: 0;
  left: -30px;
}
.er_photo {
  transform: rotate(-1.2deg);
  .photo {
  background: url('../assets/edgeryders_group.jpg') no-repeat center 15px #f7f8f8;
  background-size: 95%;
  height: 290px;
  padding-bottom: 80px;
  position: relative;
  border-radius: 10px;
  width: 90%;
  left: 5%;
  margin-top: 2%;
  &:before, &:after {
        z-index: -1;
        position: absolute;
        content: "";
        bottom: 15px;
        left: 10px;
        width: 50%;
        top: 80%;
        max-width: 300px;
        background: #777;
        box-shadow: 0 15px 10px #777;
        transform: rotate(-3deg);
      }
      &:after {
        transform: rotate(3deg);
        right: 10px;
        left: auto;
      }
      h3 {
        position: absolute;
        bottom: 6%;
        left: 0%;
        width: 100%;
        text-align: center;
        color: orangered;
        font-size: 1.1em;
        font-family: "Permanent Marker", cursive;
        }
}
}


.speech-bubble {
  position: relative;
  background: #fff;
  border-radius: 0.4em;
}

.speech-bubble:after {
  content: "";
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
