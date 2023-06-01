<template>
  <div>
    <header class="container">
      <a href="#"><img src="../images/Vector.svg" alt="logo" /></a>
      <ul>
        <li><a href="#">Home</a></li>
        <li><a href="#">About</a></li>
        <li><a href="#">Offers</a></li>
        <li><a href="#">Services</a></li>
        <li><a href="#">How can we help you?</a></li>
      </ul>
      <i class="fas fa-bars"></i>
    </header>
  </div>
</template>
<script>
export default {};
</script>
<style lang="scss" scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 70px;
  img {
    width: 30px;
  }
  img:hover {
    transition: 0.3s;
    position: relative;
    bottom: 5px;
  }
  ul {
    display: flex;
    gap: 40px;
    li a {
      color: #000;
      padding: 8px 0;
      border-bottom: 2px solid transparent;
      transition: 0.3s;
    }
    li a:hover {
      border-bottom: 2px solid #000;
    }
  }
  i {
    display: none;
  }
  @media (max-width: 768px) {
    header {
      margin-bottom: 40px;
    }
    ul {
      display: none;
    }
    i {
      display: block;
    }
  }
}
</style>
