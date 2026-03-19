---
title: Voltage Buck | 24V to 12V Fan Adapter
date: 2025-05-15 12:00:00 -0700
categories: [Personal-Misc, Electrical]
tags: [mechatronics, electronics_integration, problem-solving]

image:
  path: /assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153100.jpg
  alt: Breadboard voltage buck circuit on a bench with power supply and PC fan
---

### I designed an extraction fan system to be retrofitted onto the Prusa MK4S enclosures at the University of Calgary Maker Space, which runs a fleet of 90 Prusa printers. The fans I spec'd ran on 24V to match the Prusa power supply output. The fans that showed up ran on 12V. With a deadline in sight and no time to wait on a reorder, I put together a quick voltage buck circuit on a breadboard -- a couple of resistors, a diode, and a small regulator -- to step the 24V supply down to something the fans could actually use. It worked well enough to get through the immediate crunch. Not something I'd call a polished solution, but functional under the circumstances, and a good reminder that a basic understanding of electronics is worth having even when you're not an electrical engineer.

{% include embed/youtube.html id="phELdGaIZRA" %}

<br>

#### Full bench setup. Power supply on the left feeding the buck circuit, fan on the bench confirming the output.

![Bench setup with power supply, breadboard buck circuit, and PC fan](/assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153100.jpg){: width="100%" }

<br>

#### The buck circuit on the breadboard. Regulator, resistors, and diode -- minimal component count for a minimal problem.

![Close-up of voltage buck circuit on breadboard with 4-pin fan connector](/assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153106.jpg){: width="100%" }

<br>

#### Circuit wired to the fan with the bench supply in the background. Confirmed working before the proper fans arrived.

![Breadboard buck circuit connected to fan with bench supply and oscilloscope visible](/assets/img/Personal-Misc/Electrical/Voltage Buck/20250515_153108.jpg){: width="100%" }
