<template>
  <div class="home">

    <Nav :activeNav="current"/>

    <div class="section" id="edgeryders" >
      <Edgeryders />
    </div>

    <div class="section" id="current" >
      <Current
        v-if="calls"
        :events="events"
        :conversations="stories"
        :calls="calls"
      />
    </div>

    <div class="section" id="people" >
      <Participants :data="participants" :users="users" />
    </div>

    <div class="section" id="connect" >
      <People :data="stories" />
    </div>

    <div class="section" id="mission" >
      <About />
    </div>

    <div class="section" id="projects" >
      <Projects :data="categories" />
    </div>

    <div class="section" id="press" >
      <Press :data="press" />
    </div>

    <div class="section" id="social" >
      <Social />
    </div>

    <div class="section" id="terms">
      <Terms />
    </div>

  </div>
</template>

<script>
import Nav from "@/components/Navigation.vue";
import Current from "@/components/Current.vue";
import Participants from "@/components/Participants.vue";
import Events from "@/components/Events.vue";
import Projects from "@/components/Projects.vue";
import Press from "@/components/Press.vue";
import About from "@/components/About.vue";
import People from "@/components/People.vue";
import Edgeryders from "@/components/Edgeryders.vue";
import Social from "@/components/Social.vue";
import Terms from "@/components/Terms.vue";

import axios from "axios";
import moment from "moment";

export default {
  name: "home",
  data() {
    return {
      current: 'welcome',
      stories: null,
      events: null,
      conversations: null,
      participants: null,
      categories: null,
      calls: null,
      users: null,
      topics: null,
    };
  },
  components: {
    Nav,
    Current,
    Participants,
    Events,
    Projects,
    Press,
    About,
    People,
    Edgeryders,
    Social,
    Terms
  },
  created() {
    this.getData();
  },
  methods: {
    setActive(waypoint) {
      alert(waypoint)
    },
    getData() {
      axios
        .get("https://edgeryders.herokuapp.com/festival")
        .then(({ data }) => {
          this.participants = data.participants;
          this.events = data.events;
          this.conversations = data.conversations;
          this.stories = data.stories;
          this.categories = data.categories;
          this.users = data.latest_users;
          this.topics = data.latest_topics;
          this.calls = data.calls;
        })
        .catch();
    }
  }
};
</script>
<style lang="scss">
.section {
  background: #efefef;
  width: 100%;
  width: 100vw;
  overflow: hidden;
  &#hero {
    position: relative;
    margin-top: 55px;
    padding-top: 0;
  }
  &#current {
    position: relative;
    padding-top: 40px;
  }
  &#people {
    position: relative;
    margin-top: 1px;
    background: #fff;
  }
  &#events {
    padding-top: 50px;
    background: #fafafa;
  }
  &#process {
    padding-top: 40px;
    padding-bottom: 60px;
    background: #efefef;
  }
  &#mission {
    padding-top: 40px;
    padding-bottom: 20px;
    background: #efefef;
  }
  &#press {
    background: #fff;
    padding: 0px 0 100px !important;
  }
  &#connect {
    padding-top: 40px;
    padding-bottom: 60px;
    background: #fafafa;
  }
  &#edgeryders {
    padding-top: 50px;
    padding-bottom: 0px;
  }
  &#projects {
    background: #fafafa;
    padding: 0px 0 60px;
  }
}

@media (max-width: 640px) {
  .section {
    &#press {
      background: #efefef;
      padding: 0px !important;
    }
    &#current {
    position: relative;
    padding-top: 30px;
    }
    &#process {
      padding-bottom: 20px;
    }
    &#mission {
      padding-bottom: 0px;
      padding-top: 0px;
    }
    &#connect {
      padding-top: 0px;
      padding-bottom: 0px;
    }
    &#edgeryders {
      padding-top: 40px;
      padding-bottom: 0px;
    }
  }
}
</style>
