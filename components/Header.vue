<template>
	<div class="w-full h-24 bg-gray-900 border-double border-b-8 border-gray-500">
		<div class="flex justify-between pt-5">
			<div class="flex mt-auto mb-auto">
				<img class="h-12 w-12 ml-4 mt-auto mb-auto" src="../static/favicon.svg"/>
				<div class="text-lg text-visudo-green font-bold mt-auto mb-auto ml-2 hidden sm:block"> Web Development </div>
			</div>
			<div class="mt-auto mb-auto text-lg text-blue-600 font-bold">
				<a class="ml-2 mr-4 hover:text-blue-300 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60" href="https://github.com/visudo20179C" target="_blank">GitHub</a>
			</div>
		</div>
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

