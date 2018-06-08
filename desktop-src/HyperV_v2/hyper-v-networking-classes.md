---
Description: The networking architecture for virtualization models the physical networking architecture. It uses standard networking objects such as switches, switch ports, and network adapters.
ms.assetid: ADD2903B-24BE-4877-B7D4-A1BDEE53FA29
title: Hyper-V networking API reference
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Hyper-V networking API reference

The networking architecture for virtualization models the physical networking architecture. It uses standard networking objects such as switches, switch ports, and network adapters.

The following are virtualization WMI classes related to networking.

## In this section



| Topic                                                                                                                    | Description                                                                                                                                                                                                                                                                                                                                                                  |
|--------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**Msvm\_ActiveConnection**](msvm-activeconnection.md)<br/>                                                       | Connects a switch port to the LAN endpoint to which the port is connected.<br/>                                                                                                                                                                                                                                                                                        |
| [**Msvm\_BindsToLANEndpoint**](msvm-bindstolanendpoint.md)<br/>                                                   | This association establishes a service access point (SAP) as a requester of protocol services from a protocol endpoint.<br/>                                                                                                                                                                                                                                           |
| [**Msvm\_ConcreteDependency**](msvm-concretedependency.md)<br/>                                                   | Defines the association between an installed Ethernet switch extension and an Ethernet switch extension.<br/>                                                                                                                                                                                                                                                          |
| [**Msvm\_DeviceSAPImplementation**](msvm-devicesapimplementation.md)<br/>                                         | An association between a service access point (SAP) and how it is implemented.<br/>                                                                                                                                                                                                                                                                                    |
| [**Msvm\_DynamicForwardingEntry**](msvm-dynamicforwardingentry.md)<br/>                                           | Represents an entry in the forwarding (filtering) database that is associated with the transparent bridging service.<br/>                                                                                                                                                                                                                                              |
| [**Msvm\_EmulatedEthernetPort**](msvm-emulatedethernetport.md)<br/>                                               | Represents an emulated Ethernet adapter.<br/>                                                                                                                                                                                                                                                                                                                          |
| [**Msvm\_EmulatedEthernetPortSettingData**](msvm-emulatedethernetportsettingdata.md)<br/>                         | Represents the configured state of an emulated Ethernet adapter.<br/>                                                                                                                                                                                                                                                                                                  |
| [**Msvm\_EthernetDeviceSAPImplementation**](msvm-ethernetdevicesapimplementation.md)<br/>                         | Represents an association between a service access point and the logical device that implements it.<br/>                                                                                                                                                                                                                                                               |
| [**Msvm\_EthernetPortAllocationSettingData**](msvm-ethernetportallocationsettingdata.md)<br/>                     | Represents an allocation request for a static or dynamic switch port, or represents the active configuration of a currently allocated static or dynamic switch port.<br/>                                                                                                                                                                                              |
| [**Msvm\_EthernetPortData**](msvm-ethernetportdata.md)<br/>                                                       | An abstract class that represents port runtime data collected by an Ethernet switch extension.<br/>                                                                                                                                                                                                                                                                    |
| [**Msvm\_EthernetPortFailoverSettingDataComponent**](msvm-ethernetportfailoversettingdatacomponent.md)<br/>       | An association used to establish relationships between one instance of an [**Msvm\_EmulatedEthernetPortSettingData**](msvm-emulatedethernetportsettingdata.md) and one or more instances of an [**Msvm\_EthernetSwitchFeatureSettingData**](msvm-ethernetswitchfeaturesettingdata.md).<br/>                                                                          |
| [**Msvm\_EthernetPortInfo**](msvm-ethernetportinfo.md)<br/>                                                       | An association between an instance of the [**Msvm\_EthernetSwitchPort**](msvm-ethernetswitchport.md) class and an instance of the [**Msvm\_EthernetPortData**](msvm-ethernetportdata.md) class that represents data gathered about the port by a switch extension.<br/>                                                                                              |
| [**Msvm\_EthernetPortSettingDataComponent**](msvm-ethernetportsettingdatacomponent.md)<br/>                       | An association used to establish "part of" relationships between one instance of an [**Msvm\_EthernetPortAllocationSettingData**](msvm-ethernetportallocationsettingdata.md) and one or more instances of an [**Msvm\_EthernetSwitchFeatureSettingData**](msvm-ethernetswitchfeaturesettingdata.md).<br/>                                                            |
| [**Msvm\_EthernetSwitchBandwidthData**](msvm-ethernetswitchbandwidthdata.md)<br/>                                 | Represents the switch bandwidth resource status.<br/>                                                                                                                                                                                                                                                                                                                  |
| [**Msvm\_EthernetSwitchData**](msvm-ethernetswitchdata.md)<br/>                                                   | Abstract class that represents a resource for a given instance of an Ethernet switch.<br/>                                                                                                                                                                                                                                                                             |
| [**Msvm\_EthernetSwitchExtension**](msvm-ethernetswitchextension.md)<br/>                                         | Represents an instance of an extension component bound to a virtual Ethernet switch.<br/>                                                                                                                                                                                                                                                                              |
| [**Msvm\_EthernetSwitchExtensionCapabilities**](msvm-ethernetswitchextensioncapabilities.md)<br/>                 | Represents the association between Ethernet extensions and their capabilities.<br/>                                                                                                                                                                                                                                                                                    |
| [**Msvm\_EthernetSwitchFeatureCapabilities**](msvm-ethernetswitchfeaturecapabilities.md)<br/>                     | Defines the means by which a client can discover the valid range of default settings for an Ethernet switch feature.<br/>                                                                                                                                                                                                                                              |
| [**Msvm\_EthernetSwitchFeatureSettingData**](msvm-ethernetswitchfeaturesettingdata.md)<br/>                       | An abstract class that represents settings for a given instance of an Ethernet switch feature.<br/>                                                                                                                                                                                                                                                                    |
| [**Msvm\_EthernetSwitchHardwareOffloadData**](msvm-ethernetswitchhardwareoffloaddata.md)<br/>                     | Represents the switch hardware offload status.<br/>                                                                                                                                                                                                                                                                                                                    |
| [**Msvm\_EthernetSwitchInfo**](msvm-ethernetswitchinfo.md)<br/>                                                   | Defines the association between an Ethernet switch and a switch resource.<br/>                                                                                                                                                                                                                                                                                         |
| [**Msvm\_EthernetSwitchOperationalData**](msvm-ethernetswitchoperationaldata.md)<br/>                             | Represents switch operational parameters.<br/>                                                                                                                                                                                                                                                                                                                         |
| [**Msvm\_EthernetSwitchPort**](msvm-ethernetswitchport.md)<br/>                                                   | Represents a port on the switch.<br/>                                                                                                                                                                                                                                                                                                                                  |
| [**Msvm\_EthernetSwitchPortAclSettingData**](msvm-ethernetswitchportaclsettingdata.md)<br/>                       | Represents the access control list (ACL) for switch port settings.<br/>                                                                                                                                                                                                                                                                                                |
| [**Msvm\_EthernetSwitchPortBandwidthData**](msvm-ethernetswitchportbandwidthdata.md)<br/>                         | Represents the port bandwidth feature status data.<br/>                                                                                                                                                                                                                                                                                                                |
| [**Msvm\_EthernetSwitchPortBandwidthSettingData**](msvm-ethernetswitchportbandwidthsettingdata.md)<br/>           | Represents the port bandwidth settings.<br/>                                                                                                                                                                                                                                                                                                                           |
| [**Msvm\_EthernetSwitchPortFeatureSettingData**](msvm-ethernetswitchportfeaturesettingdata.md)<br/>               | Abstract base class for classes that represent settings for an Ethernet switch port feature.<br/>                                                                                                                                                                                                                                                                      |
| [**Msvm\_EthernetSwitchPortOffloadData**](msvm-ethernetswitchportoffloaddata.md)<br/>                             | Represents the port offload feature status data.<br/>                                                                                                                                                                                                                                                                                                                  |
| [**Msvm\_EthernetSwitchPortOffloadSettingData**](msvm-ethernetswitchportoffloadsettingdata.md)<br/>               | Represents the port offload feature setting data.<br/>                                                                                                                                                                                                                                                                                                                 |
| [**Msvm\_EthernetSwitchPortProfileSettingData**](msvm-ethernetswitchportprofilesettingdata.md)<br/>               | Represents the port profile settings.<br/>                                                                                                                                                                                                                                                                                                                             |
| [**Msvm\_EthernetSwitchPortSecuritySettingData**](msvm-ethernetswitchportsecuritysettingdata.md)<br/>             | Represents the security feature setting data.<br/>                                                                                                                                                                                                                                                                                                                     |
| [**Msvm\_EthernetSwitchPortVlanSettingData**](msvm-ethernetswitchportvlansettingdata.md)<br/>                     | Represents the virtual LAN (VLAN) setting data.<br/>                                                                                                                                                                                                                                                                                                                   |
| [**Msvm\_ExternalEthernetPort**](msvm-externalethernetport.md)<br/>                                               | Represents an external Ethernet port (network adapter).<br/>                                                                                                                                                                                                                                                                                                           |
| [**Msvm\_ExternalEthernetPortCapabilities**](msvm-externalethernetportcapabilities.md)<br/>                       | Describes the capabilities of the associated [**Msvm\_ExternalEthernetPort**](msvm-externalethernetport.md).<br/>                                                                                                                                                                                                                                                     |
| [**Msvm\_GuestNetworkAdapterConfiguration**](msvm-guestnetworkadapterconfiguration.md)<br/>                       | Represents the configuration of a network adapter within the guest operating system.<br/>                                                                                                                                                                                                                                                                              |
| [**Msvm\_HostedEthernetSwitchExtension**](msvm-hostedethernetswitchextension.md)<br/>                             | Associates a virtual Ethernet switch to the extensions currently bound to it.<br/>                                                                                                                                                                                                                                                                                     |
| [**Msvm\_HostedSwitchService**](msvm-hostedswitchservice.md)<br/>                                                 | An association that connects a virtual switch service to a transparent bridging service.<br/>                                                                                                                                                                                                                                                                          |
| [**Msvm\_InstalledEthernetSwitchExtension**](msvm-installedethernetswitchextension.md)<br/>                       | Represents an instance of an extension component installed on a host system.<br/>                                                                                                                                                                                                                                                                                      |
| [**Msvm\_InternalEthernetPort**](msvm-internalethernetport.md)<br/>                                               | Represents an internal Ethernet port (network adapter).<br/>                                                                                                                                                                                                                                                                                                           |
| [**Msvm\_LANEndpoint**](msvm-lanendpoint.md)<br/>                                                                 | Represents the logical connection point for a network adapter. When the LAN endpoint is connected to a switch port, the network adapter connected to the LAN endpoint has network connectivity.<br/>                                                                                                                                                                   |
| [**Msvm\_ParentEthernetSwitchExtension**](msvm-parentethernetswitchextension.md)<br/>                             | Represents the association between a parent Ethernet switch extension and a child Ethernet switch extension.<br/>                                                                                                                                                                                                                                                      |
| [**Msvm\_SettingDataComponent**](msvm-settingdatacomponent.md)<br/>                                               | Establish a relationship between an instance of the [**Msvm\_EmulatedEthernetPortSettingData**](msvm-emulatedethernetportsettingdata.md) or [**Msvm\_SyntheticEthernetPortSettingData**](msvm-syntheticethernetportsettingdata.md) class with an instance of the [**Msvm\_GuestNetworkAdapterConfiguration**](msvm-guestnetworkadapterconfiguration.md) class.<br/> |
| [**Msvm\_SwitchPortDynamicForwarding**](msvm-switchportdynamicforwarding.md)<br/>                                 | Connects a switch port to a dynamic forward entry (learned MAC address).<br/>                                                                                                                                                                                                                                                                                          |
| [**Msvm\_SyntheticEthernetPort**](msvm-syntheticethernetport.md)<br/>                                             | Represents a synthetic Ethernet adapter.<br/>                                                                                                                                                                                                                                                                                                                          |
| [**Msvm\_SyntheticEthernetPortSettingData**](msvm-syntheticethernetportsettingdata.md)<br/>                       | Represents the configured state of a synthetic Ethernet adapter.<br/>                                                                                                                                                                                                                                                                                                  |
| [**Msvm\_TransparentBridgingDynamicForwarding**](msvm-transparentbridgingdynamicforwarding.md)<br/>               | Connects a transparent bridging service to a dynamic forward entry (learned MAC address).<br/>                                                                                                                                                                                                                                                                         |
| [**Msvm\_TransparentBridgingService**](msvm-transparentbridgingservice.md)<br/>                                   | Serves as a placeholder for the service inside the switch that learns MAC addresses and serves as a bridge between the [**Msvm\_VirtualEthernetSwitch**](msvm-virtualethernetswitch.md) and [**Msvm\_DynamicForwardingEntry**](msvm-dynamicforwardingentry.md) classes.<br/>                                                                                         |
| [**Msvm\_VirtualEthernetSwitch**](msvm-virtualethernetswitch.md)<br/>                                             | Represents a virtual Ethernet switch. Each switch has many different ports to which network adapters can be attached. The switch itself is not highly configurable and acts mostly as a placeholder.<br/>                                                                                                                                                              |
| [**Msvm\_VirtualEthernetSwitchBandwidthSettingData**](msvm-virtualethernetswitchbandwidthsettingdata.md)<br/>     | Represents the bandwidth settings for a virtual switch.<br/>                                                                                                                                                                                                                                                                                                           |
| [**Msvm\_VirtualEthernetSwitchManagementCapabilities**](msvm-virtualethernetswitchmanagementcapabilities.md)<br/> | Describes the capabilities of the associated [**Msvm\_VirtualEthernetSwitchManagementService**](msvm-virtualethernetswitchmanagementservice.md).<br/>                                                                                                                                                                                                                 |
| [**Msvm\_VirtualEthernetSwitchManagementService**](msvm-virtualethernetswitchmanagementservice.md)<br/>           | Represents the virtualization service present on a single host system. Msvm\_VirtualEthernetSwitchManagementService is used to control the definition, modification, and deletion of virtual Ethernet switches.<br/>                                                                                                                                                   |
| [**Msvm\_VirtualEthernetSwitchSettingData**](msvm-virtualethernetswitchsettingdata.md)<br/>                       | Represents the current configuration of a virtual Ethernet switch.<br/>                                                                                                                                                                                                                                                                                                |
| [**Msvm\_VirtualEthernetSwitchSettingDataComponent**](msvm-virtualethernetswitchsettingdatacomponent.md)<br/>     | An association used to establish "part of" relationships between one instance of [**Msvm\_VirtualEthernetSwitchSettingData**](msvm-virtualethernetswitchsettingdata.md) and one or more instances of [**Msvm\_EthernetSwitchFeatureSettingData**](msvm-ethernetswitchfeaturesettingdata.md).<br/>                                                                    |
| [**Msvm\_VLANEndpoint**](msvm-vlanendpoint.md)<br/>                                                               | Represents the VLAN endpoint of a switch port.<br/>                                                                                                                                                                                                                                                                                                                    |
| [**Msvm\_WiFiDeviceSAPImplementation**](msvm-wifidevicesapimplementation.md)<br/>                                 | An association between a service access point (SAP) and how it is implemented.<br/>                                                                                                                                                                                                                                                                                    |
| [**Msvm\_WiFiEndpoint**](msvm-wifiendpoint.md)<br/>                                                               | Represents the logical connection point for a network adapter. When the Wi-Fi endpoint is connected to a switch port, the network adapter connected to the Wi-Fi endpoint has network connectivity.<br/>                                                                                                                                                               |
| [**Msvm\_WiFiPort**](msvm-wifiport.md)<br/>                                                                       | Represents a physical Wi-Fi (802.11) network adapter that can be bound to a virtual switch to provide external network connectivity to virtual machines.<br/>                                                                                                                                                                                                          |



 

 

 



