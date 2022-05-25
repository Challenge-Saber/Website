<script setup>
const route = useRoute();

let { data } = useFetch(`${process.env.API_URL}/player/data/${route.params.id}`);
</script>

<template>
	<div>
		<!-- Account Details -->
		<div class="m-auto w-fit p-10">
			<div>
				<img
					:src="data.ProfilePicture"
					alt="i've been trying to contact you about your car's extended warranty"
					class="m-3 w-32 h-32 float-left rounded-full"
				/>
			</div>
			<div class="p-4 text-center">
				<h1>
					<b class="text-blue-500">{{ data.Name }}</b>
					<b class="text-green-600"> #{{ data.RankData[0].Rank }}</b>
				</h1>
				<table>
					<thead>
						<tr>
							<th>
								<img
									src="https://cdn.discordapp.com/emojis/874215132874571787.webp?size=4096&quality=lossless"
									alt="Plastic"
								/>
							</th>
							<th>
								<img
									src="https://cdn.discordapp.com/emojis/874215133197500446.webp?size=4096&quality=lossless"
									alt="Silver"
								/>
							</th>
							<th>
								<img
									src="https://cdn.discordapp.com/emojis/874215133147197460.webp?size=4096&quality=lossless"
									alt="Gold"
								/>
							</th>
							<th>
								<img
									src="https://cdn.discordapp.com/emojis/874215133289795584.webp?size=4096&quality=lossless"
									alt="Diamond"
								/>
							</th>
							<th>
								<img
									src="https://cdn.discordapp.com/emojis/954043083887116368.webp?size=4096&quality=lossless"
									alt="Ruby"
								/>
							</th>
						</tr>
					</thead>
					<tbody>
						<tr>
							<td>{{ data.Trophy.Plastic }}</td>
							<td>{{ data.Trophy.Silver }}</td>
							<td>{{ data.Trophy.Gold }}</td>
							<td>{{ data.Trophy.Diamond }}</td>
							<td>{{ data.Trophy.Ruby }}</td>
						</tr>
					</tbody>
				</table>
				<h2>maybe quote or account links here</h2>
			</div>
		</div>
		<!-- Leaderboards -->
		<div>
			<div class="flex gap-2 mx-2 md:mt-0 mt-3 md:mx-16 pb-12 lg:flex-row flex-col">
				<Leaderboard />
				<Leaderboard />
			</div>
		</div>
	</div>
</template>
