<template>
	<div class="flex justify-between h-48 bg-gray-900 border-double border-t-8 border-gray-500">
		<div class="mt-auto mb-auto ml-4 text-visudo-red border border-2 border-gray-900">
			{{quoteCompute}}
		</div>
		<div class="mt-auto mb-auto mr-8 text-visudo-green text-center">
			<div class="font-bold">Are you a streamer or other content creator in need of a website or web service? Contact Me:</div>
			<ul class="mt-4">
				<li>Email:  cjkbusiness96@gmail.com</li>
				<li>Discord: visudo#0318 </li>
			</ul>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Footer',
	data() {
		return {
			quoteOptions: [
				'"When you are following a trail, you are not a trailblazer."',
				'"Some people are so poor, all they have is money."',
				'"A fool admires complexity. A genius admires simplicity."',
				'"In life there are two types of people. Those who live, and those who compare and impress."'
			],
		}
	},
	computed: {
		quoteCompute() {
			return this.quoteOptions[Math.floor(Math.random()*this.quoteOptions.length)]
		}
	}
} 
</script>

