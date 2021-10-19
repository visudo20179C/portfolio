<template class="bg-gray-900">
	<div class="bg-gray-900">
		<div class="w-1/2 h-80 mt-10 mb-10 ml-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg relative">
			<div class="w-2/3 text-2xl text-visudo-green font-black mb-10 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
				root@visudo:~$ whoami
			</div>
			<transition name="fade">
				<div class="text-gray-900 text-center" v-show="!firstShow">
					Why do I call myself "visudo"?
				</div>
			</transition>
			<transition name="fade">
				<div class="text-gray-900 text-center" v-show="firstShow">
				It's based upon the Linux command visudo. visudo locks the sudoers file against multiple simultaneous edits, provides basic sanity checks, and checks for parse errors. The sudoers file controls who can run commands as the root user of the OS.
				</div>
			</transition>
			<div class="absolute bottom-0 left-10 right-10">
				<div class="flex justify-center">
					<button @click="firstShowPrev">
						<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
						</svg>
					</button>
					<button @click="firstShowNext">
						<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
							<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
						</svg>
					</button>
				</div>
			</div>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Main',
	data() {
		return {
			firstShow: false,
		}
	},
	methods: {
		firstShowNext() {
			this.firstShow = true
		},
		firstShowPrev() {
			this.firstShow = false
		},
	}
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

