<template>
	<div class="about-component">
		<p>{{ content }}</p>
	</div>
</template>

<script>
export default {
	name: 'About',
	props: {
		content: String
	}
}
</script>

<style scoped>

</style>