<template>
	<!-- App container -->
	<div class="app">
		<app-header></app-header>
		<app-main></app-main>
		<app-action :action-title="actionTitle"></app-action>
	</div>
</template>

<script>
import Header from './components/tarifCard/header/Header.vue';
import Main from './components/tarifCard/main/Main.vue';
import Action from './components/tarifCard/action/Action.vue';

export default {
  name: 'app',
  components: {
    'app-header': Header,
	'app-main': Main,
	'app-action': Action,
  },
  data() {
	return {
		actionTitle: "Connect now"
	}
  }
}
</script>

<style>
.app {
	box-sizing: content-box;
	font-family: Roboto, sans-serif;
}
</style>
