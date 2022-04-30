<template>
	<div>
		<div class="flex ml-16">
			<div class="grid col-span-1 w-full m-2 rounded-lg bg-gray-900">
				<LeaderboardEntry />
				<LeaderboardEntry />
				<LeaderboardEntry />
				<LeaderboardEntry />
				<LeaderboardEntry />
				<LeaderboardEntry />
				<LeaderboardEntry />
			</div>
			<div class="rounded-lg p-2 h-full bg-gray-900 m-2">
				<h1 class="m-1 text-center">
					Latest <i><strong>Video</strong></i>
				</h1>
				<iframe
					width="560"
					height="315"
					src="https://www.youtube.com/embed/6jBmIR4w6hw"
					title="YouTube video player"
					frameborder="0"
					allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
					allowfullscreen
				></iframe>
			</div>
		</div>
	</div>
</template>
