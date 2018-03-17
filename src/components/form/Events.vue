<template>
	<div class="card events-card">
		<header class="card-header">
			<p class="card-header-title">
				Events
			</p>
			<a href="#" class="card-header-icon" aria-label="more options">
				<span class="icon">
					<i class="fa fa-angle-down" aria-hidden="true"></i>
				</span>
			</a>
		</header>
		<div class="card-table">
			<div class="content">
				<table class="table is-fullwidth is-striped">
					<tbody>
						<tr v-for="event in events" :key="event.id" v-if="event.id<5">
							<td width="5%"><i class="fa fa-bell-o"></i></td>
							<td>{{event.title}}</td>
							<td>
								<a class="button is-small is-primary" :href="event.url" target="_blank">Ver</a>
							</td>
						</tr>
					</tbody>
				</table>
			</div>
		</div>
		<footer class="card-footer" v-if="events.length>5">
			<a href="#" class="card-footer-item">View All</a>
		</footer>
	</div>
</template>

<script>
	export default{
		name:'Events',
		props:{},
		data:function(){
			return{
				events:[
					{id:0,title:'Primer evento',url:'#'},
					{id:1,title:'Segundo evento',url:'#'},
					{id:2,title:'Tercer evetnto',url:'#'},
					{id:3,title:'Cuarto evetnto',url:'#'},
					{id:4,title:'Quinto evetnto',url:'#'},
					{id:5,title:'Sexto evetnto',url:'#'}
				]
			}
		}
	}
</script>

<style>
</style>