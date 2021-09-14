---
title: WBSMasks Element
TOCTitle: WBSMasks Element
ms:assetid: 8901ca64-c183-4be9-895a-53d25a9975c4
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968580(v=office.12)
ms:contentKeyID: 13188271
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- WBSMasks element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# WBSMasks Element




The collection of elements that define a work breakdown structure (WBS) mask.

    <WBSMasks>
      ComplexTypeValue
    </WBSMasks>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
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
<td><p><a href="verifyuniquecodes-element.md">VerifyUniqueCodes</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether WBS codes are unique for new tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="generatecodes-element.md">GenerateCodes</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether WBS codes are generated for new tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="prefix-element.md">Prefix</a></p></td>
<td><p>Optional</p></td>
<td><p>Prefix for all WBS codes.</p></td>
</tr>
<tr class="even">
<td><p><a href="wbsmask-element.md">WBSMask</a></p></td>
<td><p>Optional</p></td>
<td><p>WBS mask that is applied to all tasks in the project.</p></td>
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
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Example

In the following example, there are two custom WBSMask levels in the WBS mask. Level one is three numbers, and level two is two lower case letters. The table shows the WBS value for example tasks. Because GenerateCodes = 1, Project generated WBS values for outline levels one and two. Although a task was deleted (the task with UID = 2), the WBS codes are not required to be unique; task T2 has the WBS value 002. The WBS value of the deleted task was also 002.

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
<td><p>001</p></td>
</tr>
<tr class="even">
<td><p>st1</p></td>
<td><p>2</p></td>
<td><p>001.aa</p></td>
</tr>
<tr class="odd">
<td><p>st2</p></td>
<td><p>2</p></td>
<td><p>001.ab</p></td>
</tr>
<tr class="even">
<td><p>ss1</p></td>
<td><p>3</p></td>
<td><p>001.ab.1</p></td>
</tr>
<tr class="odd">
<td><p>ss2</p></td>
<td><p>3</p></td>
<td><p>001.ab.2</p></td>
</tr>
<tr class="even">
<td><p>T2</p></td>
<td><p>1</p></td>
<td><p>002</p></td>
</tr>
</tbody>
</table>

``` xml
<Project>
   . . .
   <WBSMasks>
      <VerifyUniqueCodes>0</VerifyUniqueCodes>
      <GenerateCodes>1</GenerateCodes>
      <Masks>
         <WBSMask>
            <Level>1</Level>
            <Type>0</Type>
            <Length>3</Length>
            <Separator>.</Separator>
         </WBSMask>
      </Masks>
      <Masks>
         <WBSMask>
            <Level>2</Level>
            <Type>2</Type>
            <Length>2</Length>
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
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001</WBS>
         <WBSLevel>001</WBSLevel>
         <OutlineNumber>1</OutlineNumber>
         <OutlineLevel>1</OutlineLevel>
         . . .
      </Task>
      <Task>
         <UID>3</UID>
         <ID>2</ID>
         <Name>st1</Name>
         <Type>0</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001.aa</WBS>
         <WBSLevel>aa</WBSLevel>
         <OutlineNumber>1.1</OutlineNumber>
         <OutlineLevel>2</OutlineLevel>
         . . .
      </Task>
      <Task>
         <UID>4</UID>
         <ID>3</ID>
         <Name>st2</Name>
         <Type>1</Type>
         <IsNull>0</IsNull>
         <CreateDate>2007-11-13T14:33:00</CreateDate>
         <WBS>001.ab</WBS>
         <WBSLevel>ab</WBSLevel>
         <OutlineNumber>1.2</OutlineNumber>
         <OutlineLevel>2</OutlineLevel>
         . . .
      </Task>
      . . .
   </Tasks>
   . . .
</Project>
```

## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[WBSMask Elements and XML Structure](wbsmask-elements-and-xml-structure.md)

[XML Schema for the WBSMasks Element](xml-schema-for-the-wbsmasks-element.md)

