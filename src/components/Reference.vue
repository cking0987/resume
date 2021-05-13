<template>
	<div class="reference-component">
		<h3>{{ name }}</h3>
		<p><a :href="requestContactInfoURL" target="_blank" rel="noreferrer">Request contact info</a></p>
		<!--
		<p v-if="phone" class="overline"><a :href="phoneURL">{{ phone }}</a></p>
		<p v-if="email" class="overline"><a :href="emailURL">{{ email }}</a></p>
		-->
		<p v-if="title" class="overline text-high-emphasis">{{ title }}</p>
		<p v-if="dates" class="overline">{{ dates }}</p>
	</div>
</template>

<script>
export default {
	name: 'Education',
	props: {
		name: String,
		phone: String,
		email: String,
		title: String,
		dates: String
	},
	computed: {
		phoneURL: function() {
			return 'tel:' + this.phone;
		},
		emailURL: function() {
			return 'mailto:' + this.email;
		},
		requestContactInfoURL: function() {
			let dest = 'cking0987@gmail.com'
			let subj = 'Request for references contact info'
			let bod = 'Hi Chuck! I came across your resume and wanted to reach out to your references. Could you provide me with their contact info? Thanks!'
			return 'mailto:' + dest + '?subject=' + encodeURIComponent(subj) + '&body=' + encodeURIComponent(bod)
		}
	}
}
</script>

<style scoped>

</style>
