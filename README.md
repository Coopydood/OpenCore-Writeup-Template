# OpenCore CHIPSET_MODEL (MODEL_GENERATION)
OpenCore Hackintosh configuration example for the **MOTHERBOARD_MODEL** motherboard with a CPU_MODEL. 

<img src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/af012dbc-dd39-474e-bb11-3f5ed0682cd3" alt="Image" width="1400"/>
<p align="center"><i>YOUR IMAGE HERE.</i></p>

<br>

## What works?

### macOS

- [ ] macOS VERSION_NAME

### Hardware

- [ ] Dedicated GPU (YOUR DGPU MODEL)
- [ ] iGPU (YOUR IGPU MODEL)
- [ ] NVMe drives
- [ ] SATA drives
- [ ] USB 3.1 (XHCI)
- [ ] Ethernet
- [ ] Wi-Fi
- [ ] Bluetooth
- [ ] Camera
- [ ] Sound
  
### Software

- [ ] AirDrop
- [ ] iMessage
- [ ] FaceTime
- [ ] Unlock with Apple Watch
- [ ] QE/CI graphics acceleration
- [ ] Metal support
- [ ] Temperature sensors
- [ ] Sleep / Wake
- [ ] RTC (protection)
- [ ] Hyperthreading
- [ ] Virtualisation
- [ ] Memory bank configuration
  
<br>

***

## Problems

<ul>
<li><b>YOUR PROBLEM HERE</b></li>
DESCRIBE YOUR PROBLEM HERE

<br>

<li><b>ANOTHER PROBLEM HERE</b></li>
DESCRIBE YOUR PROBLEM HERE

<br><br>

<li><b><s>FIXED PROBLEM EXAMPLE</s> ‏‏‎ ‏‏‎ ‎‎‏‏‎ ‎ 🎉 FIXED!</b></li>
<s>THE ART OF FIXING A PROBLEM AS DESCRIBED HERE</s>

> [!TIP]
> Describe to viewers how you managed to fix the issue here.

</ul>


***

## System

The specs of the main system that the OpenCore configuration targets.

| **Motherboard** |                  MOTHERBOARD_MODEL                 |
|-----------------|:-------------------------------------------------------------:|
| **CPU**         |                      CPU_MODEL                     |
| **Chipset**     |                             CHIPSET_MODEL                            |
| **Generation**  |                           MODEL_GENERATION                          |
| **Memory**      |                       HOST_RAM                       |
| **Storage**     |                     STORAGE_MODEL                    |
| **GPU**         | GPU_MODEL<br>~~DISABLED_GPU_MODEL~~ * |
| **NIC**         |                  ETHERNET_MODEL                  |

> [!NOTE]
> The system contains a **DISABLED_GPU_MODEL** graphics card, but it has been intentionally disabled through a custom YOUR_METHOD.

***

## ACPI

SSDTs used:
- SSDT-1
- SSDT-2
- SSDT-3
  
***

## DeviceProperties

The following tables display the added PCI devices and their child keys.


### PciRoot(0x0)/Pci(0x2,0x0)

EXAMPLE

| **Key**                  | **Type** |   **Value**  |
|--------------------------|:--------:|:------------:|
| AAPL,ig-platform-id      |   Data   | ``0000923E`` |
| device-id                |   Data   | ``923E7000`` |
| framebuffer-fbmem        |   Data   | ``00009000`` |
| framebuffer-patch-enable |   Data   | ``01000000`` |
| framebuffer-stolenmem    |   Data   | ``00003001`` |
| framebuffer-unifiedmem   |   Data   | ``00000080`` |
| hda-gfx                  |  String  |   onboard-1  |

<br>

### PciRoot(0x0)/Pci(0x1b,0x0)

Apple ALC

| **Key**                  | **Type** |   **Value**  |
|--------------------------|:--------:|:------------:|
| AAPL,ig-platform-id      |   Data   | ``0300220D`` |
| layout-id                |   Data   | ``01000000`` |


***

## Kernel

The following shows the kernel configuration.

### Kexts

Kexts used:
- Lilu
- WhateverGreen
- ...


### Patches

EXAMPLE

| **Key**     | **Type** |                **Value**                |
|-------------|:--------:|:---------------------------------------:|
| Arch        |  String  |                   Any                   |
| Base        |  String  |    __Z18e1000_set_mac_typeP8e1000_hw    |
| Comment     |  String  |               I225-V patch              |
| Count       |  Number  |                    1                    |
| Enabled     |  Boolean |                   True                  |
| Find        |   Data   |               ``F2150000``              |
| Identifier  |  String  | com.apple.driver.AppleIntelI210Ethernet |
| Limit       |  Number  |                    0                    |
| Mask        |   Data   |                                         |
| MaxKernel   |  String  |                  20.4.0                 |
| MinKernel   |  String  |                  19.0.0                 |
| Replace     |   Data   |               ``F3150000``              |
| ReplaceMask |   Data   |                                         |
| Skip        |  Number  |                    0                    |

***

## Security

**SecureBootModel 》** SECURE_BOOT_MODEL

**Vault 》** Optional


***

## NVRAM

Contents stored in NVRAM.

<br>

### 4D1EDE05-38C7-4A6A-9CC6-4BCCA8B38C14

| **Key**                | **Type** |   **Value**  |
|------------------------|:--------:|:------------:|
| DefaultBackgroundColor |   Data   | ``00000000`` |

<br>

### 4D1FDA02-38C7-4A6A-9CC6-4BCCA8B30102

| **Key**       | **Type** | **Value** |
|---------------|:--------:|:---------:|
| rtc-blacklist |   Data   |           |

<br>

### 7C436110-AB2A-4BBB-A880-FE41995C9F82

| **Key**                   | **Type** |                                    **Value**                                   |
|---------------------------|:--------:|:------------------------------------------------------------------------------:|
| boot-args                 |  String  | YOUR_BOOT_ARGS |

***

## SMBIOS

### MAC_MODEL

DESCRIPTION ON WHY YOU PICKED THIS SMBIOS MODEL...?

***



## UEFI

Drivers in use:

- HFSPlus
- OpenRuntime
- ...
  
***

## Gallery

ADD SOME IMAGES TO SHOW OFF YOUR WORK!

<img src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/9dd5dda0-92c3-4cc7-a7e4-3aab714671db" width="30%"></img> <img src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/4694291b-adcd-4847-99e2-a4f89c9c1ac9" width="60%"></img> <img src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/569407bd-0893-4974-82f0-ff669d317783" width="45%"></img> <img src="https://github.com/Coopydood/OpenCore-Z490E-CometLake/assets/39441479/c3ec115d-fe2c-4382-9fa3-d73d3c10cfd2" width="45%"></img> 

***

## Disclaimer

ADD A DISCLAIMER HERE!

