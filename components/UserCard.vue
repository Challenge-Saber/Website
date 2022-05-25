<script setup>
const props = defineProps({
	name: {
		type: String,
	},
	role: {
		type: String,
	},
	pic: {
		type: String,
	},
	discord: {
		type: String,
	},
	scoresaber: {
		type: String,
	},
	github: {
		type: String,
	},
	steam: {
		type: String,
	},
	twitch: {
		type: String,
	},
	mal: {
		type: String,
	},
});
</script>

<template>
	<div
		class="hover:scale-105 hover:rotate-3 transition-all duration-100 hover:bg-gray-900 max-w-md w-full p-2 rounded-lg"
	>
		<img :src="pic" alt="NahSahh was here." class="m-3 w-24 h-24 float-left rounded-lg" />
		<div class="mt-6">
			<h3>{{ name }}</h3>
			<h4 class="text-blue-200">{{ role }}</h4>
			<div class="flex">
				<a :href="discord">
					<img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/DiscordLogo.png?raw=true"
						class="w-5 h-5 m-1"
					/>
				</a>
				<a v-if="scoresaber" :href="scoresaber"
					><img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/ScoreSaberLogo.png?raw=true"
						class="w-5 h-5 m-1"
				/></a>
				<a v-if="github" :href="github"
					><img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/GithubLogo.png?raw=true"
						class="w-5 h-5 m-1"
				/></a>
				<a v-if="steam" :href="steam"
					><img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/SteamLogo.png?raw=true"
						class="w-5 h-5 m-1"
				/></a>
				<a v-if="twitch" :href="twitch"
					><img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/TwitchLogo.png?raw=true"
						class="w-5 h-5 m-1"
				/></a>
				<a v-if="mal" :href="mal"
					><img
						src="https://github.com/Challenge-Points/Website/blob/1b8ba0a3d98ef08394dfcb348ca9869d1bfb8ded/src/Icons/MyAnimeListLogo.png?raw=true"
						class="w-5 h-5 m-1"
				/></a>
			</div>
		</div>
	</div>
</template>
