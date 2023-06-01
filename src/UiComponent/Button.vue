<template>
  <div>
    <button><slot></slot></button>
  </div>
</template>
<script>
export default {};
</script>
<style>
button {
  padding: 10px 18px;
  background-color: #ea625c;
  border-radius: 4px;
  border: 1px solid #ea625c;
  color: #fff;
  text-transform: uppercase;
  font-weight: 500;
  cursor: pointer;
}
button:hover {
  transition: 0.3s ease;
  background-color: transparent;
  color: #ea625c;
}
</style>
