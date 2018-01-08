<template lang='pug'>
#app
	.header
		app-header
	.tabs
		app-nav
	.content
		router-view
</template>

<script>
export default {
	components: {
		appHeader: require('./components/Header'),
		appNav: require('./components/Nav')
	}
};
</script>

<style lang="scss">
	#app {
		min-height: 100vh;
		display: flex;
		flex-direction: column;
	}
	.content {
		background: url('./assets/img/bg.jpg') center no-repeat;
		background-size: cover;
	}
</style>