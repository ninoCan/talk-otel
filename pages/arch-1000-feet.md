---
transition: fade-out
layout: two-cols-header
addons:
  - fancy-arrow
---

# Architecture
## 1000-feet view

<br>
<br>
::left::

- Instrument & collect the _Context_
- Transmit
    * OTLP/HTTP (1 or 2)
    * OTLP/gRPC
- Collect & process
    * pipeline as YAML
- Send to Backends
    * !!! vendor-agnostic !!!

::right::

<img style="margin-top: -220px; border-radius: 5%" src="../assets/architecture.excalidraw.svg">


<div v-click.hide at="+1">
    <v-click>
      <FancyArrow
        x1="500"
        y1="120"
        x2="350"
        y2="220"
        color="blue"
      />
    </v-click>
</div>
<div v-click.hide at="+3">
<v-click at="-0">
    <FancyArrow
        x1="520"
        y1="375"
        x2="150"
        y2="260"
        color="red"
        arc="-0.2"
    />
    <FancyArrow
        x1="520"
        y1="235"
        x2="150"
        y2="260"
        color="red"
        arc="0.009"
    />
</v-click>
</div>
<div v-click.hide at="+2">
    <v-click at="-0">
        <FancyArrow
            x1="518"
            y1="312"
            x2="220"
            y2="360"
            color="green"
        />
    </v-click>
</div>
<v-click at="-0">
    <FancyArrow
        x1="518"
        y1="452"
        x2="225"
        y2="425"
        color="yellow"
    />
</v-click>

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
