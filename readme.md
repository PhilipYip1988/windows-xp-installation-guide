# Windows XP Reinstallation Guide

Before attempting to install Windows XP on your end of life Dell model, confer with the [Dell Drivers and Downloads](https://www.dell.com/support/home/en-uk?app=drivers) to check if there is a Windows XP driver set. The last Dell Desktop to support Windows XP Professional via OEM Downgrade Rights from Windows 7 Professional is the OptiPlex 7010 which has a Intel Q77 Express Chipset (3rd Generation Intel Processors). Intel did not provide drivers for the Intel Q87 Express Chipset (4th Generation Intel Processors).

## Dell Windows XP Reinstallation CD/DVD

Most Dell Windows XP Devices shipped with a Dell Windows Reinstallation CD/DVD:

<img src='./images/img_001.png' alt='img_001' width='600'/>

Windows XP Devices shipped with Windows XP came with a Windows XP Code of Authenticity (CoA). Newer Dell Business Devices came with a Windows Vista Business CoA or Windows 7 Professional CoA. The Product Key affixed to the CoA wasn't typically used as Windows XP OEM activated using OEM System Locked Preinstallation (SLP). In OEM SLP, the Dell Device has a System License Internal Code (SLIC) of 1.0 embedded in the Devices BIOS. Instead of the OEM Product Key on the CoA, a generic SLP key is used. When the SLP key is used in conjunction with a Dell Device with a SLIC 1.0, automatic offline Product Activation occurs:

<img src='./images/img_002.png' alt='img_002' width='600'/>

<details>
  <summary>Unofficial Links (Untested)</summary>

Unofficially a copy of the Dell Windows XP Reinstallation ISO appears to be listed here:

* [Archive Org Dell Windows XP SP3 Professional Reinstallation ISO](https://archive.org/details/dell.-xp-pro-sp-3)
* [Archive Org Dell Windows XP SP2 Home Reinstallation ISO](https://archive.org/details/dell-xp-home-sp-2)
* [Archive Org Dell Windows XP SP2 Media Center Reinstallation ISO](https://archive.org/details/xp-mce-sp-2)

For best results use a CD/DVD.

</details>

It is recommended to integrate Service Pack 3 and the systems driver cabinet using nLite as this will make Windows XP Installation on hardware much smoother. For more details see [Service Pack and Driver Integration using nLite](./integration/readme.md).

## Dell Media Direct DVD

Dell Media Direct was a Windows application for Media Playback configured for selected 2006-2007 Inspiron, Latitude and XPS laptop models. Dell also included a second power button which allowed Media Direct to boot from a preboot environment allowing Media Direct to be used outwith Windows. Ignore this section if your Dell Device does not have a Media Direct button:

<img src='./images/img_003.png' alt='img_003' width='600'/>

For correct operation the preboot environment needs to be setup before Windows by booting from the DVD and setting up the partitions and the application needs to be installed after Windows XP and the Windows XP system drivers:

<img src='./images/img_004.png' alt='img_004' width='600'/>

**Failure to setup up Media Direct properly on these models often resulted in Booting Issues when the Media Direct Button was pressed.**

<details>
  <summary>Unofficial Links (Untested)</summary>

For Inspiron 640M, 6400/E1505, 9400/E1705, XPS M1210, XPS M1710, XPS M2010:

* [Media Direct 3.3 ISO](https://archive.org/details/dell-media-direct-3.3)

For Inspiron 1420, 1520, 1720, 6400, XPS M1210
M1330, Latitude D620 and Latitude D630:

* [Dell Media Direct 3.3](https://archive.org/details/media-direct-restore)

For Vostro 1400, 1500, 1700:

* Dell Media Direct (No Download)

For Inspiron 1525, XPS M1330, M1530, M1730 and Latitude D830:

* [Dell Media Direct 3.5](https://archive.org/details/DellMediaDirect3.5ReinstallDVDForInspiron)

The Media Direct ISO images don't boot properly from USB so burn the image to a DVD.

</details>

## BIOS Setup

Power up the Dell and press `F2` to get to the Dell BIOS Setup:

<img src='./images/img_005.png' alt='img_005' width='600'/>

Most Dell XP Devices that supported Windows XP had a Legacy BIOS. However the later Dell Windows 7 Devices that supported Windows XP via downgrade rights had a UEFI BIOS. Windows XP does not support UEFI or Secure Boot: 

<img src='./images/img_006.png' alt='img_006' width='600'/>

Select Secure Boot:

<img src='./images/img_007.png' alt='img_007' width='600'/>

Change from Enabled to Disabled:

<img src='./images/img_008.png' alt='img_008' width='600'/>

<img src='./images/img_009.png' alt='img_009' width='600'/>

In Advanced Boot Options, enable Legacy Option ROMs:

<img src='./images/img_010.png' alt='img_010' width='600'/>

In System Configuration, the SATA Operation can be selected. For Windows XP use AHCI:

<img src='./images/img_011.png' alt='img_011' width='600'/>

## Setup Media Direct Partition

<details>
  <summary>Media Direct</summary>


<img src='./images/img_012.png' alt='img_012' width='600'/>



<img src='./images/img_013.png' alt='img_013' width='600'/>
<img src='./images/img_014.png' alt='img_014' width='600'/>
<img src='./images/img_015.png' alt='img_015' width='600'/>
<img src='./images/img_016.png' alt='img_016' width='600'/>
<img src='./images/img_017.png' alt='img_017' width='600'/>
<img src='./images/img_018.png' alt='img_018' width='600'/>

<img src='./images/img_019.png' alt='img_019' width='600'/>

</details>

## Installation


<img src='./images/img_020.png' alt='img_020' width='600'/>
<img src='./images/img_021.png' alt='img_021' width='600'/>
<img src='./images/img_022.png' alt='img_022' width='600'/>
<img src='./images/img_023.png' alt='img_023' width='600'/>
<img src='./images/img_024.png' alt='img_024' width='600'/>
<img src='./images/img_025.png' alt='img_025' width='600'/>
<img src='./images/img_026.png' alt='img_026' width='600'/>
<img src='./images/img_027.png' alt='img_027' width='600'/>
<img src='./images/img_028.png' alt='img_028' width='600'/>
<img src='./images/img_029.png' alt='img_029' width='600'/>
<img src='./images/img_030.png' alt='img_030' width='600'/>
<img src='./images/img_031.png' alt='img_031' width='600'/>
<img src='./images/img_032.png' alt='img_032' width='600'/>
<img src='./images/img_033.png' alt='img_033' width='600'/>
<img src='./images/img_034.png' alt='img_034' width='600'/>
<img src='./images/img_035.png' alt='img_035' width='600'/>
<img src='./images/img_036.png' alt='img_036' width='600'/>
<img src='./images/img_037.png' alt='img_037' width='600'/>
<img src='./images/img_038.png' alt='img_038' width='600'/>
<img src='./images/img_039.png' alt='img_039' width='600'/>
<img src='./images/img_040.png' alt='img_040' width='600'/>
<img src='./images/img_041.png' alt='img_041' width='600'/>
<img src='./images/img_042.png' alt='img_042' width='600'/>
<img src='./images/img_043.png' alt='img_043' width='600'/>
<img src='./images/img_044.png' alt='img_044' width='600'/>
<img src='./images/img_045.png' alt='img_045' width='600'/>
<img src='./images/img_046.png' alt='img_046' width='600'/>
<img src='./images/img_047.png' alt='img_047' width='600'/>
<img src='./images/img_048.png' alt='img_048' width='600'/>
<img src='./images/img_049.png' alt='img_049' width='600'/>
<img src='./images/img_050.png' alt='img_050' width='600'/>
<img src='./images/img_051.png' alt='img_051' width='600'/>