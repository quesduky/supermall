<template>
	<swiper class="swipers">
		<swiper-item v-for="(item,index) in topImages" :key="index">
			<img :src="item" alt="">
		</swiper-item>
	</swiper>
</template>

<script>
	import {Swiper,SwiperItem} from '../../../components/common/swiper'
	export default{
		name:"DetailBanner",
		components:{
			Swiper,
			SwiperItem
		},
		props:{
			topImages:{
				type:Array,
				default(){
					return []
				}
			}
		}
	}
</script>

<style>
	.swipers{
		height: 320px;
	}
</style>
