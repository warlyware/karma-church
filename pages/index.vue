<template>
  <div class="w-screen h-screen flex flex-col justify-around items-center bg-blue-800 giant-text">
    <div class="text-yellow-600 star">
      *
    </div>
    <div class="text-yellow-600 word-karma ml-2">
      KARMA
    </div>
    <div class="text-yellow-600 word-church">
      CHURCH
    </div>
    <div class="text-yellow-600 star star-2">
      *
    </div>
  </div>
</template>

<script>

export default { }
</script>

<style scoped>
  .star {
    line-height: 1em;
  }
  .star-2 {
    transform:rotate(-180deg);
  }
  .giant-text {
    line-height: 0.8;
    font-size: 20vw
  }
  .word-karma {
    letter-spacing: 0.22em;
  }
  .word-church {
    letter-spacing: 0.05em;
  }
</style>
