<script setup>
const props = defineProps({
	itemName: {
		type: String,
	},
	to: {
		type: String,
	},
});
</script>

<template>
	<div class="hover:bg-gray-400 p-2 rounded-xl w-full text-center hover:bg-opacity-10">
		<NuxtLink :to="to">
			<h1>{{ itemName }}</h1>
		</NuxtLink>
	</div>
</template>
