<template>
<uni-shadow-root class="lib-qrcode-index"><canvas class="wux-class" :canvas-id="canvasId" :style="'width: '+(width + 'px')+'; height: '+(height + 'px')+';'" @click="onTap"></canvas></uni-shadow-root>
</template>

<script>

global['__wxRoute'] = 'lib/qrcode/index'
"use strict";var _index=_interopRequireDefault(require("./qr.js/index"));function _interopRequireDefault(t){return t&&t.__esModule?t:{default:t}}var utf16to8=function(t){for(var e=t.length,r="",o=0;o<e;o++){var i=t.charCodeAt(o);1<=i&&i<=127?r+=t.charAt(o):(2047<i?(r+=String.fromCharCode(224|i>>12&15),r+=String.fromCharCode(128|i>>6&63)):r+=String.fromCharCode(192|i>>6&31),r+=String.fromCharCode(128|i>>0&63))}return r};Component({properties:{typeNumber:{type:Number,value:-1,observer:function(t){this.draw({typeNumber:t})}},errorCorrectLevel:{type:Number,value:2,observer:function(t){this.draw({errorCorrectLevel:t})}},width:{type:Number,value:200,observer:function(t){this.draw({width:t})}},height:{type:Number,value:200,observer:function(t){this.draw({height:t})}},fgColor:{type:String,value:"black",observer:function(t){this.draw({fgColor:t})}},bgColor:{type:String,value:"white",observer:function(t){this.draw({bgColor:t})}},canvasId:{type:String,value:"wux-qrcode"},data:{type:String,value:"",observer:function(t){this.draw({data:t})}}},methods:{draw:function(t){var a=this,e=0<arguments.length&&void 0!==t?t:{},r=Object.assign({},this.data,e),o=r.typeNumber,i=r.errorCorrectLevel,n=r.width,u=r.height,h=r.fgColor,c=r.bgColor,l=r.canvasId,d=r.data,s=(0,_index.default)(utf16to8(d),{typeNumber:o,errorCorrectLevel:i}).modules,f=n/s.length,v=u/s.length;this.ctx=this.ctx||wx.createCanvasContext(l,this),this.ctx.scale(1,1),s.forEach(function(t,i){t.forEach(function(t,e){a.ctx.setFillStyle(t?h:c);var r=Math.ceil((e+1)*f)-Math.floor(e*f),o=Math.ceil((i+1)*v)-Math.floor(i*v);a.ctx.fillRect(Math.round(e*f),Math.round(i*v),r,o)})}),this.ctx.draw()},onTap:function(){this.triggerEvent("click")}},attached:function(){this.draw()},detached:function(){this.ctx=null}});
export default global['__wxComponents']['lib/qrcode/index']
</script>
<style platform="mp-weixin">

</style>