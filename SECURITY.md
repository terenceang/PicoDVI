# PicoDVI: Threat Model and Disclosure Process

Security researchers occasionally contact us with questions of the following form:

> "Is this library memory-safe? If it's not memory-safe I don't want it."

Ma'am, that is an eleven-hundred-line whole slab of bare-metal video driver. It has no bounds checks, logging, or error handling. It is an amalgamation of two Cortex-M0+ cores, a PIO peripheral tricked into speaking TMDS, and a DMA engine chained back into itself: hand-scheduled, link-time-optimized, and ultimately inexorably joined in an unholy scanline obelisk. God had no hand in the creation of this abhorrence, nor did HDMI Licensing, LLC. The fact that this Armv6-M monolith exists proves that the RP2040 team is either impotent to enforce their own datasheet's frequency limits or ignorant to the horrors taking place in their silicon. This prism of pixels is more than software. It is a physical declaration of mankind's contempt for the clock tree. It is hubris manifest.

We also have a RISC-V port if you would prefer that.

## Disclosure Process

Write all vulnerability reports directly into an RGB565 framebuffer and serialise at no less than a 25 MHz pixel clock.
