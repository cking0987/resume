<template>
	<div class="header-component">
		<div class="names-and-pronouns-container">
			<h2>{{ name }}</h2>
			<p v-if="nickname">But you can call me {{ nickname }}</p>
			<p v-if="pronouns">My pronouns are {{ pronouns }}</p>
		</div>
		<div class="contact-info-container">
			<p v-if="title">{{ title }}</p>
			<p v-if="phone">{{ phone }}</p>
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
		emailURL () {
			return 'mailto:' + this.email
		}
	}
}
</script>

<style scoped>

</style>