<template>
	<div class="work-experience-component">
		<h3>{{ jobTitle }}</h3>
		<div class="work-experience-meta-info">
			<p>{{ dates }}</p>
			<p>{{ location }}</p>
			<p v-if="websiteURL"><a href="websiteURL">{{ websiteLabel }}</a></p>
			<p v-else-if="websiteLabel">{{ websiteLabel }}</p>
		</div>
		<div class="work-experience-description">
			<p>{{ experienceDescription }}</p>
		</div>
	</div>
</template>

<script>
export default {
	name: 'WorkExperience',
	props: {
		jobTitle: String,
		dates: String,
		location: String,
		websiteLabel: String,
		websiteURL: String,
		experienceDescription: String
	}
}
</script>

<style scoped>

</style>