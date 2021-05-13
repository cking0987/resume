<template>
	<div class="header-component">
		<div class="names-and-pronouns-container">
			<h2>{{ name }}</h2>
			<p v-if="nickname" class="text-subtle">But you can call me {{ nickname }}.</p>
			<p v-if="pronouns" class="text-subtle">My pronouns are {{ pronouns }}.</p>
		</div>
		<div class="contact-info-container">
			<h2 v-if="title">{{ title }}</h2>
			<p v-if="phone"><a :href="phoneURL">{{ phone }}</a></p>
			<p v-if="email"><a :href="emailURL">{{ email }}</a></p>
		</div>
	</div>
</template>

<script>
export default {
	name: 'Header',
	props: {
		name: String,
		nickname: String,
		pronouns: String,
		title: String,
		phone: String,
		email: String,
		website: String
	},
	computed: {
		emailURL() {
			return 'mailto:' + this.email
		},
		phoneURL() {
			return 'tel:' + this.phone
		}
	}
}
</script>

<style scoped>

</style>