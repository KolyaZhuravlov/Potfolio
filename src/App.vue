<script>
import AboutMe from './components/AboutMe.vue';
import Contact from './components/Contact.vue';
import NavBar from './components/NavBar.vue';
import Project from './components/Project.vue';
import Scills from './components/Scills.vue';
export default {
	components: {NavBar,AboutMe,Scills,
		Project,Contact
	}
}
</script>

<template >
 <NavBar/>
 <AboutMe/>
 <Project/>
 <Scills/>
 <Contact/>
</template>

<style scoped>

</style>
