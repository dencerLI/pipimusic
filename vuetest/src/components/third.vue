<template>
	<div id="listme">
    <div class="search">
    	<span class="search_icon"></span>
    	<input type="text" placeholder="搜索歌曲、歌单、专辑"/>
    </div>
    <div class="Label">
    	<span class="lable_con" v-for="n in 20">父亲写的散文诗</span>
    </div>
  </div>
</template>

<script>
</script>

<style>
	.search{width: 6.8rem; height:0.8rem; margin: 0px auto; background: #fff; margin-top: 0.2rem;}
	.search input{ width: 4.8rem; height: 100%; float:left;border: none;outline: none; text-indent: 10px;}
	.search_icon{ float: left; width: 0.4rem; height: 0.4rem; margin:0.2rem 0px 0px 0.5rem; background: url(../assets/ss.png) no-repeat; background-size: 100%;}
    .Label{ width: 100%; height: auto;overflow: hidden; background: #fff; margin-top: 0.2rem; padding: 0.2rem;}
    .lable_con{ float: left; padding: 5px 12px; border: 1px solid #B2B2B2; border-radius: 20px; font-size: 0.2rem; margin: 0px 0px 0.2rem 0.2rem;}
</style>