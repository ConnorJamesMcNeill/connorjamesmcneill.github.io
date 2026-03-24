---
title: Voltage Buck | 24V to 12V Fan Adapter
date: 2025-05-15 12:00:00 -0700
categories: [Personal-Misc, Electrical]
tags: [mechatronics, electronics_integration, problem-solving]

image:
  path: /assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153100.jpg
  alt: Breadboard voltage buck circuit on a bench with power supply and PC fan
---

### The Circuit

I designed an extraction fan system to be retrofitted onto the Prusa MK4S enclosures at the University of Calgary Maker Space, which runs a fleet of 70 Prusa MK4s. The fans I spec'd ran on 24V to match the Prusa power supply output. The fans that showed up ran on 12V. With a deadline in sight and no time to wait on a reorder, I put together a quick voltage buck circuit on a breadboard: a 7812A three-terminal voltage regulator IC with a pair of capacitors (~133uF and ~100uF) to step the 24V supply down to 12V. It worked well enough to get through the immediate crunch. Not something I'd call a polished solution, but functional under the circumstances, and a good reminder that a basic understanding of electronics is worth having even when you're not an electrical engineer.

<br>

{% include embed/youtube.html id="phELdGaIZRA" %}

<br>

![Close-up of voltage buck circuit on breadboard with 4-pin fan connector](/assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153106.jpg){: width="100%" }

#### The buck circuit on the breadboard. The 7812A regulator and capacitors; minimal component count for a minimal problem.

<br>

![Breadboard buck circuit connected to fan with bench supply and oscilloscope visible](/assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153108.jpg){: width="100%" }

#### Circuit wired to the fan with the bench supply in the background. Confirmed working before the proper fans arrived.
