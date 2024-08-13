---
title: "Linearized N-Path for Self-Interference Cancellation"
excerpt: "Developed adaptive and reconfigurable n-path linear filters for high programmability across diverse applications, achieving effective self-interference cancellation at 500MHz with an IM3 value of -5dBm (two-tone) and a supply voltage of 3.3V.<br/><img src='/images/npath1.png'>"
collection: portfolio
---

---
title: "Linearized N-Path for Self-Interference Cancellation"
excerpt: "Developed adaptive and reconfigurable n-path linear filters for high programmability across diverse applications, achieving effective self-interference cancellation at 500MHz with an IM3 value of -5dBm (two-tone) and a supply voltage of 3.3V.<br/><img src='/images/npath1.png' style='display: block; margin-left: auto; margin-right: auto; width: 50%;'/>"
collection: portfolio
---

N-path filters have emerged as a revolutionary type of tunable band-pass filter that is gaining interest in RF radio applications. Unlike traditional discrete RF filters, which are bulky and expensive, N-path filters can be integrated into silicon, reducing size, cost, and power consumption while offering great configurability. Specifically, these filters leverage periodic switching to achieve band-pass filtering over a wide range of frequencies by programmably adjusting their frequency response. This ability to fine-tune filtering characteristics makes N-path filters particularly useful in rejecting undesired interference in RF radios and generating programmable delay spreads for self-interference cancelers. Currently, the main limitation of this technology is its insufficient linearity for high-output power applications. Despite this, the ongoing advancements in N-path filter design and integration hold significant promise for future enhancements in RF performance and efficiency.

<br/>
<img src='/images/npath2.png' style='display: block; margin-left: auto; margin-right: auto; width: 50%;'/>
<p style='text-align: center;'>N-Path Filter Schematic</p>
<br/>
<img src='/images/npath3.png' style='display: block; margin-left: auto; margin-right: auto; width: 50%;'/>
<p style='text-align: center;'>N-Path Filter Layout</p>
<br/>

Specific contributions included: Resistive Ladder Schematic Design, Layout, and Verification, 5:32 Decoder Schematic Design, Layout, and Verification. The n-path circuitry requires two voltage bias circuits with different voltage ranges. The voltage range of the common mode voltage bias is 0-800mV with a 25mV resolution, and the voltage range of the transistor mode voltage bias is 1.0-1.8 V with a 25mV resolution. To achieve this, a design with a series of 32 resistors, each providing a 25mV resolution between nodes, was implemented. A 5:32 decoder is used to switch to the required node. The output of the decoder is connected to each resistor node with a transistor acting as a switch, passing one node to the output. This design was implemented using the Skywater 130nm PDK standard cells. The input bits are taken from the scan chain, which not only decides the voltage bias but also determines which implementation of the n-path is to be tested. With four different implementations, the 2:4 decoder was used again to disable unused biases and unused clocking as well.

**Skills**: Analog Design, Klayout, Top-level Layout Design, Verification
