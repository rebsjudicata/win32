---
Description: 'Sent when the DVD Navigator parses a PCI packet.'
ms.assetid: '25548c23-22f0-47cb-9062-273ad39d3007'
title: 'EC\_DVD\_VOBU\_Timestamp'
---

# EC\_DVD\_VOBU\_Timestamp

Sent when the [DVD Navigator](dvd-navigator-filter.md) parses a PCI packet.

The event data is the time stamp of the most recent video object unit (VOBU).

## Parameters

<dl> <dt>

<span id="lParam1"></span><span id="lparam1"></span><span id="LPARAM1"></span>*lParam1*
</dt> <dd>

Contains the low-order **DWORD** of the time stamp.

</dd> <dt>

<span id="lParam2"></span><span id="lparam2"></span><span id="LPARAM2"></span>*lParam2*
</dt> <dd>

Contains the high-order **DWORD** of the time stamp.

</dd> </dl>

## Remarks

This event is disabled by default. To enable this event, call [**IDvdControl2::SetOption**](idvdcontrol2-setoption.md) and set the **DVD\_EnableLoggingEvents** option to **TRUE**.

Reconstruct the time stamp as follows:


```C++
LARGE_INTEGER li;
li.LowPart = DWORD( lParam1 );
li.HighPart = DWORD( lParam2 );
```



## Requirements



|                   |                                                                                                          |
|-------------------|----------------------------------------------------------------------------------------------------------|
| Header<br/> | <dl> <dt>Dvdevcode.h (include Dshow.h)</dt> </dl> |



## See also

<dl> <dt>

[DVD Applications](dvd-applications.md)
</dt> <dt>

[DVD Event Notification Codes](dvd-notification-codes.md)
</dt> <dt>

[Event Notification in DirectShow](event-notification-in-directshow.md)
</dt> </dl>

�

�



