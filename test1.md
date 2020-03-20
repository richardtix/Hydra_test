osc(15, 0.1, 76).out(o1)
osc(18, 1, 15).rotate(-2).pixelate(7, 15).out(o1)
s0.initCam() // initialize a webcam in source buffer s0
src(s0).kaleid(20).out() // render the webcam to a kaleidoscope
osc(15, 0.2, 99).diff(o0).out(o1)
render (o1)
