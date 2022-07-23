<!-- Home -->
<template>
	<div class="home-container">
		<div class="warpper">
			<h1 class="demo-home__title">
				<!-- <img src="https://imgs.solui.cn/weapp/logo.png" /> -->
				<span>vite2 VUE3 H5开发模板</span>
			</h1>
			<h2 class="demo-home__desc">A vue h5 template with Vant UI</h2>
		</div>
		<van-cell icon="success" v-for="item in list" :key="item" :title="item" />
	</div>
</template>
<script lang="ts" setup>
// import { defineComponent } from 'vue'
// import { UserDevelopRecordList } from '@/api/authController'
// import { useAuthStore } from '@/store/auth';
// onMounted(() => {
	// token
// 	state.params = window.location.href
// 	if(!userStore.token){
// 		state.token = window.location.href.split('=')[1];
// 	}else {
// 		state.token =userStore.token
// 	}
	
// 	console.log(state.token)
// 	userStore.saveToken(state.token);
// 	getUserDevelopRecordList();
// });

// const getUserDevelopRecordList = () => {
// 	UserDevelopRecordList({ page: 1, limit: 10 }).then(res=> {
// 		console.log(res, 'kk');
// 		Toast.loading({
//  		 message: '加载中...',
//   		forbidClick: true,
// });
// 		state.list = res.data.list
	// })
		

</script>
<style lang="scss" scoped>
.home-container {
	.warpper {
		padding: 12px;
		background: #fff;
		.demo-home__title {
			margin: 0 0 6px;
			font-size: 28px;
			.demo-home__title img,
			.demo-home__title span {
				display: inline-block;
				vertical-align: middle;
			}
			img {
				width: 32px;
			}
			span {
				margin-left: 16px;
				font-weight: 500;
			}
		}
		.demo-home__desc {
			margin-top: 10px;
			// margin: 0 0 10px;
			color: rgba(69, 90, 100, 0.6);
			font-size: 14px;
		}
	}
}
</style>
