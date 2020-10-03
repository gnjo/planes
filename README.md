# planes
```
//usage

let canvas=document.createElement('canvas')
let ctx=canvas.context('2d')
let pm=planes(ctx) //ctx or canvas or null is demo mode 640x320
pm.add('shop',(ctx,o)=>{
o.clear()
o.tick1fps
o.tick20fps
o.tick30fps
o.tick60fps

})

pm.mode('shop,mes',100) //fadetick

funtion animate(){
 requestAnimationFrame(),pm.update()
}


function entry(obj){
 if(!obj){
  let canvas=document.createElement('canvas'),m=300  
  return canvas.width=16*m,canvas.height=9*m,document.body.appendChild(canvas),entry(canvas)
 }
 let ctx=(obj.canvas)?ctx:canvas.getContext('2d')
 ;
 let o={}
 o.ctx=ctx
 o.mode='default'
 o.fading=0
 o.add()
 o.mode()
 o.clear()
 o.update=()=>{
  
 }
 ;
 return o;
}



```
