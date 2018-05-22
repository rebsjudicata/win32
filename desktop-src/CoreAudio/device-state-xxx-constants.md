---
Description: 'The DEVICE\_STATE\_XXX constants indicate the current state of an audio endpoint device.'
ms.assetid: 'd03f2fbc-313a-42cf-902a-fd9f6dce2a35'
title: 'DEVICE\_STATE\_XXX Constants'
---

# DEVICE\_STATE\_XXX Constants

The DEVICE\_STATE\_XXX constants indicate the current state of an audio endpoint device.



| Constant/value                                                                                                                                                                                                                                               | Description                                                                                                                                                                                                                                                                                                                                                                      |
|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span id="DEVICE_STATE_ACTIVE"></span><span id="device_state_active"></span><dl> <dt>**DEVICE\_STATE\_ACTIVE**</dt> <dt>0x00000001</dt> </dl>             | The audio endpoint device is active. That is, the audio adapter that connects to the endpoint device is present and enabled. In addition, if the endpoint device plugs into a jack on the adapter, then the endpoint device is plugged in.<br/>                                                                                                                            |
| <span id="DEVICE_STATE_DISABLED"></span><span id="device_state_disabled"></span><dl> <dt>**DEVICE\_STATE\_DISABLED**</dt> <dt>0x00000002</dt> </dl>       | The audio endpoint device is disabled. The user has disabled the device in the Windows multimedia control panel, Mmsys.cpl. For more information, see Remarks.<br/>                                                                                                                                                                                                        |
| <span id="DEVICE_STATE_NOTPRESENT"></span><span id="device_state_notpresent"></span><dl> <dt>**DEVICE\_STATE\_NOTPRESENT**</dt> <dt>0x00000004</dt> </dl> | The audio endpoint device is not present because the audio adapter that connects to the endpoint device has been removed from the system, or the user has disabled the adapter device in Device Manager.<br/>                                                                                                                                                              |
| <span id="DEVICE_STATE_UNPLUGGED"></span><span id="device_state_unplugged"></span><dl> <dt>**DEVICE\_STATE\_UNPLUGGED**</dt> <dt>0x00000008</dt> </dl>    | The audio endpoint device is unplugged. The audio adapter that contains the jack for the endpoint device is present and enabled, but the endpoint device is not plugged into the jack. Only a device with jack-presence detection can be in this state. For more information about jack-presence detection, see [Audio Endpoint Devices](audio-endpoint-devices.md).<br/> |
| <span id="DEVICE_STATEMASK_ALL"></span><span id="device_statemask_all"></span><dl> <dt>**DEVICE\_STATEMASK\_ALL**</dt> <dt>0x0000000F</dt> </dl>          | Includes audio endpoint devices in all states�active, disabled, not present, and unplugged.<br/>                                                                                                                                                                                                                                                                           |



## Remarks

The [**IMMDeviceEnumerator::EnumAudioEndpoints**](immdeviceenumerator-enumaudioendpoints.md), [**IMMDevice::GetState**](immdevice-getstate.md), and [**IMMNotificationClient::OnDeviceStateChanged**](immnotificationclient-ondevicestatechanged.md) methods use the DEVICE\_STATE\_XXX constants. These methods enable clients to obtain information about endpoint devices that are in any of the states represented by the DEVICE\_STATE\_XXX constants.

However, a client can open a stream (for example, by obtaining an [**IAudioClient**](iaudioclient.md) interface for the device) only on a device that is in the DEVICE\_STATE\_ACTIVE state.

The Windows multimedia control panel, Mmsys.cpl, displays the audio endpoint devices in the system. Disabling a device in Mmsys.cpl hides the device from the device-discovery mechanisms in higher-level audio APIs, but it does not invalidate any stream objects that a client might have instantiated before the device was disabled. For example, if a stream is playing on the device when the user disables it in Mmsys.cpl, the stream continues to play uninterrupted.

In contrast, disabling a device in Device Manager effectively removes the device from the system.

To use Mmsys.cpl to view the rendering devices, open a Command Prompt window and enter the following command:

**control mmsys.cpl,,0**

To view the capture devices, enter the following command:

**control mmsys.cpl,,1**

Alternatively, you can view the rendering devices or the capture devices in Mmsys.cpl by right-clicking the speaker icon in the notification area, which is located on the right side of the taskbar, and selecting **Playback Devices** or **Recording Devices**.

Mmsys.cpl always displays endpoint devices that are in the DEVICE\_STATE\_ACTIVE state. In addition, it can be configured to display disabled and disconnected devices.

To view endpoint devices that are in the DEVICE\_STATE\_DISABLED and DEVICE\_STATE\_NOTPRESENT states, right-click in the Mmsys.cpl window and select the **Show Disabled Devices** option.

To view endpoint devices that are in the DEVICE\_STATE\_UNPLUGGED state, right-click in the Mmsys.cpl window and select the **Show Disconnected Devices** option.

To view only endpoint devices that are in the DEVICE\_STATE\_ACTIVE state, deselect both the **Show Disabled Devices** and **Show Disconnected Devices** options.

To enable or disable an endpoint device in Mmsys.cpl, click **Playback** or **Recording**, depending on whether the device is a playback or recording device. Next, select the device and click **Properties**. In the **Properties** window, next to **Device usage**, select either **Use this device (enable)** or **Don't use this device (disable)**.

## Requirements



|                                     |                                                                                          |
|-------------------------------------|------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                           |
| Minimum supported server<br/> | Windows Server�2008 \[desktop apps only\]<br/>                                     |
| Header<br/>                   | <dl> <dt>Mmdeviceapi.h</dt> </dl> |



## See also

<dl> <dt>

[Core Audio Constants](core-audio-constants.md)
</dt> <dt>

[**IMMDevice::GetState**](immdevice-getstate.md)
</dt> <dt>

[**IMMDeviceEnumerator Interface**](immdeviceenumerator.md)
</dt> <dt>

[**IMMDeviceEnumerator::EnumAudioEndpoints**](immdeviceenumerator-enumaudioendpoints.md)
</dt> <dt>

[**IMMNotificationClient::OnDeviceStateChanged**](immnotificationclient-ondevicestatechanged.md)
</dt> </dl>

�

�



