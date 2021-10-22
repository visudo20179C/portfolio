<template class="bg-gray-900">
	<div>
		<div class="flex flex-col bg-gray-900 h-full w-full justify-center items-center sm:flex-row">
			<div class="w-2/3 h-5/6 mt-10 mb-10 ml-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg relative sm:w-1/3">
				<div class="w-2/3 text-2xl text-visudo-green font-black mb-8 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
					Who Am I?
				</div>
				<div class="mb-24 w-3/4 m-auto">
					<transition name="fade" mode="out-in">
						<div class="text-gray-900 text-left" v-if="!firstShow" key="0">
							Hi, my name is Cameron, otherwise known as my online alias "visudo". I'm a full-stack web developer who has been doing web development work for 3+ years, mostly self-taught. Why do I call myself "visudo"?
						</div>
						<div class="text-gray-900 text-left" v-else-if="firstShow" key="1">
							It's based upon the Linux command visudo. visudo locks the sudoers file against multiple simultaneous edits, provides basic sanity checks, and checks for parse errors. The sudoers file controls who can run commands as the root user of the OS.
						</div>
					</transition>
				</div>
				<div class="pb-8">
					<div class="absolute bottom-10 left-10 right-10">
						<div class="flex justify-center">
							<button @click="firstShowPrev">
								<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-900 hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
								</svg>
							</button>
							<button @click="firstShowNext">
								<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-900 hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
								</svg>
							</button>
						</div>
					</div>
				</div>
			</div>
			<div class="w-2/3 h-5/6 mt-10 mb-10 ml-4 bg-gray-500 border rounded-lg border-gray-900 shadow-lg relative sm:w-1/3">
				<div class="w-2/3 text-2xl text-visudo-green font-black mb-4 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
					What do I want to do?
				</div>
				<div class="mt-8 mb-24 w-3/4 m-auto">
					<transition name="fade" mode="out-in">
						<div class="text-gray-900 text-left" v-if="!secondShow" key="0">
							I want to develop websites and web services for Streamers and Content Creators alike. The benefit of hiring me compared to going with a competitor is that you get a completely customized experience. I make dynamic sites that are rich with style and custom features.
						</div>
						<div class="text-gray-900 text-left" v-else-if="secondShow" key="1">
							I also have extensive knowledge using 3rd-party API's such as PayPal, Twitch, Discord, and more. This gives me the oppourtunity to add custom features to your website and interact with other services that you use that would otherwise be unavailable.
						</div>
					</transition>
				</div>
				<div class="pb-8">
					<div class="absolute bottom-10 left-10 right-10">
						<div class="flex justify-center">
							<button @click="secondShowPrev">
								<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-900 hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
								</svg>
							</button>
							<button @click="secondShowNext">
								<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-gray-900 hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
								</svg>
							</button>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div class="w-3/4 h-5/6 mt-4 mb-10 mx-auto bg-gray-500 border rounded-lg border-gray-900 shadow-lg">
			<div class="w-2/3 text-2xl text-visudo-green font-black mb-6 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center ml-auto mr-auto">
				What have I done?
			</div>
			<div class="divide-y divide-gray-900">
				<div class="text-gray-900 text-center mb-4 mt-4 w-3/4 ml-auto mr-auto">
					I've worked on several websites and web projects. My core langauges are PHP &amp; JavaScript. I've used these languages to implement standalone projects as well as projects using a framework such as Laravel or VueJS. Here are some examples:
				</div>
				<div class="text-gray-900 text-left ml-2 w-5/6 ml-auto mr-auto text-sm mb-12 pt-8 flex flex-col justify-between sm:flex-row">
					<div class="flex flex-col"><a href="https://staging.ponder-app.org/" target="_blank" class="w-2/3 ml-auto mr-auto text-gray-900 text-center text-xs sm:text-md border-2 rounded-full py-1.5 px-3 border-gray-900 text-md font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">Ponder</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">An API-based Trivia Application written in the Laravel framework.</div></div>
					<div class="flex flex-col"><a href="https://connect-four.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-gray-900 text-center text-xs sm:text-md border-2 rounded-full py-1.5 px-3 border-gray-900 text-md font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">ConnectFour</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">A web-based version of the game "Connect-Four" in the VueJS framework.<a href="https://github.com/visudo20179C/connect-four" target="_blank"><img src="../static/GitHub-Mark-32px.png" class="m-auto mt-4"/></a></div></div>
					<div class="flex flex-col"><a href="https://apex-stats.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-gray-900 text-center text-xs sm:text-md border-2 rounded-full py-1.5 px-3 border-gray-900 text-md font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60">ApexPlayerStats</a><div class="w-2/3 m-auto mt-4 text-center">A hobby project that was inspired by my love for gaming. Another in VueJS.<a href="https://github.com/visudo20179C/apex-player-stats" target="_blank"><img src="../static/GitHub-Mark-32px.png" class="m-auto mt-4"/></a></div></div>
				</div>
			</div>
		</div>
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-4 mt-4 text-center ml-auto mr-auto">
			Things I can create:
		</div>
		<div class="ml-auto mr-auto h-60 w-full flex flex-row justify-evenly items-top mb-10 text-center text-gray-900 font-bold sm:h-80">
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 md:text-lg mb-4">Node.js Micro-services</div>
				<img src="../static/Node.js_logo.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 md:text-lg mb-4">A CRUD application</div>
				<img src="../static/lara.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 md:text-lg mb-4">A Single Page Application</div>
				<img src="../static/Vue.js_Logo_2.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 md:text-lg mb-4">Any other project ideas</div>
				<img src="../static/idee.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
		</div>
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-4 mt-4 text-center ml-auto mr-auto">
			Services I can integrate:
		</div>
		<div class="ml-auto mr-auto h-60 w-full flex flex-row justify-evenly items-top mb-10 text-center text-gray-900 font-bold sm:h-80">
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 text-lg mb-4">Discord</div>
				<img src="../static/js_discord-ar21.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 text-lg mb-4">Twitch</div>
				<img src="../static/Twitch_logo.svg" class="m-auto w-2/3 h-2/3"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 text-lg mb-16">GitHub</div>
				<img src="../static/GitHub_Logo.png" class="m-auto"/>
			</div>
			<div class="w-1/6 border border-2 rounded-lg border-gray-900 bg-gray-500">
				<div class="ml-auto mr-auto mt-4 text-lg mb-16">3rd-party APIs</div>
				<img src="../static/Globe_icon.svg" class="m-auto h-1/3 w-1/3"/>
			</div>
		</div>
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-4 mt-4 text-center ml-auto mr-auto">
			My Twitch Channel:
		</div>
		<div class="mb-10 w-3/4 ml-auto mr-auto">
			<div class="border border-2 rounded-lg border-gray-900 bg-gray-500 pt-10 pb-10" ref="tVideo"/>
		</div>
	</div>
</template>

<script>
import Twitch from '../lib/twitch.v1.js'

export default {
	name: 'Main',
	data() {
		return {
			firstShow: false,
			secondShow: false,
			player: null,
		}
	},
	methods: {
		firstShowNext() {
			this.firstShow = true
		},
		firstShowPrev() {
			this.firstShow = false
		},
		secondShowNext() {
			this.secondShow = true
		},
		secondShowPrev() {
			this.secondShow = false
		},
	},
	mounted() {
		const options = {
			width: '66%',
			height: 480,
			channel: 'v1sudo',
		}
		this.player = new Twitch.Player(this.$refs.tVideo, options)
		this.player.setVolume(0.5)
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
iframe {margin: auto}
</style>

