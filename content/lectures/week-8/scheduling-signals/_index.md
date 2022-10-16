+++
title = "Scheduling Signals and LFOs"
outputs = ["Reveal"]
[reveal_hugo]
custom_theme = "reveal-hugo/themes/robot-lung.css"
margin = 0.2
separator = "##"
+++

# Scheduling Signals

---

## Setting Values

- This will set the value when ever you trigger it

```
oscillator.frequency.value; //returns the current frequency value
oscillator.frequency.value = 100; //sets the value immediately
```

---

## Scheduling Values

- these are used to create [Envelopes](https://github.com/Tonejs/Tone.js/blob/e68fe68e4c4fef5b6eb3771491e9362c5b93579c/Tone/component/envelope/Envelope.ts#L355) in tone, but we can use them on their own

---

## Types of scheduling

- **setValueAtTime** - to schedule a value change at a precise time.
- **linearRampToValueAtTime** - to ramp to a value starting from the previously scheduled value.
- **exponentialRampToValueAtTime** - same as the above, but with an exponential curve instead of a linear curve.

---

- **setTargetAtTime** - unlike the RampValueAtTime methods, in setTargetAtTime, the time attribute is when it should start ramping towards the value instead of arrive at the value. It takes a third parameter which is the time constant at which it will change.
- **setValueCurveAtTime** - sets an array of values which will be evenly invoked over the course of the duration.
- **cancelScheduledValues** - cancels all values after the specified time.

---

## Ramping values

- **linearRampTo** - set a value and a ramp time and the signal will begin linearly ramping towards that value.
- **exponentialRampTo** - same as above but exponential ramp.
- **rampTo** - same interface as the above methods, but will automatically decide to use linear or exponential based on the units of the signal.

---

## Time

- Number: seconds
  - 1.2: 1.2 seconds
- String: synchronized to the Tone.Transport

- ex of setting BPM:

```
Tone.Transport.bpm.value = 80;
//ramp the bpm to 120 over 10 seconds
Tone.Transport.bpm.rampTo(120, 10)
```

---

## Notation time

- Describes time in BPM and time signature relative values.
  - "4n" = quarter note
  - "8t" = eighth note triplet
  - "2m" = two measures
  - "8n." = dotted-eighth note

---

## Relative time

- Prefix any of the above with "+" and it will be interpreted as "the current time plus whatever expression follows"

  - "+1m" = 1 measure from now
  - "+0.5" = half a second from now

---

## scheduling examples

- see [signal](https://tonejs.github.io/docs/14.7.77/Signal) for specifics

<iframe src="https://codesandbox.io/embed/scheduling-examples-9be8ns?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="scheduling examples"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[starter](https://codesandbox.io/s/scheduling-examples-starter-vjcjci?file=%2Fsketch.js)

---

## LFO - Low Frequency Oscillator

### [Learning Synths](https://learningsynths.ableton.com/en/lfos/change-that-repeats)

---

## LFO (Low Frequency Oscillator)

<iframe height="300" style="width: 100%;" scrolling="no" title="PDM Sound - LFO" src="//codepen.io/lsuddem/embed/JxxbMy/?height=300&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/JxxbMy/'>PDM Sound - LFO</a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[starter](https://codepen.io/lsuddem/pen/QYYGmL)

---

## remaking effects with lfos

- we can use an LFO to remake any effect with 'auto' in the name
  - autowah, autopanner, autofilter
  - also tremolo, vibrato
  - fast tremolo is amplitude modulation
  - fast vibrato is frequency modulation

[examples](https://tonejs.github.io/examples/lfoEffects.html)

---

## Autofilter and Autopan

<iframe height="300" style="width: 100%;" scrolling="no" title="PDM Sound - Autofilter, autowah, autopanner remake" src="//codepen.io/lsuddem/embed/VgNOVb/?height=300&theme-id=35490&default-tab=result" frameborder="no" allowtransparency="true" allowfullscreen="true">
  See the Pen <a href='https://codepen.io/lsuddem/pen/VgNOVb/'>PDM Sound - Autofilter, autowah, autopanner remake</a> by LSU DDEM
  (<a href='https://codepen.io/lsuddem'>@lsuddem</a>) on <a href='https://codepen.io'>CodePen</a>.
</iframe>

[starter](https://codepen.io/lsuddem/pen/ErzeKo?editors=1011)
