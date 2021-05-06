<template>
	<div class="education-component">
		<h4>{{ major }}</h4>
		<p v-if="dates">{{ dates }}</p>
		<p v-if="school">{{ school }}</p>
		<p v-if="location">{{ location }}</p>
	</div>
</template>

<script>
export default {
	name: 'Education',
	props: {
		major: String,
		dates: String,
		school: String,
		location: String
	}
}
</script>

<style scoped>

</style>