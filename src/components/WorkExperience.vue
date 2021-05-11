<template>
	<div class="work-experience-component">
		<hr align="left" />
		<div class="title-and-dates">
			<h3>{{ jobTitle }}</h3>
			<div class="overline inline">{{ dates }}</div>
		</div>
		<div class="work-experience-meta-info">
			<div class="overline text-high-emphasis">{{ employerName }}</div>
			<div class="overline">{{ location }}</div>
			<div v-if="websiteURL" class="overline"><a :href="websiteURL" target="_blank" rel="noreferrer">{{ websiteLabel }}</a></div>
			<div v-else-if="instagram" class="overline"><a :href="instagramURL" target="_blank" rel="noreferrer"><IconInstagram />{{ instagram }}</a></div>
		</div>
		
		<div class="work-experience-description">
			<p>{{ experienceDescription }}</p>
		</div>
	</div>
</template>

<script>
import IconInstagram from './icons/IconInstagram.vue'

export default {
  components: { IconInstagram },
	name: 'WorkExperience',
	props: {
		jobTitle: String,
		dates: String,
		employerName: String,
		location: String,
		instagram: String,
		websiteLabel: String,
		websiteURL: String,
		experienceDescription: String
	},
	computed: {
		instagramURL: function() {
			return 'http://www.instagram.com/' + this.instagram;
		}
	}
}
</script>

<style scoped>

</style>
