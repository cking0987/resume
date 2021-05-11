<template>
	<div class="education-component">
		<h3>{{ major }}</h3>
		<p v-if="dates" class="overline">{{ dates }}</p>
		<p v-if="school" class="overline text-high-emphasis">{{ school }}</p>
		<p v-if="location" class="overline">{{ location }}</p>
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