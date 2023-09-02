<script setup>
import ChatBot from '@/components/ChatBot.vue'
</script>

<template>
  <div class="wrapper">
    <ChatBot />
  </div>
</template>

<style lang="scss">
@use '@/assets/_variables.scss' as *;

@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
	background: linear-gradient(-45deg, #ee7752, #e73c7e, #23a6d5, #23d5ab);
	background-size: 400% 400%;
	animation: gradient 15s ease infinite;
}

@keyframes gradient {
	0% {
		background-position: 0% 50%;
	}
	50% {
		background-position: 100% 50%;
	}
	100% {
		background-position: 0% 50%;
	}
}

.wrapper {
  padding-inline: 1rem;
}

.styled-scrollbars {
  --scrollbar-size: 7px;
}
.styled-scrollbars::-webkit-scrollbar {
  border-radius: 5px;
  width: var(--scrollbar-size);
  height: var(--scrollbar-size);
}
.styled-scrollbars::-webkit-scrollbar-thumb {
  border-radius: 5px;
  background: $grey;
}
.styled-scrollbars::-webkit-scrollbar-track {
  border-radius: 5px;
  background: $bg-secondary;
}
</style>
