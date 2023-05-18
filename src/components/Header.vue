<template>
  <div class="headerContainer">
    <div class="headerContent">
      <h1>Welcome to my Portofolio</h1>
      <p>This website is dedicated to showcase projects that i've worked on.</p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style scoped>
.headerContainer {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 90vh;
  color: black;
  margin: 0;
  width: 100%;
}

.headerContent {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border-radius: 50%;
  box-shadow: rgba(178, 164, 255, 0.2) 0px 45px 110px 0px;
  width: 3000px;
  height: 1000px;
  overflow: hidden;
  padding: 100px 100px;
}

h1 {
  color: #b2a4ff;
}

@media screen and (max-width: 900px) {
  .headerContainer {
    padding: clamp(10px, 16px, 20px);
  }
}
</style>
