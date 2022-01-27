//cloudy circles
//by vadim_art
noise(3,1)
  .add(voronoi(1.9,0.09,4),30)
  .mult(src(o2).rotate([-0.05,0.05],1))
  .mult(src(o1).modulateRepeat(osc(50), 5.0, ({time})=>Math.sin(time)*5))
  .rotate(({time})=>(time%360)/2,0.9)
  .modulateRotate(o0, 200.2)
  .out(o0)

noise(400,0.2)
  .colorama(({time})=>Math.sin(time/20) )
.out(o1)

shape(1,1)
  .mult(osc(8,0.25,0.5))
.out(o2)

render(o0)
