<template>
	<div class="list-item editingClass editing">
		<label class="checkbox">
			<input type="checkbox" v-model="item.checked" />
			<span class="checkbox-custom"></span>
		</label>
		<input type="text" v-model="item.text" placeholder='写点什么...' />
		<a class="detele-item">
			<span class="icon-trash"></span>
		</a>
	</div>
</template>


<script>
export default{
	props:{
		item:{
			type:Object,
			default:() => {
				return{
					checked:false,
					text:'你好，世界'
				}
			}
		}
	}
};
</script>



<style lang="less">
	@import '../common/style/list-items.less';
</style>