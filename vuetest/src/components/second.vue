<template>
	<div id="listme">
    <div class="list_pai">
    	<div class="list_content" v-for="todo in 15">
    		<div class="list_content_left">
    			<img src="../assets/toplist_4_300_213836602.jpg" />
    		</div>
    		<div class="list_content_right">
    			<h3>巅峰榜·流行指数</h3>
    			<p>1<span class="name">哼</span><span class="inname">- 冯提莫</span></p>
    			<p>2<span class="name">圆梦一代</span><span class="inname">- 王俊凯</span></p>
    			<p>3<span class="name">Bloom</span><span class="inname">- Troye Sivan</span></p>
    			<i class="topic_arrow"></i>
    		</div>
    	</div>
    </div>
  </div>
</template>

<script>
</script>

<style scoped>
	.list_pai{ width: 6.8rem; height: auto;overflow: hidden; margin: 0px auto;}
	.list_content{ width: 100%; height: auto;overflow: hidden; background: #ffffff; margin-top: 0.2rem;}
	.list_content_left{ float: left; width: 1.8rem; height: 1.8rem;}
	.list_content_left img{ width: 100%; height: 100%;}
	.list_content_right{ float: right; width: 4.6rem; position: relative;}
	.list_content_right h3{ font-size: 0.3rem; text-align: left; height: 0.5rem;color: #000; margin-top: 0.1rem;}
	.list_content_right p{ font-size: 0.15rem; text-align: left; height: 0.35rem; line-height: 0.35rem;}
    .name{ margin: 0px 5px;color: #000;}
    .inname{color: rgba(0,0,0,.5);}
    .topic_arrow {
    position: absolute;
    right: 10px;
    top: 50%;
    margin-top: -4px;
    width: 6px;
    height: 6px;
    border-right: 1px solid #b2b2b2;
    border-bottom: 1px solid #b2b2b2;
    -webkit-transform: rotate(-45deg);
}
</style>