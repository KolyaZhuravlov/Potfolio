<template>
  <div class="mb-24 h-auto w-full sm:mb-0 md:h-screen">
    <div>
      <p
        class="mx-auto w-[50%] pb-10 pt-8 text-center text-2xl tracking-wider text-gray-900 lg:text-3xl"
      >
        Projects
      </p>
    </div>

    <div class="mx-auto mb-2 grid w-[90%] grid-cols-1 gap-4 sm:mb-8 md:grid-cols-2">
      <div
        class="mb-8 h-auto rounded-lg bg-transparent p-4 shadow-[rgba(50,_50,_105,_0.15) _0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px] hover:shadow-[0_8px_30px_rgb(0,0,0,0.12)]"
      >
        <h2 class= "text-gray-900 mb-2 cursor-pointer text-base font-semibold lg:text-xl"
		  @click="goToProjectWeaher">Weater Vue</h2>
        <p class="text-gray-900 mt-3 flex flex-wrap lg:mt-6">
          Stratagile HRMS is a web-based Human Resource Management System built using React. It is
          designed to streamline HR proce
        </p>
        <div class="mt-3 flex flex-wrap lg:mt-6" >
			<p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Vue JS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">CSS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Tailwind</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Git</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">GitHub</p>
		  </div>
      </div>
		<div class="mb-8 h-auto rounded-lg bg-transparent p-4 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px] hover:shadow-[0_8px_30px_rgb(0,0,0,0.12)]">
			<h2 class= " text-gray-900 mb-2 cursor-pointer text-base font-semibold lg:text-xl" @click="goToProjectWeaterIo">Weater JS</h2>
        <p class="text-gray-900">
			Contributed to the frontend development of Zymsi, a platform facilitating flexible gym memberships. Implemented user-fri
		  </p>
		  <div class="mt-3 flex flex-wrap lg:mt-6" >
			<p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Vue JS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">CSS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Tailwind</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Git</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">GitHub</p>
		  </div>
		</div>
		<div class="mb-8 h-auto rounded-lg bg-transparent p-4 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px] hover:shadow-[0_8px_30px_rgb(0,0,0,0.12)]">
			<h2 class= "text-gray-900 mb-2 cursor-pointer text-base font-semibold lg:text-xl"
			@click="goToProjectKatya">Katya KatyaZhuravlova</h2>
        <p class="text-gray-900">
			Contributed to the frontend development of Zymsi, a platform facilitating flexible gym memberships. Implemented user-fri
		  </p>
		  <div class="mt-3 flex flex-wrap lg:mt-6" >
			<p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Vue JS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">CSS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Tailwind</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Git</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">GitHub</p>
		  </div>
		</div>
		<div class="mb-8 h-auto rounded-lg bg-transparent p-4 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px] hover:shadow-[0_8px_30px_rgb(0,0,0,0.12)]">
			<h2 class= " text-gray-900 mb-2 cursor-pointer text-base font-semibold lg:text-xl" @click="goToProjectTodo">Todo-List-Git</h2>
        <p class="text-gray-900">
			Contributed to the frontend development of Zymsi, a platform facilitating flexible gym memberships. Implemented user-fri
		  </p>
		  <div class="mt-3 flex flex-wrap lg:mt-6" >
			<p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Vue JS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">CSS</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Tailwind</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">Git</p>
			 <p class="mr-2 inline-block  rounded-full bg-transparent px-3 py-1 text-sm font-semibold text-gray-900
			 shadow-[rgba(50,_50,_105,_0.15)_0px_2px_5px_0px,_rgba(0,_0,_0,_0.05)_0px_1px_1px_0px]">GitHub</p>
		  </div>
		</div>
    </div>
  </div>
</template>

<script>
export default {
	methods:{
		goToProjectWeaher() {
			window.location.href = 'https://kolyazhuravlov.github.io/Weather-Vue/'
		},
		goToProjectKatya() {
			window.location.href = 'https://kolyazhuravlov.github.io/KatyaZhuravlova.io/'
		},
		goToProjectTodo() {
			window.location.href = 'https://kolyazhuravlov.github.io/Todo-List-Git/'
		},
		goToProjectWeaterIo() {
			window.location.href = 'https://kolyazhuravlov.github.io/Weather22.io/'
		}
	},
  data() {
    return {}
  }
}
</script>

<style scoped></style>
