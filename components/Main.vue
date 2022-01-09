<template class="bg-gray-900">
	<div class="w-full">
		<div class="w-full h-5/6 mt-12 mb-10 mx-auto bg-gray-900">
			<div class="mb-12 w-3/4 m-auto flex flex-col lg:flex-row divide-x divide-gray-900 lg:divide-gray-500">
				<div class="w-2/3 mx-auto mb-8">
					<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg border-gray-900 text-center ml-auto mr-auto">
						About me:
					</div>
					<img class="w-48 h-48 rounded-full mx-auto mb-2" src="me2.jpg" alt="A picture of me in Times Square NY.">
					<div class="text-visudo-green text-xs text-center mb-4"><i>A picture of me in Times Square, NY.</i></div>
					<div class="text-gray-500 text-md text-left md:mb-0 w-3/4 mx-auto">
						Hi, my name is Cameron, otherwise known as my online alias "visudo". I stream on Twitch and I'm also a full-stack web developer who has been doing web development work for 3+ years. I make things using Linux, PHP, MySQL, JavaScript, &amp; HTML/CSS.
					</div>
				</div>
				<div class="w-2/3 mx-auto">
					<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg border-gray-900 text-center ml-auto mr-auto sm:w-2/3">
						Work with me:
					</div>
					<svg xmlns="http://www.w3.org/2000/svg" class="h-48 w-48 rounded-full mx-auto text-visudo-green mb-8" fill="none" viewBox="0 0 24 24" stroke="currentColor">
					  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
					</svg>
					<div class="mb-10 text-gray-500 text-md text-right md:mb-0 w-3/4 mx-auto">
						I want to develop websites and web services for streamers, content creators, and other professionals. Working with me gives you a 1-on-1 experience tailored to specific web needs. I have extensive knowledge using 3rd-party technologies such as PayPal, Twitch, Discord, and more.
					</div>
				</div>
			</div>
		</div>
		<div class="w-5/6 h-5/6 mt-10 mb-10 mx-auto bg-gray-900 text-gray-500">
			<div class="w-2/3 text-3xl text-visudo-green font-black mb-8 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center mx-auto">
				Dev experience:
			</div>
			<div>
				<div class="text-left mb-6 mt-6 w-3/4 ml-auto mr-auto text-lg">
					I've worked on several websites and web projects. My core langauges are PHP &amp; JavaScript. I've used these languages to implement standalone projects as well as projects using a framework such as Laravel or VueJS. Here are some examples:
				</div>
				<div class="text-left ml-2 w-5/6 ml-auto mr-auto text-sm mb-12 pt-8 flex flex-col justify-evenly divide-x divide-gray-900 lg:flex-row lg:divide-gray-500">
					<div class="flex flex-col mb-4 lg:mb-0"><a href="https://visudo.me/follow-bot" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Follow-Bot</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">A Discord Bot that automates the process of giving a 'Follower' role to your Twitch Followers.</div></div>
					<div class="flex flex-col mb-4 lg:mb-0"><a href="https://connect-four.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Connect Four</a><div class="w-2/3 m-auto mt-4 mb-4 text-center">A web-based version of the game "Connect-Four" with a VueJS front-end and socket.io back-end.<a href="https://github.com/visudo20179C/connect-four" target="_blank"><img src="../static/GitHub-Mark-Light-32px.png" class="m-auto mt-4"/></a></div></div>
					<div class="flex flex-col"><a href="https://apex-stats.visudo.me/" target="_blank" class="w-2/3 ml-auto mr-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">Apex Stats</a><div class="w-2/3 m-auto mt-4 text-center">A hobby project that was inspired by my love for gaming. This is a "server-less" VueJS project.<a href="https://github.com/visudo20179C/apex-player-stats" target="_blank"><img src="../static/GitHub-Mark-Light-32px.png" class="m-auto mt-4"/></a></div></div>
				</div>
			</div>
			<div class="w-2/3 text-lg text-visudo-green font-black mb-8 mt-4 border rounded-lg bg-gray-900 border-gray-900 text-center mx-auto">
				Open-source contributions:
			</div>
			<div class="w-full mb-8 text-center"><a href="https://apexlegendsstatus.com/discord/" target="_blank" class="mx-auto py-2 px-4 text-visudo-green text-center border-2 rounded-full border-visudo-green text-sm font-black hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 text-lg">ALS Bot</a><div class="w-3/4 mx-auto mt-4 mb-4 text-center">The official Apex Legends Status discord bot.<a href="https://github.com/HugoDerave/als_bot" target="_blank"><img src="../static/GitHub-Mark-Light-32px.png" class="m-auto mt-4"/></a></div></div>
		</div>
		<div class="w-5/6 mx-auto">
			<transition name="fade" mode="out-in">
				<div v-if="!secondShow" key="0">
					<div class="w-2/3 text-xl text-visudo-green font-black mb-8 mt-4 text-center ml-auto mr-auto">
						Types of apps I can create:	
					</div>
					<div class="mx-auto h-3/4 w-3/4 flex flex-col justify-evenly items-top mb-10 pb-10 text-center text-gray-900 font-bold lg:h-80 lg:flex-row">
						<div class="w-1/2 mx-auto border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4">
							<div class="mx-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">Node.js Micro-services</div>
							<img src="../static/Node.js_logo.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="ml-auto mr-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">CRUD applications</div>
							<img src="../static/lara.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="ml-auto mr-auto mt-4 md:text-lg mb-4 text-visudo-green font-black">Single Page Applications</div>
							<img src="../static/Vue.js_Logo_2.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
					</div>
				</div>
				<div v-else-if="secondShow" key="1">
					<div class="w-2/3 text-xl text-visudo-green font-black mb-8 mt-4 text-center ml-auto mr-auto">
						Services I have knowledge using:
					</div>
					<div class="mx-auto h-3/4 w-3/4 flex flex-col justify-evenly items-top mb-10 pb-10 text-center text-gray-900 font-bold lg:h-80 lg:flex-row">
						<div class="w-1/2 mx-auto border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4">
							<div class="mx-auto mt-4 text-lg mb-4 text-visudo-green font-black">Discord</div>
							<img src="../static/js_discord-ar21.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
							<div class="mx-auto mt-4 text-lg mb-4 text-visudo-green font-black">Twitch</div>
							<img src="../static/Twitch_logo.svg" class="m-auto w-2/3 h-2/3 pb-4 lg:pb-0"/>
						</div>
						<div class="w-1/2 mx-auto mt-6 border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 lg:w-1/4 lg:mt-0">
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
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-10 mt-8 text-center mx-auto flex flex-col">
			Twitch Embed/Apex Stats:
			<i class="text-gray-500 text-xs sm:text-sm">Some cool things I can do.</i>
		</div>
		<div class="flex flex-col h-full w-full justify-evenly mb-10 lg:flex-row mx-auto lg:w-3/4">
			<div class="w-5/6 lg:w-1/2 mx-auto mb-4 lg:mb-none">
				<div ref="tVideo"/>
			</div>
			<div class="w-1/2 h-full mb-4 text-center mx-auto">
				<transition name="fade" mode="out-in">
					<div v-if="this.data != null && this.data.Error == null" class="w-2/3 mx-auto text-visudo-green border border-2 rounded-lg border-visudo-green bg-gray-900 transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 py-2" key="0">
						<div class="text-2xl font-bold mb-10">
							Last Played Legend:
						</div>
						<div class="text-2xl font-bold mt-10">
							{{this.data.legends.selected.LegendName}}
						</div>
						<img class="object-contain mx-auto h-48 w-48 mb-4" :src="this.data.legends.selected.ImgAssets.icon"/>
						<p class="mb-4 mx-auto">
							Skin: <i class="text-sm mx-auto">{{this.data.legends.selected.gameInfo.skin}}</i>
						</p>
						<h1 class="text-xl mb-4 mx-auto">Equipped Trackers:</h1>
						<ul>
							<div v-for="item in this.data.legends.selected.data" class="flex flex-col divide-y divide-gray-500 mx-auto">
								<li class="w-5/6 mx-auto">{{item.name}}: {{item.value}}</li>
							</div>
						</ul>
					</div>
					<div v-else-if="this.data != null && this.data.Error != null" class="mx-auto my-auto text-center text-2xl text-visudo-green">
						{{this.data.Error}}
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
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-10 mt-8 text-center mx-auto flex flex-col">
			My GitHub Activity:
			<i class="text-gray-500 text-xs sm:text-sm">(Showing 10 latest commits)</i>
		</div>
		<div v-if="this.gitHubData != null" class="flex flex-col w-full text-gray-500 mb-10">
			<div v-for="(item, index) in this.pushEvents">
				<div class="w-3/4 mx-auto flex flex-col items-center mb-4 lg:flex-row">
					<button>
						<div v-if="item.payload.head" class="text-visudo-green text-center border-2 rounded-full py-1 px-2 border-visudo-green text-sm sm:text-md mr-4">
							{{headRevision(item.payload.head)}}
						</div>
						<div v-else-if="item.payload.pull_request.merge_commit_sha != null" class="text-visudo-green text-center border-2 rounded-full py-1 px-2 border-visudo-green text-sm sm:text-md mr-4">
							{{headRevision(item.payload.pull_request.merge_commit_sha)}}
						</div>
						<div v-else class="text-visudo-green text-center border-2 rounded-full py-1 px-2 border-visudo-green text-sm sm:text-md mr-4">
							{{headRevision(item.payload.pull_request.head.sha)}}
						</div>
					</button>
					<div class="text-visudo-blue mr-4">
						{{item.repo.name}}
					</div>
					<div class="text-xs sm:text-sm">
						<div v-if="item.payload.commits && item.payload.commits.length > 1">
							"{{item.payload.commits.at(-1).message}}"
						</div>
						<div v-else-if="item.payload.commits">
							"{{item.payload.commits[0].message}}"
						</div>
						<div v-else>
							"{{item.payload.pull_request.title}}"
						</div>
					</div>
				</div>
			</div>
		</div>
		<div v-else class="w-full mx-auto mb-10">
			<div class="text-2xl mb-10 mt-10 text-center text-visudo-green">Loading... Please Wait... </div>
			<half-circle-spinner
			  :animation-duration="1000"
			  :size="100"
			  color="#15AB0D"
			  class="m-auto"
			/>
		</div>
		<div class="w-2/3 text-3xl text-visudo-green font-black mb-10 mt-8 text-center mx-auto flex flex-col">
			Service Status:
			<i class="text-gray-500 text-xs sm:text-sm">Displays the status of the services I maintain.</i>
		</div>
		<div v-if="this.statusData != null" class="flex flex-col mb-16 text-visudo-green border border-visudo-green rounded w-1/2 mx-auto px-2 py-2">
			<div class="w-full mx-auto px-2 py-2 text-visudo-green hover:bg-gray-700 hover:text-visudo-blue hover:border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 font-bold rounded-lg" v-for='item in this.statusData'>
				<div v-for='i in Object.keys(item)' class="flex flex-row mb-2">
					<div class="w-full">
						{{i}}
					</div>
					<div v-if='i == "ConnectFourBackend" || i == "FollowBot"'>
						<div v-for='i in item'>
							<div v-if='i == 400 || i == 500'>
								<img class="h-8 w-8 float-right" src="green.png"/>
							</div>
							<div v-else>
								<img class="h-8 w-8 float-right" src="red.png"/>
							</div>
						</div>
					</div>
					<div v-else>
						<div v-for='i in item'>
							<div v-if='i == 200'>
								<img class="h-8 w-8 float-right" src="green.png"/>
							</div>
							<div v-else>
								<img class="h-8 w-8 float-right" src="red.png"/>
							</div>
						</div>
					</div>
				</div>
			</div>
		</div>
		<div v-else class="w-full mx-auto mb-10">
			<div class="text-2xl mb-10 mt-10 text-center text-visudo-green">Loading... Please Wait... </div>
			<half-circle-spinner
			  :animation-duration="1000"
			  :size="100"
			  color="#15AB0D"
			  class="m-auto"
			/>
		</div>
		<div class="w-3/4 text-visudo-green mx-auto mb-10 text-center">
			<div class="mb-4">
				<i>The source code for this wesbite is open-source and proudly made using the </i><a class="text-visudo-blue hover:text-blue-300" href="https://nuxtjs.org/" target="_blank">NuxtJS</a><i> framework</i> 
			</div>
			<iframe src="https://ghbtns.com/github-btn.html?user=visudo20179C&repo=portfolio&type=star&count=true&size=large" frameborder="0" scrolling="0" width="170" height="30" title="GitHub"></iframe>
			</div>
		</div>
	</div>
</template>

<script>
import Twitch from '../lib/twitch.v1.js'
import { HalfCircleSpinner } from 'epic-spinners'
import { Octokit } from '@octokit/core'

export default {
	name: 'Main',
	components: {HalfCircleSpinner, Octokit},
	data() {
		return {
			firstShow: false,
			secondShow: false,
			player: null,
			data: null,
			gitHubData: null,
			statusData: null,
			pushEvents: [],
			mozamKey: process.env.MOZAMRE_API_TOKEN,
			gitHubKey: process.env.GITHUB_ACCESS_TOKEN,
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
			if(data.Error) {
				this.data = {'Error': 'Something went wrong :('}
			}
			else {
				this.data = data
			}
		},
		processStatusData(data) {
			if(data) {
				data.push({'FollowBotBackend': 200})
			}
			else {
				data.push({'Error': 'Invalid API Response.'})
			}
			this.statusData = data
		},
		async makeGitHubRequest() {
			const octokit = new Octokit({auth: this.gitHubKey})
			const gitHubResponse = await octokit.request("GET /users/visudo20179C/events")
			this.gitHubData = gitHubResponse.data
			this.setupPushEvents()
		},
		makeMozamRequest() {
			fetch(
				"https://api.mozambiquehe.re/bridge?version=5&platform=PC&player=visudo20179&auth="+this.mozamKey,
				{
					method: 'GET',
				}
			)
			.then(response => response.json())
			.then(data => this.processData(data))
		},
		makeStatusRequest() {
			fetch(
				"https://follow-bot-backend.plank-and-timber.com/api/status",
				{
					method: 'GET',
				}
			)
			.then(response => response.json())
			.then(data => this.processStatusData(data))
		},
		headRevision(s) {
			return s.substr(0,7)
		},
		setupPushEvents() {
			var count = 0
			this.gitHubData.forEach((elem) => {
				if(this.pushEvents.length == 10) {
					return
				}
				else {
					if(elem.type == 'PushEvent') {
						this.pushEvents.push(elem)
					}
				}
			})
		},
	},
	mounted() {
		const options = {
			width: '66%',
			height: 480,
			channel: 'v1sudo',
		}
		this.player = new Twitch.Player(this.$refs.tVideo, options)
	},
	created() {
		this.makeMozamRequest()
		this.makeGitHubRequest()
		this.makeStatusRequest()
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

