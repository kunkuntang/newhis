<template>
  <div>
    <div class="headerBar">
      <a class="menutoggle ">
        <i class="fa fa-bars"></i>
      </a>
      <div class="menuinfo">
        <ul class="headermenu">
          <li class="btn-group">
            <span class="">
              <svg xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink" width="31" height="32" viewBox="0 0 31 32">
                <image id="iconfont-service" width="31" height="32" xlink:href="data:img/png;base64,iVBORw0KGgoAAAANSUhEUgAAAB8AAAAgCAQAAABAi2vKAAAABGdBTUEAALGPC/xhBQAAACBjSFJNAAB6JgAAgIQAAPoAAACA6AAAdTAAAOpgAAA6mAAAF3CculE8AAAAAmJLR0QAAKqNIzIAAAAJcEhZcwAACxIAAAsSAdLdfvwAAAAHdElNRQfgCRMRKwNnsU62AAAC1UlEQVQ4y43Uf2iVVRzH8de9d4lMSSzCTPIfc4t0kNtDsTWKjMlEFtScWVJR2IwSAlvQcKvAEvsBMSMGsSIJSUdkJpLTiCbVyk7LX5WCuUXRkM1kC4dzW+uPXdnu3b27fv55zvk+3/dzns/ncE6sRAbdosa9lpqPy84K9vs8DE5tjE3Bi2y1SmxK5wXbvZH+iVQ8oVGDBM47qF23IddZokKZBLo9Ejqy4fk+dj+6NGo1PF4MIFqgzkZ5hj0WdmXCE/aoQovnDJqtXKl5ZrrgjG/CMaLbtVrsPzXh06n4Fg2ot83NNltndorJ37ztA3O1KXZRSTidihc7IqHZMzZ6XX6m7XDUw/7RaYHvlIexyXibFU5Zpkmt7Or3gIRDeDDsgThYagVe9Oq0MHN8pteX2DReGMfX4XejnpdL19ptO8qjhRP4fWjzbk4YCkUG8FZUQaxkkV0ifGX5NNAOl2xIjvv8aRmoj5UcVHEVa9ba7azr06OMi64C7rYzDHhtapTxpPvpdFxlGESLi+mv8rJClxzzs07fhxPjhfBv1OqJXPiIHQ77ySmjXDkySe3LhY+pcmAaG2lKd/7FNDC9afPBuB9TCmemyzAMJAc9yed7cet9ixO2gUK51afIO2hWl+cP5WCGGouUyzeYjYvmgzfD+egM3g+jE94vexazrE3Or5mErY4eAmX4VVMU87hunanJt9miUYOdhrDVjToNRwWWm+tW8JR+q8NQVK3YpjBG4qbJf/e1WVaZ6RDalalX5U6nVYceomobrAxHo3n2OufJ2pFM9/yjmtT6BMxR6O/wF0SlXvF06IpucMAS94QfMu07HymwMOm835FxGN0qQ1dUqkORNeNwptUnNEOlPPvDUDLAAnXWO2dtaL/Skh2PO+wudFhjsTusdLcRLV4KfRNN2fHb/JIyP26v5tCT2pT9wPYalcCoF5x0Mh3Mjdd6WZ7N4cPs8fwPmRjg6hH9aX8AAAAASUVORK5CYII="></image>
              </svg>
            </span>
          </li>
          <li class="btn-group"></li>
          <li class="btn-group"></li>
        </ul>
      </div>
    </div>
    <div class="headerTittle">
      <h2>
        <i class="fa fa-user-md"></i>
        {{tittle}}
      </h2>
    </div>
  </div>

</template>

<script>

export default {
  name: '',
  props: ['a'],
  data: function(){
		return {
      tittle: "医生门诊"
    }
	},
	methods: {

	},
  components: {

  }
}
</script>

<style>
.headerBar{
  background-color: #f3f3f4;
  border-left: 1px solid #e7eaec;
  overflow: hidden;
}
.menutoggle{
  float: left;
  width: 50px;
  height: 50px;
  font-size: 1.6rem;
  color: #1d2939;
  cursor: pointer;
  border-right: 1px solid #e7eaec;
  -moz-transition: all .2s ease-out 0s;
  -webkit-transition: all .2s ease-out 0s;
  transition: all .2s ease-out 0s;
}
.menutoggle .fa{
  margin: 14px 0 0 15px;
}
.menuifo{
  float: right;
}
.menuinfo>ul{
  list-style: none;
}
.menuinfo>ul>li{
  float: right;
}
.headerTittle{
  padding: 10px 15px;
  border-bottom: 1px solid #e7eaec;
  border-top: 1px solid #e7eaec;
  position: relative;
  background: #fff;
}
.headerTittle .fa{
  font-size: 16px;
  margin-right: 5px;
  padding: 6px 8px;
  border: 2px solid #1d2939;
  border-radius: 60px;
}
.headerTittle h2{
  font-size: 1.8rem;
  color: #1d2939;
  letter-spacing: -4px;
  margin: 0;
}
</style>
