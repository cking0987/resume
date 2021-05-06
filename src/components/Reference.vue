<template>
	<div class="reference-component">
		<h4>{{ name }}</h4>
		<p v-if="phone">{{ phone }}</p>
		<p v-if="email">{{ email }}</p>
		<p v-if="title">{{ title }}</p>
		<p v-if="relation">{{ relation }}</p>
		<p v-if="dates">{{ dates }}</p>
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
		relation: String,
		dates: String
	}
}
</script>

<style scoped>

</style>
