<template>
  <div class="w-full h-screen bg-gray-100 flex flex-col items-center justify-center p-4 relative overflow-hidden">
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

<script>
export default {
  name: 'App'
}
</script>

<style>
.font-satisfy {
  font-family: 'Satisfy', cursive;
}

h1 {
  text-shadow: .1rem .1rem .5rem pink;
}

p {
  text-shadow: .1rem .1rem .5rem lightpink;

}
</style>
