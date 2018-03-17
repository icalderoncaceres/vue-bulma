<template>
	<aside class="menu">
		<Searcher />
		<section v-for="option in options">
	 		<p class="menu-label" >
	 			{{option.title}}
			</p>
			<ul class="menu-list">
				<li v-for="option2 in option.options">
					<a>{{option2.title}}</a>
					<ul v-if="option2.options.length>0">
						<li v-for="option3 in option2.options">
							<a>{{option3.title}}</a>
						</li>
					</ul>
				</li>
			</ul>
        </section>
	</aside>
</template>

<script>
import Searcher from '../form/Searcher.vue'
export default {
  name: 'VerticalMenu',
  data:function(){
  	return {
  		options:[
  			{
  				id:0,
  				title:'Menú 1',
  				options:[
  					{id:0,title:'Menú 1.1',options:[]},
  					{id:1,title:'Menú 1.2',options:[]},
  					{id:2,title:'Menú 1.3',options:[]}
  				]
  			},
  			{
  				id:1,
  				title:'Menú 2',
  				options:[
  					{id:0,title:'Menú 2.1',options:[]},
  					{
  						id:1,
  						title:'Menú 2.2',
  						options:[
  							{id:0,title:'Menú 2.2.1'},
  							{id:0,title:'Menú 2.2.2'},
  							{id:0,title:'Menú 2.2.3'}
  						]
  					},
  					{id:2,title:'Menú 2.3',options:[]}
  				]
  			},
  			{
  				id:2,
  				title:'Menú 3',
  				options:[
  					{
  						id:0,
  						title:'Menú 3.1',
						options:[
  							{id:0,title:'Menú 3.1.1'},
  							{id:0,title:'Menú 3.1.2'}
  						]
  					},
  					{id:1,title:'Menú 3.2',options:[]},
  					{id:2,title:'Menú 3.3',options:[]}
  				]
  			}
  		]
  	}
  },
  components:{
  	Searcher
  }
}
</script>

<style>
	aside{
		text-align:left;
	}
</style>