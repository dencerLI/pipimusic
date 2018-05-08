<template>
	<div class="mod_header">
		<i class="music_logo">QQ音乐</i>
	</div>
</template>

<script>
	export default {
		data() {
			return {
				author: "微信公众号 jinkey-love"
			}
		}
	}
	
</script>

<style>
	.mod_header {
		position: relative;
		height: 44px;
		background: #31c27c;
	}
	
	.mod_header .music_logo {
		float: left;
		display: block;
		width: 90px;
		height: 25px;
		margin: 9px 0 0 10px;
		background-image: url(../assets/logo1.png);
		background-size: cover;
		background-repeat: no-repeat;
		text-indent: -9999px;
	}
</style>