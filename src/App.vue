<template>
  <div id="app">
    <Header title="VueJS" />
		<Profile :user="user" />
  </div>
</template>

<script>
	import Header from './components/Header';
	import Profile from './components/Profile'

	export default {
		name: 'app',
		components: {
			Header,
			Profile
		},
		data: function () {
			return {
				user: {
					name: 'Alper Silistre',
					image: require('./assets/profile-img.png')
				}
			}
		}
	}

</script>

<style>
body {
	margin: 0;
	background-color: #F3F3F3; 
}

#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
