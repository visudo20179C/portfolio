<template class="bg-gray-900">
	<div class="flex flex-col bg-gray-900 h-full w-full justify-between">
		<div class="w-1/2 h-80 mt-10 mb-10 ml-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg relative">
			<div class="w-2/3 text-2xl text-visudo-green font-black mb-10 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
				whoami?
			</div>
			<transition name="fade">
				<div class="text-gray-900 text-center" v-show="!firstShow">
					Hi, my name is Cameron, otherwise known as my online alias "visudo". I'm a full-stack web developer who has been doing web development work for 3+ years, mostly self-taught. Why do I call myself "visudo"?
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
		<div class="w-1/2 h-80 mt-10 mb-10 mr-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg self-end relative">
			<div class="w-2/3 text-2xl text-visudo-green font-black mb-4 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
				What have I done?
			</div>
			<div class="text-gray-900 text-center mb-4">
				I've worked on several websites and web projects. My core langauges are PHP &amp; JavaScript. I've used these languages to implement standalone projects as well as projects using a framework such as Laravel or VueJS. Some cool examples would be:
			</div>
			<ul class="text-gray-900 text-left ml-2">
				<li class="mb-4"><a href="https://staging.ponder-app.org/" target="_blank" class="text-blue-600 border-2 rounded-full py-1.5 px-3 border-blue-600 text-lg font-black hover:text-blue-400 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">Ponder</a> - An API-based Trivia Application written in the Laravel framework.</li>
				<li class="mb-4"><a href="https://connect-four.visudo.me/" target="_blank" class="text-blue-600 border-2 rounded-full py-1.5 px-3 border-blue-600 text-lg font-black hover:text-blue-400 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">ConnectFour</a> - A web-based version of the game "Connect-Four" in the VueJS framework.<a href="https://github.com/visudo20179C/connect-four" target="_blank"><img src="../static/GitHub-Mark-32px.png" class="inline-block h-6 w-6 ml-2"/></a></li>
				<li class="mb-4"><a href="https://apex-stats.visudo.me/" target="_blank" class="text-blue-600 border-2 rounded-full py-1.5 px-3 border-blue-600 text-lg font-black hover:text-blue-400 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">ApexPlayerStats</a> - A hobby project that was inspired by my love for gaming. Another in VueJS.<a href="https://github.com/visudo20179C/apex-player-stats" target="_blank"><img src="../static/GitHub-Mark-32px.png" class="inline-block h-6 w-6 ml-2"/></a></li>
			</ul>
		</div>
		<div class="w-1/2 h-80 mt-10 mb-10 ml-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg relative">
			<div class="w-2/3 text-2xl text-visudo-green font-black mb-4 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
				What do I want to do?
			</div>
			<div class="text-gray-900 text-center mb-4">
				I want to develop websites and web services for Streamers, YouTubers, Pro-Gamers, and Content Creators alike. The benefit of hiring me compared to a large competitor is that you get an intimate, one-on-one user experience. I don't just make flat pages with walls of texts and links. I make functioning, innovative, sites and services that can interact with 3rd-party services and display meaningful and useful data. 
			</div>
			<ul class="ml-8 text-gray-900">Use Cases:
				<li> - A CRUD application with a web front-end.</li>
				<li> - A Node.js micro-service, such as a Discord Bot.</li>
				<li> - A Single Page Application (SPA).</li>
				<li> - Or anything else you can think of. I love taking on new challenges!</li>
			</ul>
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

