<template>
  <div class="parallax-container" :style="{ width: width, height: height }">
    <div ref="parallax" class="parallax" :style="parallaxStyle">
      <img :src="imageUrl" alt="Parallax Image" style="transform: scale(1.5)" />
    </div>
  </div>
</template>

<script>
export default {
  props: {
    imageUrl: String,
    intensity: {
      type: Number,
      default: 0.5,
    },
    width: {
      type: String,
      default: "100%",
    },
    height: {
      type: String,
      default: "100%",
    },
    direction: {
      type: String,
      default: "Vertical",
    },
    transition: {
      type: String,
      default: "transform 0.3s ease-out",
    },
  },
  data() {
    return {
      scrollPosition: 0,
      coordinates: {},
    };
  },
  computed: {
    parallaxStyle() {

        if (this.direction === "Horizontal") {
        return {
          transform: `translateX(${this.scrollPosition * this.intensity}px)`,
          transition: this.transition,
        };
      }
      else {
        return {
          transform: `translateY(${this.scrollPosition * this.intensity}px)`,
          transition: this.transition,
        };
      }
    
   
    },
  },
  methods: {
    handleScroll() {
      this.scrollPosition = window.scrollY - this.coordinates.y;
    },
    
  },
  mounted() {
    window.addEventListener("scroll", this.handleScroll);
    const el = this.$refs.parallax;
    const coordinates = el.getBoundingClientRect();
    this.coordinates = coordinates;
    console.log(this.coordinates);
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.handleScroll);
  },
};
</script>

<style scoped>
.parallax-container {
  position: relative;
  overflow: hidden;
}

.parallax {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

img {
  max-width: 100%;
  height: auto;
}
</style>
