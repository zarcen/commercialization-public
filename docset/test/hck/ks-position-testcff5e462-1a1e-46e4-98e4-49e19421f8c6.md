---
author: joshbax-msft
title: KS Position Test
description: KS Position Test
MSHAttr:
- 'PreferredSiteName:MSDN'
- 'PreferredLib:/library/windows/hardware'
ms.assetid: 986fb0ea-b984-4d80-b18a-6f5b5c466abe
---

# KS Position Test


This automated test verifies that an audio device and driver accurately implement audio render position for stream synchronization.

This test requires that an audio device and driver are installed on a test system. The test targets the audio device and calls **GetPosition** on the kernel-streaming (KS) filter to make sure that the position is reported accurately.

The following table shows the details for this test.

## Test details


<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><strong>Associated requirements</strong></p></td>
<td><p>Device.Audio.Base.SamplePositionAccuracy Device.Audio.Base.TimeSynchronizedSampleRates</p>
<p>[See the device hardware requirements.](http://go.microsoft.com/fwlink/p/?linkid=254483)</p></td>
</tr>
<tr class="even">
<td><p><strong>Platforms</strong></p></td>
<td><p>Windows 7 (x64) Windows 7 (x86) Windows RT (ARM-based) Windows 8 (x64) Windows 8 (x86) Windows Server 2012 (x64) Windows Server 2008 R2 (x64) Windows RT 8.1 Windows 8.1 x64 Windows 8.1 x86 Windows Server 2012 R2</p></td>
</tr>
<tr class="odd">
<td><p><strong>Expected run time</strong></p></td>
<td><p>~12 minutes</p></td>
</tr>
<tr class="even">
<td><p><strong>Categories</strong></p></td>
<td><p>Certification Functional</p></td>
</tr>
<tr class="odd">
<td><p><strong>Type</strong></p></td>
<td><p>Automated</p></td>
</tr>
</tbody>
</table>

 

## Running the test


Before you run the test, complete the test setup as described in the test requirements: [Audio Device Testing Prerequisites](audio-device-testing-prerequisites.md).

## Troubleshooting


For troubleshooting information, see [Troubleshooting Audio Testing](troubleshooting-audio-testing.md).

## More information


### Command syntax

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>Command option</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><strong>CScript DevIDparse.vbs /WDKDeviceID:[WDKDeviceID]</strong></p></td>
<td><p>This command runs the KS Position test job.</p>
<div class="alert">
<strong>Note</strong>  
<p>For private testing, set the <strong>[WDKDeviceID]</strong> option to the device ID and run the test outside of the outside the Windows Hardware Certification Kit (Windows HCK) Studio.</p>
</div>
<div>
 
</div></td>
</tr>
</tbody>
</table>

 

**Note**  
For help with this test job, review the DevIDparse.vbs file in a text editor.

 

### File list

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr class="header">
<th>File</th>
<th>Location</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>DevIDParse.vb</p></td>
<td><p><em>&lt;testbinroot&gt;</em>\nttest\multimediatest\avcore\audio\scripts\</p></td>
</tr>
<tr class="even">
<td><p>S98wtt.dll</p></td>
<td><p><em>&lt;testbinroot&gt;</em>\nttest\multimediatest\common\</p></td>
</tr>
</tbody>
</table>

 

 

 





