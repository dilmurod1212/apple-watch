<template>
  <div>
    <section id="showcase">
      <div class="container">
        <div class="content">
          <div class="info">
            <h1>Freedom calls.</h1>
            <p>
              Answer a call from your surfboard. Ask Siri to send a message.
              Stream your favorite songs on your run. And do it all while
              leaving your phone behind. Introducing Apple Watch Series 3 with
              cellular. Now you have the freedom to go with just your watch.
            </p>
            <Button>Watch the keynote</Button>
          </div>
          <div class="watch">
            <img src="@/images/intro-bg.png" alt="" />
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
import Button from "../UiComponent/Button.vue";
export default {
  components: {
    Button,
  },
};
</script>
<style lang="scss">
.content {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 1rem;
  .info {
    // flex: 2;
    display: flex;
    flex-direction: column;
    gap: 2rem;
    h1 {
      font-size: 36px;
      font-weight: 700;
    }
    p {
      padding: 0 20px;
      border-left: 2px solid #888888;
      width: 60%;
      line-height: 2;
    }
    .watch {
      flex: 1;
    }
  }
}

@media (max-width: 768px) {
  .content {
    flex-direction: column;
    gap: 50px;
    margin-top: 40px;
    .info {
      p {
        width: 100%;
        font-size: 14px;
      }
    }
  }
}
</style>
