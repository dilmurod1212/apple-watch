<script>
import Header from "./Components/Header.vue";
import Showcase from "./Components/Showcase.vue";
import Cards from "./Components/Cards.vue";
export default {
  data() {
    return {
      card: [
        {
          title: "Know your runs. In and out.",
          descr:
            "Train smarter with more in-run stats. Want to compare a run to your last five? Just swipe left. Mark splits by selecting pause or using gestures, like tapping the screen or double-clicking the side button. And get a full post-run report, including elevation.",
        },
        {
          title: "Run in good spirits.",
          descr:
            "A little support can go a long way. You can receive encouraging emoji from friends. And reminders triggered by your friends’ shared activity, the current weather, or your own history give you every reason to run.",
        },
        {
          title: "Just do it. Sunday.",
          descr:
            "Run every Sunday and see how long you can keep your streak alive. Fuel your run with exclusive Nike+ Run Club playlists on Apple Music.",
        },
      ],
    };
  },
  components: {
    Header,
    Showcase,
    Cards,
  },
};
</script>

<template>
  <div>
    <Header />

    <main>
      <Showcase />
      <Cards v-bind:card="card" />
    </main>
  </div>
</template>

<style scoped></style>
