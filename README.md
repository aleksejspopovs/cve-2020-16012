This repo contains PoCs for CVE-2020-16012, a side channel vulnerability in the implementation of [CanvasRenderingContext2D.drawImage()](https://developer.mozilla.org/en-US/docs/Web/API/CanvasRenderingContext2D/drawImage) in Firefox and Chromium.

Read a writeup of this vulnerability [on the Mozilla Attack & Defense blog](https://blog.mozilla.org/attack-and-defense/2021/01/11/leaking-silhouettes-of-cross-origin-images/).

Inside `benchmark` is code for measuring the timing of the operations involved, as well as the results of the benchmark obtained on Firefox 76 and Chromium 83 running on Linux using CPU rendering.

Inside `exploit` is an example exploit that recovers the silhouette of a cross-origin image using this vulnerability, as well as a recording of the exploit in action.
