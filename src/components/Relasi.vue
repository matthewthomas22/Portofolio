<template>
  <div class="contentContainer">
    <div class="contentLeft">
      <img
        src="../assets/ScreenshotRelasi.png"
        alt="screenshot website Relasi"
        @click="redirect"
      />
    </div>
    <div class="contentRight">
      <h2>Relasi Apps</h2>
      <p>
        Relasi adalah sebuah ide project website yang dikemukakan oleh Teach For
        Indonesia. Website ini berguna untuk menyediakan pelatihan bagi UMKM
        yang ingin belajar untuk mengembangkan usahanya.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "Relasi",
  methods: {
    redirect() {
      window.location.href = "https://shimmering-youtiao-3be9f2.netlify.app/";
    },
  },
};
</script>

<style scoped>
@keyframes hoverAnimation {
  0% {
    transform: translateY(5px);
  }
  100% {
    transform: translateY(-5px);
  }
}

.contentContainer {
  display: flex;
  justify-content: center;
  height: clamp(10rem, 30vh + 1rem, 20rem);
  align-items: center;
  padding: clamp(100px, 160px, 200px);
  transition: 0.3s;
}

.contentLeft {
  object-fit: contain;
  width: fit-content;
}

.contentLeft img {
  object-fit: contain;
  cursor: pointer;
  width: clamp(20rem, 40vw, 30rem);
  border-radius: 16px;
  animation: hoverAnimation 1s infinite alternate;
  animation-play-state: paused;
}

.contentLeft img:hover {
  animation-play-state: running;
}

.contentRight {
  display: flex;
  flex-direction: column;
  text-align: left;
  padding: 0 0 0 24px;
}

.contentRight p {
  margin-top: 0;
  font-size: clamp(12px, 14px, 18px);
  line-height: 30px;
}

.contentRight h2 {
  color: #b2a4ff;
  margin-bottom: 10px;
}

@media screen and (max-width: 900px) {
  .contentContainer {
    flex-direction: column;
  }
  .contentRight {
    width: min(20rem, 30rem);
    padding: 0;
  }
}
</style>
