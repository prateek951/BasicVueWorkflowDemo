<template>
	<div>
		<h1>{{message}}</h1>
		<app-input :msg = "message" @messageChanged="message = $event"></app-input>
	</div>
</template>

<script>
	import input from './input'
	export default {
		data() {
			return {
				message: 'This is a great message'
			}
		},
		components: {
			'app-input' : input
		}
	}
</script>

