---
layout: two-cols-header
title: Logging Levels
---


# Logs flavours

<v-click>
  <div style="display: flex; justify-content: space-around;">
    <div style="background-color: #ADD8E6; padding: 20px; border-radius: 5px; text-align: center; width: 100px;">
      TRACE
    </div>
    <div style="background-color: #87CEEB; padding: 20px; border-radius: 5px; text-align: center; width: 100px;">
      DEBUG
    </div>
    <div style="background-color: #00BFFF; padding: 20px; border-radius: 5px; text-align: center; width: 100px;">
      INFO
    </div>
    <div style="background-color: #FFD700; padding: 20px; border-radius: 5px; text-align: left; width: 120px;">
      WARNING
    </div>
    <div style="background-color: #FF4500; padding: 20px; border-radius: 5px; text-align: center; width: 100px;">
      ERROR
    </div>
    <div style="background-color: #FF1493; padding: 20px; border-radius: 5px; text-align: left; width: 110px;">
      CRITICAL
    </div>
  </div>
</v-click>

::left::

<v-click>

## Unstructured

Simple strings

```log
[ERROR] 2024-08-04 12:45:23 - Failed to connect.
System reboot initiated at 2024-08-04 03:00:00
DEBUG - 2024-08-04 09:30:15 - action: file_upload.
```

</v-click>

<v-click>

## Semi-structured

String attributes
```log
2024-08-04T12:45:23Z level=ERROR service=user-authentication
    userId=12345 action=login message="Failed login attempt"
    error="Invalid password" ipAddress=192.168.1.1

```

</v-click>

::right::

<v-click>

## Structured
Full JSON payload

<div ml-2>

  ```json
  {
    "timestamp": "2024-08-04t12:34:56.789z",
    "level": "info",
    "service": "user-authentication",
    "environment": "production",
    "message": "user login successful",
    "context": {
      "userid": "12345",
      "username": "johndoe",
      "ipaddress": "192.168.1.1",
    },
  }
  ```
</div>

</v-click>

<style>
.slidev-layout {
    background: linear-gradient(to right, #A11CAF, #5B21B6);
}
</style>