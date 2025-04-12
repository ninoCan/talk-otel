---
transition: fade-out
layout: image-right
image: "../assets/architecture.excalidraw.svg"
---

# Architecture
## 1000<sup>nd</sup>-feet view

<br>
<br>

- Instrument & collect the _Context_
- Transmit
    * OTLP/HTTP (1 or 2)
    * OTLP/gRPC
- Collect & process
    * pipeline as YAML
- Send to Backends
    * !!! vendor-agnostic !!!

<style>
h1, h2 {
  background-color:  linear-gradient(180deg, #271817 0%, #27181700 100%);
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 90%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>