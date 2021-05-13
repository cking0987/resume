<template>
	<div class="cert-component">
		<a href="https://bcert.me/sqpetblny" target="_blank" rel="noreferrer">
			<img :src="imgPath" alt="Certified Scrum Product Owner">
		</a>
	</div>
</template>

<script>
export default {
	name: 'CSPO',
	data () {
		return {
			imgPath: require("@/assets/CSPO.png")
		}
	}
}
</script>

<style scoped>
img {
	width: 75%;
}
</style>