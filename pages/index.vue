<template>
  <div class="w-screen h-80 flex flex-col justify-around items-center giant-text text-yellow-600 ">
    <div class="star">
      *
    </div>
    <div class="word-karma ml-2">
      KARMA
    </div>
    <div class="word-church">
      CHURCH
    </div>
    <div class="text-xl italic mt-4">
      {{ tagline }}
    </div>
    <div class="star star-2">
      *
    </div>
  </div>
</template>

<script>

export default {
  data () {
    return {
      tagline: '',
      taglines: [
        `Don't be an asshole`,
        `No crystals allowed`,
        `Bring all your crystals`,
        `Bring your religion`,
        `Leave your religion at home`,
        `Double rainbows all the way`
      ]
    }
  },
  mounted () {
    this.selectPhrase()
  },
  methods: {
    selectPhrase () {
      this.tagline = this.taglines[Math.floor(Math.random() * this.taglines.length)]
    }
  }
}
</script>

<style scoped>
  .star {
    line-height: 1em;
  }
  .star-2 {
    transform:rotate(-180deg);
  }
  .giant-text {
    line-height: 0.9;
    font-size: 20vw
  }
  .word-karma {
    letter-spacing: 0.22em;
  }
  .word-church {
    letter-spacing: 0.05em;
  }
</style>
