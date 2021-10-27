<template>
	<div class="w-full h-24 bg-gray-900 border-double border-b-8 border-gray-500">
		<div class="flex justify-between pt-5">
			<div class="flex mt-auto mb-auto">
				<img class="h-12 w-12 ml-4 mt-auto mb-auto" src="../static/favicon.svg"/>
				<div class="text-lg text-visudo-green font-bold mt-auto mb-auto ml-2 hidden sm:block"> Streaming | Web Development </div>
			</div>
			<div class="hidden mt-auto mb-auto text-lg text-blue-600 font-bold sm:flex">
				<a class="mr-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.twitch.tv/v1sudo" target="_blank">Twitch</a> |
				<a class="ml-2 mr-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.twitter.com/v1sudo" target="_blank">Twitter</a> |
				<a class="ml-2 mr-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.youtube.com/channel/UC4gq_UflDu--JuISXL4C8UQ" target="_blank">YouTube</a> |
				<a class="ml-2 mr-4 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://github.com/visudo20179C" target="_blank">GitHub</a>
			</div>
			<div class="flex sm:hidden">
				<button @click="toggleMenu">
					<transition name="fade" mode="out-in">
						<div v-if="!shouldToggleMenu" key="0">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 mr-2 text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
							  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
							</svg>
						</div>
						<div v-else key="1">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 mr-2 text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
							  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 14l2-2m0 0l2-2m-2 2l-2-2m2 2l2 2m7-2a9 9 0 11-18 0 9 9 0 0118 0z" />
							</svg>
						</div>
					</transition>
				</button>
			</div>
		</div>
		<transition name="fade" mode="out-in">
			<div v-if="shouldToggleMenu" class="mt-10 w-full text-lg text-blue-600 font-bold sm:hidden absolute z-40">
					<div class="flex flex-col text-right bg-transparent">
						<a class="px-4 py-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.twitch.tv/v1sudo" target="_blank">Twitch</a>
						<a class="px-4 py-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.twitter.com/v1sudo" target="_blank">Twitter</a>
						<a class="px-4 py-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://www.youtube.com/channel/UC4gq_UflDu--JuISXL4C8UQ" target="_blank">YouTube</a>
						<a class="px-4 py-2 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://github.com/visudo20179C" target="_blank">GitHub</a>
					</div>
			</div>
		</transition>
	</div>
</template>

<script>
export default {
	name: 'Header',
	data() {
		return {
			shouldToggleMenu: false,
		}
	},
	methods: {
		toggleMenu() {
			this.shouldToggleMenu = !this.shouldToggleMenu
		}
	},
}
</script>

<style>
.fade-enter-active, .fade-leave-active {
  transition: opacity .5s;
}
.fade-enter, .fade-leave-to /* .fade-leave-active below version 2.1.8 */ {
  opacity: 0;
}
</style>

