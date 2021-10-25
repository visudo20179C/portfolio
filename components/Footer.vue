<template>
	<div class="w-full flex justify-between h-full bg-gray-900 border-double border-t-8 border-gray-500 sm:h-48 pb-10 pt-10">
		<div class="w-3/4 hidden mt-auto mb-auto ml-4 text-visudo-red border border-2 border-gray-900 md:block">
			{{this.selectedQuote}}
		</div>
		<div class="m-auto text-visudo-green text-center">
			<div class="w-1/2 mx-auto font-bold md:w-3/4">Are you a streamer or other content creator in need of a website or web service? Contact Me:</div>
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
			selectedQuote: null,
			quoteIndex: null,
			quoteOptions: [
				'"When you are following a trail, you are not a trailblazer."',
				'"Some people are so poor, all they have is money."',
				'"A fool admires complexity. A genius admires simplicity."',
				'"In life there are two types of people. Those who live, and those who compare and impress."',
				'"If you\'re not willing to go \'too far\', you\'ll never go far enough."'
			],
		}
	},
	created() {
		this.quoteIndex = 0
		this.selectedQuote = this.quoteOptions[this.quoteIndex]
		setInterval(() => {
			if (this.quoteIndex < this.quoteOptions.length-1) {
				this.selectedQuote = this.quoteOptions[this.quoteIndex+1]
				this.quoteIndex++
			}
			else {
				this.selectedQuote = this.quoteOptions[0]
				this.quoteIndex = 0
			}
		},10000)
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

