<template>
	<div class="container">
		<div class="header">
			<div class="side-bar">
				<router-link to="/new_task">新建任务</router-link>
				<router-link to="/mind_task">头脑风暴</router-link>
				<router-link to="/team_task">团队任务</router-link>
			</div>
		</div>
		<div class="content">
			<router-view />
		</div>
	</div>
</template>

<script>
	export default {
		name: 'UCenter',
		data() {
			return {};
		}
	};
</script>

<style scoped>
	.container {

		width: 90%;
		margin: 0 auto;

	}
	.header{
		display:flex;
	}

	.side-bar {
		flex: 1 1 20%;;
		flex-direction: column;
		background-color: #fff;
		margin-top: 20px;
		width:90%;
	}

	a {
		margin-bottom: 30px;
	}

	.content {
		flex: 1 1 80%;
		text-align: left;
		background-color: #fff;
		margin-left: 20px;
		padding-bottom: 20px;
		width:90%;
	}
</style>
