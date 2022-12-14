+++
title = "Sequencing - 2"
outputs = ["Reveal"]
[reveal_hugo]
custom_theme = "reveal-hugo/themes/robot-lung.css"
margin = 0.2
separator = "##"
+++

## Rain on a tin roof

<iframe src="https://codesandbox.io/embed/rain-on-a-tin-roof-0ylzwl?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Rain on a tin roof"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[starter](https://codesandbox.io/s/rain-on-a-tin-roof-start-cmb2jk?file=%2Fsketch.js)

---

## Part

- collection Tone.Events which can be started/stopped and looped as a single unit.

<iframe src="https://codesandbox.io/embed/tone-transport-part-gcel2p?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Tone.Transport - Part"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[starter](https://codesandbox.io/s/tone-transport-part-starter-gcijvf?file=%2Fsketch.js)

---

## Sequence

- alternate notation of a part

<iframe src="https://codesandbox.io/embed/tone-transport-sequence-msq1lw?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Tone.Transport - Sequence"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[starter](https://codesandbox.io/s/tone-transport-sequence-start-w4smpu?file=%2Fsketch.js)

---

## Loop

- an event that loops by default
- notes can not be passed in like event though
- it's good for looping things that aren't note based
- lets redo out rain example with Loop

---

# Rain loop

<iframe height="400" style="width: 100%;" scrolling="no" title="Tone.loop with Rain on a tin roof " src="//codepen.io/lsuddem/embed/VRLOwb/?height=317&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/VRLOwb/'>Tone.loop with Rain on a tin roof </a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[starter](https://codepen.io/lsuddem/pres/VRLOQy?editors=0010)

---

## Pattern

- play through note arrays like sequence or part
- arpeggiate based on Tone.CtrlPattern type
- see: [docs](https://tonejs.github.io/docs/r13/CtrlPattern)
- CtrlPattern types
  - up, down, upDown, downUp, alternateUp, alternateDown, random, randomWalk

---

<iframe height="490" style="width: 100%;" scrolling="no" title="Tone.Transport - Pattern" src="//codepen.io/lsuddem/embed/NJGPyy/?height=300&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/NJGPyy/'>Tone.Transport - Pattern</a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

---

## Sound Effect

---

## Massive impact

<iframe height="490" style="width: 100%;" scrolling="no" title="Massive Impact" src="//codepen.io/lsuddem/embed/moyYbx/?height=300&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/moyYbx/'>Massive Impact</a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[starter](https://codepen.io/lsuddem/pres/eXNXMy?editors=0010)

---

## Sirens

<iframe height="490" style="width: 100%;" scrolling="no" title="Sirens" src="//codepen.io/lsuddem/embed/oVXyaE/?height=300&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/oVXyaE/'>Sirens</a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[starter](https://codepen.io/lsuddem/pres/jJPJoL?editors=0010)
