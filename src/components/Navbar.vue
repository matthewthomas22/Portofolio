<template>
  <nav>
    <div class="navTitle">
      <h3>Matthew Thomas</h3>
    </div>
    <div class="navButtons">
      <p>About Me</p>
      <p>Skills</p>
    </div>
  </nav>
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
nav {
  display: flex;
  justify-content: space-between;
  margin: 0 80px 0 80px;
  padding: 16px 0;
}
.navButtons {
  display: flex;
  align-items: center;
  justify-content: space-evenly;
}

p {
  padding-right: 40px;
  transition: 0.5s ease-in-out;
  cursor: pointer;
}

p:hover {
  font-size: 18px;
  /* font-weight: bold; */
  color: #b2a4ff;
}

@media screen and (max-width: 552px) {
  nav {
    margin: 0 20px 0 20px;
  }
  p {
    padding-right: 10px;
  }
}
</style>
