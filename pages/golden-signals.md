---
transition: fade-out
layout: center
---

# The 4 Golden Signals<sup>+</sup>


<div class="grid cols-2 ml-4" style="margin-top: -16px; margin-bottom: -25px">
    <div class="gif">
        <h3>Error Rate</h3>
        <img src="https://media3.giphy.com/media/v1.Y2lkPTc5MGI3NjExN3pnMW90ZGZpNmx0Z3Roczhxa3ZhbnhjbWNwN3ZvOGI3MGd6OGFmYSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/RSOUOj8H9A3Xq/giphy.gif">
    </div>
    <div class="gif">
        <h3>Latency</h3>
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExZHBnaGE1aG1heXpheTMwdHF4cG5tYXIzM2R3b3kwMXJzcXhzMDRxYiZlcD12MV9naWZzX3NlYXJjaCZjdD1n/l2JHVUriDGEtWOx0c/giphy.gif">
    </div><div class="gif">
        <h3>Traffic</h3>
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExNndoNWExcmNjam80ejFqNWM5ZjZ1eWRzeTQ3bzdldzRqMTExZ2xtcSZlcD12MV9naWZzX3NlYXJjaCZjdD1n/l0HlKQPTHOGNUPTZm/giphy.gif">
    </div>
    <div round class="gif">
        <h3>Saturation</h3>
        <img src="https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExbnpkcjFjMmJ0NHc4OWJnNXhwZ2U4NGlpbnM5bG4zdTVyd2Z0cXpkaCZlcD12MV9naWZzX3NlYXJjaCZjdD1n/d9CX7F5Um8vzZIZOp4/giphy.gif">
    </div>
</div>


<sup style="margin-top: -30px; text-align: right;">
<em>

+According to [Google' SRE book](https://sre.google/sre-book/monitoring-distributed-systems/#xref_monitoring_golden-signals)

</em>
</sup>

<style>
  img {
    padding: 10px;
    border-radius: 8%;
    height: 185px;
    width: 360px;
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

<!--
- ERRORS: requests that fail
    * implicitly: wrong features
    * explicitly: genuine errors
    * by policy: missed objectives
- LATENCY: time it takes to service a request
- TRAFFIC: demand is being placed on your system
- SATURATION: amount of work that a resource is unable to service
-->