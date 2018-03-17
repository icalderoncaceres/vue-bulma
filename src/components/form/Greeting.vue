<template>
	<section class="hero is-info welcome is-small">
		<div class="hero-body">
			<div class="container">
				<h1 class="title">
					Hello, {{user}}.
				</h1>
				<h2 class="subtitle">
					{{message}}
				</h2>
			</div>
		</div>
	</section>
</template>

<script>
	export default{
		name:'Greeting',
		props:['user','message']
	}
</script>

<style>
</style>