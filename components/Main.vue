<template class="bg-gray-900">
	<div class="w-full">
		<div class="w-5/6 h-5/6 mt-20 mb-10 mx-auto bg-gray-900 border-b-4 border-gray-500 rounded shadow-lg relative lg:h-80">
			<div class="mb-24 w-3/4 m-auto">
				<transition name="fade" mode="out-in">
					<div v-if="!firstShow" key="0">
						<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg border-gray-900 text-center ml-auto mr-auto">
							Who am I?
						</div>
						<div class="text-gray-500 text-lg font-bold md:mb-0">
							Hi, my name is Cameron, otherwise known as my online alias "visudo". I stream on Twitch and I'm also a full-stack web developer who has been doing web development work for 3+ years. My technology "stack" consists of Linux, PHP, MySQL, JavaScript, &amp; HTML/CSS.
						</div>
					</div>
					<div class="text-gray-900 text-left" v-else-if="firstShow" key="1">
						<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg border-gray-900 text-center ml-auto mr-auto sm:w-2/3">
							What do I want to do?
						</div>
						<div class="mb-10 text-gray-500 text-lg font-bold md:mb-0">
							I want to develop websites and web services for Streamers and Content Creators alike. The benefit of hiring me compared to going with a competitor is that you get a completely customized experience. I also have extensive knowledge using 3rd-party API's such as PayPal, Twitch, Discord, and more.
						</div>
					</div>
				</transition>
			</div>
			<div class="pb-8">
				<div class="absolute bottom-4 left-10 right-10">
					<div class="flex justify-center">
						<button @click="firstShowPrev">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-visudo-green hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
							</svg>
						</button>
						<button @click="firstShowNext">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-visudo-green hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
							</svg>
						</button>
					</div>
				</div>
			</div>
		</div>
		<div class="w-5/6 h-5/6 mt-4 mb-10 mx-auto bg-gray-900 shadow-lg font-bold text-gray-500">
			<div class="w-2/3 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center mx-auto">
				What have I done?
			</div>
			<div class="border-b-4 rounded border-gray-500">
				<div class="text-left mb-6 mt-6 w-3/4 ml-auto mr-auto text-lg">
					I've worked on several websites and web projects. My core langauges are PHP &amp; JavaScript. I've used these languages to implement standalone projects as well as projects using a framework such as Laravel or VueJS. Here are some examples:
				</div>
				<div class="text-left ml-2 w-5/6 ml-auto mr-auto text-sm mb-12 pt-8 flex flex-col justify-evenly divide-x divide-gray-900 lg:flex-row lg:divide-gray-500">
					<div class="flex flex-col mb-4 lg:mb-0"><a href="https://staging.ponder-app.org/" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Ponder</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">An API-based Trivia Application craeted with a Laravel back-end and InertiaJS front-end.</div></div>
					<div class="flex flex-col mb-4 lg:mb-0"><a href="https://connect-four.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Connect Four</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">A web-based version of the game "Connect-Four" with a VueJS front-end and socket.io back-end.<a href="https://github.com/visudo20179C/connect-four" target="_blank"><img src="../static/GitHub-Mark-Light-32px.png" class="m-auto mt-4"/></a></div></div>
					<div class="flex flex-col"><a href="https://apex-stats.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Apex Stats</a><div class="w-2/3 m-auto mt-4 text-center">A hobby project that was inspired by my love for gaming. This is a "server-less" VueJS project.<a href="https://github.com/visudo20179C/apex-player-stats" target="_blank"><img src="../static/GitHub-Mark-Light-32px.png" class="m-auto mt-4"/></a></div></div>
				</div>
			</div>
		</div>
		<div class="w-5/6 border-b-4 rounded border-gray-500 mx-auto">
			<transition name="fade" mode="out-in">
				<div v-if="!secondShow" key="0">
					<div class="w-2/3 text-3xl text-visudo-green font-black mb-8 mt-4 text-center ml-auto mr-auto">
						What do I like to make?
					</div>
					<div class="mx-auto h-3/4 w-3/4 flex flex-col justify-evenly items-top mb-10 pb-10 text-center text-gray-900 font-bold lg:h-80 lg:flex-row">
						<div class="w-1/2 mx-auto border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4">
							<div class="mx-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">Node.js Micro-services</div>
							<img src="../static/Node.js_logo.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="ml-auto mr-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">CRUD applications</div>
							<img src="../static/lara.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="ml-auto mr-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">Single Page Applications</div>
							<img src="../static/Vue.js_Logo_2.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
					</div>
				</div>
				<div v-else-if="secondShow" key="1">
					<div class="w-2/3 text-3xl text-visudo-green font-black mb-8 mt-4 text-center ml-auto mr-auto">
						What services can I integrate?
					</div>
					<div class="mx-auto h-3/4 w-3/4 flex flex-col justify-evenly items-top mb-10 pb-10 text-center text-gray-900 font-bold lg:h-80 lg:flex-row">
						<div class="w-1/2 mx-auto border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4">
							<div class="mx-auto mt-4 text-lg mb-4 text-visudo-green font-black">Discord</div>
							<img src="../static/js_discord-ar21.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="mx-auto mt-4 text-lg mb-4 text-visudo-green font-black">Twitch</div>
							<img src="../static/Twitch_logo.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-gray-500 bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="mx-auto mt-4 mb-0 text-lg text-visudo-green font-black lg:mb-16">GitHub</div>
							<img src="../static/GitHub_Logo_White.png" class="mt-4 pb-4 lg:pb-0"/>
						</div>
					</div>
				</div>
			</transition>
			<div class="pb-8">
				<div class="">
					<div class="flex justify-center">
						<button @click="secondShowPrev">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-visudo-green hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
							</svg>
						</button>
						<button @click="secondShowNext">
							<svg xmlns="http://www.w3.org/2000/svg" class="h-8 w-8 text-visudo-green hover:text-visudo-blue" fill="none" viewBox="0 0 24 24" stroke="currentColor">
								<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
							</svg>
						</button>
					</div>
				</div>
			</div>
		</div>
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-10 mt-8 text-center mx-auto">
			My Twitch Channel:
		</div>
		<div class="flex flex-col h-full w-full justify-evenly mb-10 lg:flex-row mx-auto lg:w-3/4">
			<div class="w-5/6 lg:w-1/2 mx-auto mb-4 lg:mb-none">
				<div ref="tVideo"/>
			</div>
			<div class="w-1/2 h-full mb-4 text-center mx-auto">
				<transition name="fade" mode="out-in">
					<div v-if="this.data != null" class="text-visudo-green" key="0">
						<div class="text-2xl font-bold mb-10">
							My last played legend in "Apex Legends":
						</div>
						<div class="text-2xl font-bold mt-10">
							{{this.data.legends.selected.LegendName}}
						</div>
						<img class="object-contain mx-auto h-48 w-48" :src="this.data.legends.selected.ImgAssets.icon"/>
						<p class="ml-auto mr-auto mb-4 w-64 mx-auto">
							Skin: <i>{{this.data.legends.selected.gameInfo.skin}}</i>
						</p>
						<h1 class="text-xl mb-4 mx-auto">Equipped Trackers:</h1>
						<ul>
							<div v-for="item in this.data.legends.selected.data" class="flex flex-col divide-y divide-gray-500 mx-auto">
								<li class="w-5/6 mx-auto">{{item.name}}: {{item.value}}</li>
							</div>
						</ul>
					</div>
					<div v-else class="text-visudo-green" key="1">
						<div class="text-2xl mb-10 mt-10">Loading... Please Wait... </div>
						<half-circle-spinner
						  :animation-duration="1000"
						  :size="100"
						  color="#15AB0D"
						  class="m-auto"
						/>
					</div>
				</transition>
			</div>
		</div>
	</div>
</template>

<script>
import Twitch from '../lib/twitch.v1.js'
import { HalfCircleSpinner } from 'epic-spinners'

export default {
	name: 'Main',
	components: {HalfCircleSpinner},
	data() {
		return {
			firstShow: false,
			secondShow: false,
			player: null,
			data: null,
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
		processData(data) {
			this.data = data
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
	},
	created() {
		fetch(
			"https://api.mozambiquehe.re/bridge?version=5&platform=PC&player=visudo20179&auth=QYMCCkwuWGEeBQFL30tT",
			{
				method: 'GET',
			}
		)
		.then(response => response.json())
		.then(data => this.processData(data))
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
iframe {
	margin: auto;
	border-radius: 20px;
}
</style>

