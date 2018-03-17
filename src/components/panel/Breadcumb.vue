<template>
	<nav class="breadcrumb" aria-label="breadcrumbs">
		<ul>
			<li v-for="(route,index) in routes" :class="index<routes.length-1?'':'is-active'" :key="route.id">
				<a :href="route.url" aria-current="page">{{route.title}}</a>
			</li>
		</ul>
	</nav>
</template>

<script>
	export default{
		name:'Breadcumb',
		props:{},
		data:function(){
			return {
				routes:[
					{id:0,title:'Home',url:'/'},
					{id:1,title:'Pagina 2',url:'/'},
					{id:1,title:'Pagina 3',url:'/'},
				]
			}
		}
	}
</script>

<style>
</style>