<template>
  <div>
    <section>
      <img class="hero" src="@/assets/hero-croc.jpg" alt="" />
      <div class="hero hero-overlay"></div>

      <div class="container">
        <div class="inner-container">
          <h1>Job4Croc</h1>
          <h2>Are you a croc looking for a job?</h2>
          <p class="sub">
            Are you tired of sitting on your scaly ass all the damn time?!
            <br />
            Well, look no further we have all the jobs that you can swing your
            disgusting tail at!
          </p>
          <GlitchButton @click="findJob" text="Start searching now!" />
        </div>
      </div>
    </section>
    <!-- <section>
      So croc we got it ON LOCK! We aint using TikTok cause we are employed and
      croc. Unblock the porn sites plz :(
    </section> -->
  </div>
</template>

<script>
import GlitchButton from "@/components/GlitchButton.vue";

export default {
  name: "HomeView",
  components: {
    GlitchButton,
  },
  methods: {
    findJob() {
      alert("JOB NOT FOUND");
    },
  },
};
</script>

<style lang="scss" scoped>
h1,
h2,
h3,
p {
  color: black;
}

section {
  padding-top: 100px;
  position: relative;
  overflow: hidden;
  min-height: 100vh;
}
.hero {
  position: absolute;
  top: -60px;
  left: 0;
  width: 100%;
  z-index: -1;

  &.hero-overlay {
    top: 0;
    height: 100%;
    background-color: #fff;
    opacity: 0.3;
    z-index: -1;
  }
}

.container {
  display: flex;
  align-items: center;
  flex-direction: column;
}

.inner-container {
}

h1 {
  font-size: 80px;
  margin-bottom: 10px;
}

h2 {
  font-size: 40px;
  margin-top: 10px;
}

.sub {
  font-size: 24px;
}

.glitch-button {
  margin: auto;
}
</style>
