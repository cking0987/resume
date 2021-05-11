<template>
	<div class="skills-component">
		<ul>
			<li v-for="skill in skills" :key="skill" class="overline">{{ skill }}</li>
		</ul>
	</div>
</template>

<script>
export default {
	name: 'Skills',
	props: {
		skills: Array
	}
}
</script>

<style scoped>

</style>