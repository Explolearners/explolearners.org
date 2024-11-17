<template>
  <div class="topMostDiv w-full h-screen bg-gray-100 flex flex-col items-center justify-center p-4 relative overflow-hidden"
       ref="topMostDiv">
    <img src="../src/assets/flowers_decor_uptodown.png"
         alt="Top right flower"
         class="absolute top-0 right-0 w-72 md:w-96 z-0">

    <img src="../src/assets/dandelions_purple_transparents.png"
         alt="Bottom left flower"
         class="absolute bottom-0 left-0 w-full md:w-[30rem] z-0">

    <div class="text-center z-10 space-y-4 p-2">
      <h1
          class="font-satisfy text-6xl md:text-8xl leading-tight bg-gradient-to-r from-[#9370DB] via-[#8B6FC9] to-[#6d53fd] text-transparent bg-clip-text p-2">
        Explolearners
      </h1>
      <p
         class="font-satisfy text-2xl md:text-3xl bg-gradient-to-r from-[#8B6FC9] via-[#7B68EE] to-[#9370DB] text-transparent bg-clip-text">
        A World for Curiosity to Flourish
      </p>
    </div>
  </div>
</template>

<script setup>
import { onMounted, ref } from 'vue';

const topMostDiv = ref(null);

onMounted(() => {
  console.log(topMostDiv.value);
});
</script>

<style>
.font-satisfy {
  font-family: 'Satisfy', cursive;
}

.topMostDiv {
  animation: boxShadowGlow;
  animation-duration: 10s;
  animation-timing-function: linear;
  animation-iteration-count: infinite;
}

@keyframes boxShadowGlow {

  0% {
    box-shadow: inset .5rem .5rem 2rem #7B68EE;

  }

  50% {
    box-shadow: inset .5rem .5rem 4rem #7B68EE;

  }

  100% {
    box-shadow: inset .5rem .5rem 2rem #7B68EE;

  }

}

h1 {
  text-shadow: .1rem .1rem .5rem pink;
}

p {
  text-shadow: .1rem .1rem .5rem lightpink;

}
</style>
