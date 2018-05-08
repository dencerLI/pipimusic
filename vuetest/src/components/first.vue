<template>
	<div id="lun">
		<secondcomponent></secondcomponent>
		<div class="mod_twocol_list mod_twocol_list_normal">
		<h2 class="list_title">电台</h2>
		<ul class="list_img">
		  <li>
		  <img src="../assets/track_radio_199_13_1.jpg" />
		  <span class="list_play"></span>
		  </li>
		  <li>
		    <img src="../assets/track_radio_307_13_1.jpg" />
		    <span class="list_play"></span>
		  </li>
		</ul>
		<h2 class="list_title">热门歌单</h2>
		<ul class="list_img">
		  <li>
		  <img src="../assets/track_radio_199_13_1.jpg" />
		  <span class="list_play"></span>
		  </li>
		  <li>
		    <img src="../assets/track_radio_307_13_1.jpg" />
		    <span class="list_play"></span>
		  </li>
		</ul>
		</div>
	</div>
</template>

<script>
	import secondcomponent from './secondcomponent.vue'
	export default {
		data() {
			return {
				msg: 'vue 真垃圾'
			}
		},
		components: {
			secondcomponent
		}
	}	
</script>

<style>
.mod_twocol_list_normal{
	    margin-bottom: 7px;
}
.mod_twocol_list {
        width: 7rem;
    margin: 0px auto;
}
.mod_twocol_list .list_title {
    font-size: 16px;
    color: #000;
    margin-bottom: 11px;
    /* font-weight: normal; */
   text-align: left;
}
.list_title{ margin-left: 0.1rem;}
.list_img{ height: auto;overflow: hidden; padding: 0; margin: 0; margin-left: -0.1rem;}
.list_img li{ width: 3.3rem; height: 3.3rem; float: left; margin-left: 0.2rem; position: relative;}
.list_img li img{ width: 100%; border: none;}
.list_play{position: absolute; bottom: 0.1rem; right: 0.1rem; background: url(../assets/list_sprite.png) no-repeat; width: 0.54rem; height: 0.54rem; background-size: 100%;}
</style>