<template>
  <div class="leftpanel" id="leftPanel">
	  <div class="logopanel"></div>
		<div class="leftpanelinner">
			<ul class="nav">
				<li v-for="item in navData" :class="[item == key ? active : notactive ]" v-on:click="clickItem(item)">{{item}}</li>
			</ul>
		</div>
	</div>
</template>

<script>

export default {
  name: 'leftPanel',
  data: function(){
		return {
      message: 'hello',
  		navData: [
  			'aaa',
  			'bbb',
  			'ccc',
  			'ddd',
        'eee'
  		],
  		key: 'aaa',
      active: 'active',
      notactive: 'notactive',
    }
	},
	methods: {
		clickItem: function (item) {
			this.key = item;
      this.$emit('change-view', item);
		}
	}
}
</script>

<style>
.leftpanel{
	width: 200px;
	height: 100%;
	background: #2F323A;
	z-index: 100;
	position: absolute;
	top: 0;
	left: 0;
	background: linear-gradient(to bottom,#2F323A 0,#2F323A 100%);
}
.logopanel{
	margin: 0;
	padding: 15px;
	background-color: #2F323A;

}
.leftpanelinner{
	padding: 0;
	z-index: 100;
	position: relative;
}
.nav{
  padding: 0;
  list-style: none;
	margin-bottom: 30px;
}
.nav>li{
	color: #B5B8BF;
	padding: 12px 20px 14px;
	cursor: pointer;
}
.nav>li:hover{
	background-color: rgba(255,255,255,.1);
}
.nav .active{
	border-left: 3px solid #41b2a6;
	color: #fff;
}
.nav .notactive{
  border-left: 3px solid transparent;
}
</style>
