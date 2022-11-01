+++
title = "Sequencing"
outputs = ["Reveal"]
[reveal_hugo]
custom_theme = "reveal-hugo/themes/robot-lung.css"
margin = 0.2
separator = "##"
+++

# Sequencing notes

- [Tone Step sequencer](https://tonejs.github.io/examples/stepSequencer.html)
- [Groove Pizza](https://apps.musedlab.org/groovepizza/?museid=89n23XJRl)
- [Infinite Drum Machine](https://experiments.withgoogle.com/ai/drum-machine/view/)
- [vGamelan](https://celanajaya.github.io/vGamelan/) - [code](https://github.com/celanajaya/vGamelan/)
- [Blips of Life](https://blipsoflife.herokuapp.com/)
- [Polymetric Drum Machine](https://react-drum-machine-6f184.firebaseapp.com/)

---

## Sequencing notes

- [Tone.Transport](https://github.com/Tonejs/Tone.js/wiki/Transport)
  - start
  - stop
  - toggle
    - go between start and stop
  - seconds
    - get current position in seconds
  - position
    - get beats:bars:sixteens
  - bpm
    - beats per minute

---

- schedule
- scheduleRepeat

<iframe src="https://codesandbox.io/embed/tone-transport-schedule-and-schedulerepeat-pi3b5f?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Tone.Transport - schedule and scheduleRepeat"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[Starter](https://codesandbox.io/s/tone-transport-schedule-and-schedulerepeat-start-52901u?file=%2Fsketch.js)

---

# higher level sequencers

## [overview](https://github.com/Tonejs/Tone.js/wiki/Events)

---

## Event

- abstracts away Tone.Transport.schedule and provides a schedulable callback for a single or repeatable events along the timeline
- loop
  - true or false
- loopEnd
- loopStart
- mute
  - won't fire if mute is true

---

- playbackRate
  - interval if looped
- probability
  - add randomness to note triggered probability
- progress
  - where are we in the loop?

---

<iframe src="https://codesandbox.io/embed/tone-transport-event-7kbzcs?fontsize=14&hidenavigation=1&theme=dark&view=preview"
     style="width:100%; height:500px; border:0; border-radius: 4px; overflow:hidden;"
     title="Tone.Transport - Event"
     allow="accelerometer; ambient-light-sensor; camera; encrypted-media; geolocation; gyroscope; hid; microphone; midi; payment; usb; vr; xr-spatial-tracking"
     sandbox="allow-forms allow-modals allow-popups allow-presentation allow-same-origin allow-scripts"
   ></iframe>

[starter](https://codesandbox.io/s/tone-transport-event-start-mfqdv6?file=%2Fsketch.js)
