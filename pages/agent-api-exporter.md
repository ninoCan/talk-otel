---
transition: fade-out
layout: two-cols-header
---

<div class="grid cols-2 ml-4">

<div style="align-content: center;">
<h1>The heart of OTEL</h1>
At its core a Proxy with different components
</div>
<div ><img style="float: right; border-radius: 5%" src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNnA4ZWpsMHpxc3Q0MTRlbjAzZTNqcDRsNTRobXZscTVudGl6NmowNiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/gx1735Ih9z4jVWZLAU/giphy.gif"></div>
</div>

::left::

### `Receiver`
- The landing API for signals

### `Exporter`
- Connectors to signals' backend

### `Pipeline`
- Telemetry tranformed & enriched via OTTL
- Possible to extend via a `Processor`
- Internal telemetry

::right::

<div style="text-align:right">
<sup><em>An example pipeline</em></sup></div>
```yaml
processors:
  filter/ottl:
    error_mode: ignore
    traces:
      span:
        - resource.attributes["service.name"] == "service1"
```
Possible actions:
<div id=menu>

<ul>
    <li>⚀ filter</li>
    <li>⚀ add</li>
    <li>⚀ rename</li>
    <li>⚀ delete</li>
</ul>

<ul>
    <li>⚀ set span status</li>
    <li>⚀ connect pipelines</li>
</ul>
<ul>
    <li>⚀ sampling</li>
    <li>⚀ route data</li>
    <li>⚀ <a href="https://github.com/open-telemetry/opentelemetry-collector-contrib/tree/main/pkg/ottl/ottlfuncs#ottl-functions">much more...</a></li>
</ul>
</div>

<style>
#menu ul{
  list-style: none;
}
#menu li{
  display: inline;
}
h1 {
  background-color:  linear-gradient(180deg, #271817 0%, #27181700 100%);
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 90%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
</style>