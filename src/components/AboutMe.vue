<template>
  <div class="about">
    <div class="about-info" :class="{ 'fade-in': isVisible }">
      <h1>About Me</h1>
      <p>
        I'm a front end developer that learned everything on my own. I specialize in creating
        dynamic, accessible websites that work on any device. Furthermore, I regularly create
        creative solutions that improve user experiences. I am proficient in React.js, Redux,
        JavaScript, HTML5, and CSS. I guarantee efficient code management and communication thanks
        to my knowledge with Git version control. Likewise, I'm also skilled at developing apps
        using mini program studio frameworks and exceeding client expectations with my high-caliber
        solutions.
      </p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isVisible: false,
    }
  },
  methods: {
    handScroll() {
      const element = this.$el.querySelector('.about-info')
      const rect = element.getBoundingClientRect()

      if (rect.top < window.innerHeight && rect.bottom >= 0) {
        this.isVisible = true
      } else {
        this.isVisible = false
      }
    },
  },
  mounted() {
    window.addEventListener('scroll', this.handScroll)
    this.handScroll()
  },
  beforeDestroy() {
    window.removeEventListener('scroll', this.handelScroll)
  },
}
</script>

<style scoped>
.about {
  width: 100%;
  height: 640px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.about-info {
  width: 1200px;
  border-radius: 20px;
  height: 400px;
  display: flex;
  flex-direction: column;
  justify-content: center;
  box-shadow: 0 4px 10px rgba(0, 0, 0, 0.2);
  opacity: 0;
  transition: opacity 1s ease-in-out;
}

.about-info.fade-in {
  opacity: 1;
}

.about-info h1 {
  color: rgb(17 24 39);
  font-weight: bold;
  font-size: 20px;
  margin-bottom: 20px;
  margin-left: 20px;
}

.about-info p {
  color: rgb(17 24 39);
  font-size: 20px;
  line-height: 1.25rem;
  margin-left: 20px;
}
@media (max-width: 900px) {
	.about {
		align-items: center;
		display: flex;
		margin-left: 22px;
		width: 350px;
		margin-left: 25px;
		height: 500px;
	}
	.about-info {
		height: 400px;
	} 
}
</style>
