<template>
	<div>
		<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
			Thank you for using Follow-Bot!
		</div>
		<div class="w-3/4 text-lg text-visudo-green text-center mx-auto mb-4">
			You have successfully synced your role using Follow-Bot.
		</div>
		<div class="w-3/4 text-lg text-visudo-green text-center mx-auto mb-16">
			Please see some of the resources below if you'd like more information about Follow-Bot.
		</div>
		<div class="w-3/4 h-5/6 mx-auto flex flex-col justify-evenly divide-x lg:flex-row divide-gray-900 mb-24">
			<div class="mx-auto mb-8 text-xs lg:text-md transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60"><a href="https://visudo.me/follow-bot" target="_blank" class="w-2/3 mx-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green hover:text-visudo-blue hover:border-visudo-blue text-lg">Follow-Bot Home</a></div>
			<div class="mx-auto mb-8 text-xs lg:text-md transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60"><a href="https://visudo.me/follow-bot/tos" target="_blank" class="w-2/3 mx-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green hover:text-visudo-blue hover:border-visudo-blue text-lg">Follow-Bot TOS</a></div>
			<div class="mx-auto text-xs lg:text-md transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60"><a href="https://visudo.me/follow-bot/privacy" target="_blank" class="w-2/3 mx-auto text-visudo-green text-center border-2 rounded-full py-1.5 px-3 border-visudo-green hover:text-visudo-blue hover:border-visudo-blue text-lg">Privacy Policy</a></div>
		</div>
		<div class="w-5/6 text-3xl text-visudo-green font-black mb-4 border rounded-lg border-gray-900 text-center mx-auto">
			Why did my role not sync?
		</div>
		<div class="w-5/6 text-lg text-visudo-green mb-24 text-center mx-auto">
			Make sure you run /authorize in the server right before you click the sync URL that the bot generated.
		</div>
		<div class="w-5/6 text-lg text-visudo-green mb-24 text-center mx-auto font-black">
			If you like Follow-Bot, consider adding it to your own Discord server via the Invite Link on the main page.
		</div>
		<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 border rounded-lg border-gray-900 text-center mx-auto">
			Learn more about me on the home page:
		</div>
		<div class="w-24 mx-auto mb-16">
			<a href="https://visudo.me/">
				<svg xmlns="http://www.w3.org/2000/svg" class="h-24 w-24 text-visudo-green mx-auto" fill="none" viewBox="0 0 24 24" stroke="currentColor">
					<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6" />
				</svg>
			</a>
		</div>
		<div class="w-5/6 text-lg text-visudo-green mb-24 text-center mx-auto">
			I make websites, web services, discord bots and much more.
		</div>
	</div>
</template>

<script>
export default {
	name: 'Follow-Bot-Thank-You',
	head: {title: 'Thank You'},
}
</script>
