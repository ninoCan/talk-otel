---
transition: fade-out
layout: two-cols-header
---

# Let's Dissect a Trace


::right::
```json
{
  "name": "hello-salutations",
  "context": {
    "trace_id": "5b8aa5a2d2c872e8321cf37308d69df2",
    "span_id": "93564f51e1abe1c2"
  },
  "parent_id": "051581bf3cb55c13",
  "start_time": "2022-04-29T18:52:58.114492Z",
  "end_time": "2022-04-29T18:52:58.114631Z",
  "attributes": {
    "http.route": "some_route3"
  },
  "events": [{
      "name": "hey there!",
      "timestamp": "2022-04-29T18:52:58.114561Z",
      "attributes": {
        "event_attributes": 1
        }
    }]
}
```
<div style="text-align: right"><sup><em>A Span as JSON </em></sup></div>


::left::

### `Span Link`
- Associate spans with a causal relationship
### `Span Context`
- Trace ID & Span ID
### `Attributes`
- Key-value metadata
- Can be specified by the Dev or `Semantic`
### `Span Status`
- One  of: `Unset`, `Error` or `Ok`
### `Span Event`
- Denote a meaningful, singular point in time
### `Baggage`
- Propagate information of parents without copying


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