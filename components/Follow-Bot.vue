<template>
<div>
	<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
		What is Follow-Bot?
	</div>
	<div class="w-3/4 text-lg text-visudo-green text-center mx-auto mb-8">
		Follow-Bot is a Discord Bot that can automate giving your Discord users' a role based on who they follow on Twitch.
	</div>
	<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
		Who is it for?
	</div>
	<div class="w-3/4 text-lg text-visudo-green text-center mx-auto mb-8">
		Follow-Bot was created for Twitch streamers, but can be used by anyone who owns a Discord server.
	</div>
	<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
		How does it work?
	</div>
	<div class="w-3/4 text-lg text-visudo-green text-center mx-auto mb-16">
		Simply invite Follow-Bot in your server using the link below, and run the /register command to get started.
	</div>
	<div class="w-1/3 text-2xl text-visudo-blue hover:text-blue-300 hover:border-blue-300 mx-auto text-center border-2 rounded-full py-1 px-2 border-visudo-blue transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-60 mb-16">
		<a href="https://discord.com/api/oauth2/authorize?client_id=889562979614466118&permissions=8&scope=bot" target="_blank">Invite Link</a>
	</div>
	<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
		Follow-Bot server owner only commands:
	</div>
	<div class="w-5/6 mx-auto flex flex-col justify-evenly divide-x divide-gray-900 lg:flex-row lg:divide-gray-500 mb-8">
		<div class="w-2/3 flex flex-col mx-auto">
			<div class="w-2/3 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/register</div>
			<div class="text-sm text-visudo-green lg:mb-2">Registers your server in the Follow-Bot database.</div>
			<div class="text-sm text-visudo-green lg:mb-2">Required Inputs:</div>
			<ul class="text-sm text-visudo-green list-disc mb-4">
				<li>Twitch account name that Follow-Bot should sync against.</li>
				<li>Channel where Follow-Bot should output.</li>
				<li>The role Follow-Bot should give to those who sync.</li>
			</ul>
		</div>
		<div class="w-2/3 flex flex-col mx-auto">
			<div class="w-2/3 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/edit</div>
			<div class="text-sm text-visudo-green lg:mb-2 lg:ml-6">Edits your server configuration in the Follow-Bot database.</div>
			<div class="text-sm text-visudo-green lg:mb-2 lg:ml-6">Required Inputs:</div>
			<ul class="text-sm text-visudo-green list-disc lg:mb-2 lg:ml-6">
				<li>Twitch account name that Follow-Bot should sync against.</li>
				<li>Channel where Follow-Bot should output.</li>
				<li>The role Follow-Bot should give to those who sync.</li>
			</ul>
			<div class="text-xs text-visudo-green mb-4 lg:ml-6"><i>NOTE: Although you might only change one, all three are still required.</i></div>
		</div>
		<div class="w-2/3 flex flex-col mx-auto">
			<div class="w-2/3 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/remove</div>
			<div class="text-sm text-visudo-green lg:mb-2 lg:ml-6">Removes your server from the Follow-Bot database.</div>
			<div class="text-xs text-visudo-green lg:ml-6"><i>NOTE: This is un-doable. Doing so and re-registering will require all your users' to run /authorize again before syncing.</i></div>
		</div>
	</div>
	<div class="w-5/6 mx-auto flex flex-col justify-evenly divide-x divide-gray-900 lg:flex-row lg:divide-gray-500 mb-16">
		<div class="w-2/3 flex flex-col mx-auto mb-4">
			<div class="w-1/3 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/show</div>
			<div class="text-sm text-center text-visudo-green lg:mb-2 lg:ml-6">Prints your Follow-Bot configuration in a message embed.</div>
		</div>
		<div class="w-2/3 flex flex-col mx-auto">
			<div class="w-1/3 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/purge</div>
			<div class="text-sm text-center text-visudo-green lg:mb-2 lg:ml-6">Purges all users' of their Follower role if they no longer follow you on Twitch.</div>
		</div>
	</div>
	<div class="w-5/6 text-3xl text-visudo-green font-black mb-8 mt-16 border rounded-lg border-gray-900 text-center mx-auto">
		Follow-Bot user commands:
	</div>
	<div class="w-2/3 flex flex-col mx-auto">
		<div class="w-1/2 mx-auto border-2 rounded-full py-1 px-2 border-visudo-blue text-center text-lg text-visudo-blue mb-4">/authorize</div>
		<div class="text-md text-visudo-green mx-auto mb-4">Authorizes you to use Follow-Bot in the server you ran the command from.</div>
		<div class="text-sm text-visudo-green mx-auto mb-8"><i>NOTE: After running this command, you still need to sync your role. Click the OAuth2 URL that Follow-Bot created after the server owner registered the server.</i></div>
	</div>
</div>
</template>

<script>
export default {
	name: 'Follow-Bot',
	head: {title: 'Follow-Bot'},
}
</script>

