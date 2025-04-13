---
layout: two-cols-header
addons:
  - fancy-arrow
---

# Architecture
## 1000-feet view

<br>
<br>
::left::

- Instrument & collect the _Context_<span data-id="instr"> &nbsp; </span>
- Transmit<span data-id="trans">&nbsp;</span>
    * OTLP/HTTP (1 or 2)
    * OTLP/gRPC
- Collect & process<span data-id="collect">&nbsp;</span>
    * pipeline as YAML
- Send to Backends<span data-id="export">&nbsp;</span>
    * !!! vendor-agnostic !!!

::right::

<img style="margin-top: -180px; border-radius: 5%" src="../assets/architecture.excalidraw.svg">


<div v-click.hide at="+1">
    <v-click>
      <FancyArrow
        x1="500"
        y1="120"
        q2="[data-id=instr]"
        pos2="right"
        color="blue"
      />
    </v-click>
</div>
<div v-click.hide at="+3">
<v-click at="-0">
    <FancyArrow
        x1="520"
        y1="375"
        q2="[data-id=trans]"
        pos2="right"
        color="red"
        arc="-0.2"
    />
    <FancyArrow
        x1="520"
        y1="235"
        q2="[data-id=trans]"
        pos2="right"
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
        q2="[data-id=collect]"
        pos2="right"
            color="green"
        />
    </v-click>
</div>
<v-click at="-0">
    <FancyArrow
        x1="518"
        y1="452"
        q2="[data-id=export]"
        pos2="right"
        color="yellow"
    />
</v-click>

<style>
.slidev-layout {
    background: linear-gradient(to right, #A11CAF, #5B21B6);
}
</style>
