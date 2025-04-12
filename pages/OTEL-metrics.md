---
transition: fade-out
layout: center
---

# OTEL Metrics API

|  Continuos   |  On demand  | Explanation |
| :--- | --- | --- |
| <kbd>Counter</kbd> | <kbd>AsynchronousCounter</kbd> | never decreasing discrete values |
| <kbd>UpDownCounter</kbd>  | <kbd>AsynchronousUpDownCounter</kbd>| discreet increments and decrements |
| <kbd>Gauge</kbd> | <kbd>AsynchronousGauge</kbd> | continuous values |
| <kbd>Histogram</kbd> | - | measure frequency distribution |

<style>
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