<template>
  <div class="flex gap-2 mx-2 md:mt-0 mt-3 md:mx-16 pb-12 lg:flex-row flex-col">
    <div class="w-full rounded-lg bg-gray-900">
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
      <LeaderboardEntry />
    </div>
    <div class="rounded-lg max-h-80 p-2 bg-gray-900 w-full max-w-lg">
      <h1 class="p-2 text-center text-gray-300 italic font-bold">
        Latest Video
      </h1>
      <div className="bg-red-200">
        <iframe
          class="max-w-lg w-full h-64"
          src="https://www.youtube.com/embed/6jBmIR4w6hw"
          title="YouTube video player"
          frameborder="0"
          allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
          allowfullscreen
        />
      </div>
    </div>
  </div>
</template>
