---
title: WBSMask Element
TOCTitle: WBSMask Element
ms:assetid: ae403c08-a9a6-4116-933f-aaa6202ffda9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968641(v=office.12)
ms:contentKeyID: 13188332
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- WBSMask element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# WBSMask Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The work breakdown structure (WBS) mask that is applied to all tasks in the project.

    <WBSMask>
      ComplexTypeValue
    </WBSMask>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968580(v=office.12).md">WBSMasks</a></p></td>
</tr>
</tbody>
</table>

## Child Elements

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Element</p></th>
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="bb968635(v=office.12).md">Level</a></p></td>
<td><p>Required</p></td>
<td><p>Number of the WBS level, beginning with 1.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968434(v=office.12).md">Type</a></p></td>
<td><p>Required</p></td>
<td><p>Type of code string for first-level tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968526(v=office.12).md">Length</a></p></td>
<td><p>Required</p></td>
<td><p>Number of characters required for the WBS mask value, from 1-255. If there can be any number of characters, Length is zero.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968421(v=office.12).md">Separator</a></p></td>
<td><p>Required</p></td>
<td><p>Character used to separate the WBS mask levels.</p></td>
</tr>
</tbody>
</table>

## Occurrences

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Minimum: 0</p>
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## Example

In the following example, there are three levels in the WBS mask and a global prefix. Level one is of type uppercase characters, level two is numbers, and level three is unordered characters of any length. The table shows the WBS value for example tasks. The user typed the WBS level 3 value; Project generated the other WBS values. Because a task was deleted and WBS codes must be unique, task T2 has the WBS value Test-AC. The WBS value of the deleted task was Test-AB.

<table>
<colgroup>
<col style="width: 33%" />
<col style="width: 33%" />
<col style="width: 33%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Task</p></th>
<th><p>Task outline level</p></th>
<th><p>WBS value</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>T1</p></td>
<td><p>1</p></td>
<td><p>Test-AA</p></td>
</tr>
<tr class="even">
<td><p>st1</p></td>
<td><p>2</p></td>
<td><p>Test-AA.001</p></td>
</tr>
<tr class="odd">
<td><p>st2</p></td>
<td><p>2</p></td>
<td><p>Test-AA.002</p></td>
</tr>
<tr class="even">
<td><p>ss1</p></td>
<td><p>3</p></td>
<td><p>Test-AA.002.ThisIsATest</p></td>
</tr>
<tr class="odd">
<td><p>T2</p></td>
<td><p>1</p></td>
<td><p>Test-AC</p></td>
</tr>
</tbody>
</table>

``` xml
<Project>
   . . .
   <WBSMasks>
      <VerifyUniqueCodes>4</VerifyUniqueCodes>
      <GenerateCodes>1</GenerateCodes>
      <Prefix>Test-</Prefix>
      <Masks>
         <WBSMask>
            <Level>1</Level>
            <Type>1</Type>
            <Length>2</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>2</Level>
            <Type>0</Type>
            <Length>3</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>3</Level>
            <Type>3</Type>
            <Length>0</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
   </WBSMasks>
   . . .
   <Tasks>
      . . .
      <Task>
         <UID>1</UID>
         <ID>1</ID>
         <Name>T1</Name>
         <Type>1</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T13:34:00</CreateDate>
         <WBS>Test-AA</WBS>
         <WBSLevel>AA</WBSLevel>
         . . .
      </Task>
      . . .
   </Tasks>
   . . .
</Project>
```

## See Also

#### Concepts

[WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

[XML Schema for the WBSMasks Element](bb968565\(v=office.12\).md)

