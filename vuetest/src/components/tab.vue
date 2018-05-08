<template>
	<div>
		<nav class="mod_nav">
			<a id="0" v-bind:class="{iscolor:0==guigeSpan}" href="javascript:void(0);" @click="toggleTabs(first);">推荐</a>
			<a id="1" v-bind:class="{iscolor:1==guigeSpan}" href="javascript:void(0);" @click="toggleTabs(second);">排行榜</a>
			<a id="2" v-bind:class="{iscolor:2==guigeSpan}" href="javascript:void(0);" @click="toggleTabs(third);">搜索</a>
		</nav>
		<first :is="currentView" keep-alive></first>
	</div>
</template>

<script type="text/ecmascript-6">
	//导入子组件
	import first from './first.vue';
	import second from './second.vue';
	import third from './third.vue';

	export default {
		data() {
			return {
				first: "first", //导航栏文本1
				second: "second", //导航栏文本2
				third: "third", //导航栏文本3
				currentView: 'first', //默认选中first子组件
				guigeSpan: "0"
			};
		},
		components: {
			first,
			second,
			third
		},
		methods: {
			toggleTabs(tabText) {
				this.currentView = tabText;
				this.guigeSpan = event.currentTarget.id;
			}
		}
	}
</script>
<style scoped>
	a{
		text-decoration: none;
	}
	.mod_nav {
		display: -webkit-box;
		background: #fff;
	}
	
	.mod_nav a {
		-webkit-box-flex: 1;
		position: relative;
		display: block;
		height: 40px;
		line-height: 40px;
		overflow: hidden;
		text-align: center;
		font-size: 16px;
		color: rgba(0, 0, 0, .6);
		-webkit-box-sizing: border-box;
	}
	
	.mod_nav a.iscolor {
		color: #31c27c;
	}
	.mod_nav a.iscolor:after {
    content: "";
    display: block;
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    height: 2px;
    background: #31c27c;
}
</style>