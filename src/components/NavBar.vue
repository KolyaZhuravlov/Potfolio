<template>
  <div class="navbar">
    <div class="header">
      <ul class="left">
        <li>
			<svg class="logo" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
				 <path fill="#74C0FC" d="M96 0C60.7 0 32 28.7 32 64l0 384c0 35.3 28.7 64 64 64l288 0c35.3 0 64-28.7 64-64l0-384c0-35.3-28.7-64-64-64L96 0zM208 288l64 0c44.2 0 80 35.8 80 80c0 8.8-7.2 16-16 16l-192 0c-8.8 0-16-7.2-16-16c0-44.2 35.8-80 80-80zm-32-96a64 64 0 1 1 128 0 64 64 0 1 1 -128 0zM512 80c0-8.8-7.2-16-16-16s-16 7.2-16 16l0 64c0 8.8 7.2 16 16 16s16-7.2 16-16l0-64zM496 192c-8.8 0-16 7.2-16 16l0 64c0 8.8 7.2 16 16 16s16-7.2 16-16l0-64c0-8.8-7.2-16-16-16zm16 144c0-8.8-7.2-16-16-16s-16 7.2-16 16l0 64c0 8.8 7.2 16 16 16s16-7.2 16-16l0-64z"/></svg>
		  </li>
      </ul>

      <ul class="right">
        <li @click="scrollAbout">About Me</li>
		  <li @click="scrollProject">Progect</li>
        <li @click="scroolSkills">Skills</li>
        <li @click="scrollContact">Contact</li>
      </ul>
    </div>
  </div>

  <InfoText />
</template>

<script>
import { Icon } from '@iconify/vue'
import InfoText from './InfoText.vue'

export default {
  components: { InfoText },
  methods: {
    scrollAbout() {
		const scrollAmount = window.innerWidth <= 900 ? 850 : 700;
		window.scrollBy({
        top: scrollAmount,
        behavior: 'smooth'
		})
      },
		scrollProject() {
			const scrollAmount = window.innerWidth <= 900 ? 1320 : 1320;
			window.scrollBy({
				top: scrollAmount,
				behavior:'smooth'
			})
		},
		scroolSkills() {
			const scrollAmount = window.innerWidth <= 900 ? 3000 : 1750;
			window.scrollBy({
				top: scrollAmount,
				behavior: 'smooth'
			})
		},
		scrollContact() {
			const scrollAmount = window.innerWidth <= 900 ? 3700 : 1850;
			window.scrollBy({
				top: scrollAmount,
				behavior: 'smooth'
			})
		}
    }
  }
</script>

<style scoped>
.header {
  display: flex;
  width: 100%;
  height: 75px;
}

ul {
  display: flex;
  padding: 0;
  margin: 0;
  list-style: none;
}
.left {
  margin-left: 25px;
  list-style: none;
}

.right {
  margin-left: auto;
  cursor: pointer;
}

li {
  padding-top: 25px;
  margin-right: 5px;
  margin-right: 25px;
  transition: color 0.3s;
}

li:last-child {
  margin-right: 25px;
}

li:hover {
  color: blueviolet;
}
.logo{
	width: 40px;
	height: 40px;
}
@media (max-width: 900px) {
	.right {
		font-size:19px;
		transition: color 0.3s ease;
	}
	.right:active, .right:focus {
    color: #FF5733;
  }
  .left svg {
	width: 25px;
	padding-bottom: 10px;
  }
}
</style>
