<template>
  <div>
    <section>
      <div class="container">
        <div class="cards">
          <div class="card" v-for="card in card">
            <h3>{{ card.title }}</h3>
            <p>
              {{ card.descr }}
            </p>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>
<script>
export default {
  props: {
    card: {
      type: Array,
      required: true,
    },
  },
};
</script>
<style lang="scss">
.cards {
  display: flex;
  justify-content: space-between;
  margin: 2rem 0;
  gap: 50px;
  flex-wrap: wrap;
  .card {
    flex: 1;
    h3 {
      font-size: 24px;
      margin-bottom: 10px;
    }
    p {
      font-size: 14px;
      letter-spacing: 1px;
      line-height: 2;
    }
  }
}

@media (max-width: 768px) {
  .cards {
    flex-direction: column;
    .card {
      h3 {
        font-size: 18px;
      }
      p {
        font-size: 10px;
      }
    }
  }
}
</style>
