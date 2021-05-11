<template>
	<div class="reference-component">
		<h3>{{ name }}</h3>
		<p v-if="phone" class="overline"><a :href="phoneURL">{{ phone }}</a></p>
		<p v-if="email" class="overline"><a :href="emailURL">{{ email }}</a></p>
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
		}
	}
}
</script>

<style scoped>

</style>
