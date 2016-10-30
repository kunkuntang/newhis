<template>
  <div class="mainView" id="viewContainer">
    <component :is="curView" @choose-item="changeView(view)"></component>
  </div>
</template>

<script>
import clinic from './clinic'
import checkin from './checkin'

export default {
  name: 'viewContainer',
  props: ['curView'],
  data: function(){
		return {
      view: 'clinic'
    }
	},
	methods: {
		changeView: function (view) {
			this.view = view;
		}
	},
  components: {
    clinic,checkin
  }
}
</script>

<style>
.mainView{
  height: auto;
  width: auto;
  margin-left: 200px;
}

</style>
