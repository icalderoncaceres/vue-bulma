<template>
	<section class="info-tiles">
		<div class="tile is-ancestor has-text-centered">
			<div class="tile is-parent" v-for="dato in data">
				<article class="tile is-child box">
					<p class="title">{{dato.value}}</p>
 					<p class="subtitle">{{dato.und}}</p>
                </article>
			</div>
		</div>
    </section>
</template>

<script>
	export default{
		name:'ResumenSection',
		props:{},
		data:function(){
			return {
				data:[
					{id:0,value:1200,und:'Users'},
					{id:1,value:20,und:'Projects'},
					{id:2,value:30,und:'Course'}

				]
			}
		}
	}
</script>