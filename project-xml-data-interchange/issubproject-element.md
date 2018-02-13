---
title: IsSubproject Element
TOCTitle: IsSubproject Element
ms:assetid: a7dcc251-f796-4d75-8146-040fe30c066b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968630(v=office.12)
ms:contentKeyID: 13188321
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- IsSubproject element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# IsSubproject Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

Indicates whether the task is an inserted project.

    <IsSubproject>
      BooleanValue
    </IsSubproject>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a></p></td>
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

## Text Value

A text value of type boolean is required.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p>Value</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p>0</p></td>
<td><p>False</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>True</p></td>
</tr>
</tbody>
</table>

## Example

The following example shows a local project file inserted as task ID 3 in a master project. The XML file for the master project includes the complete Project element for the inserted project as a child of task ID 3.

``` xml
<Project xmlns="http://schemas.microsoft.com/project">
   . . .
   <Tasks>
      . . .
      <Task>
         <UID>4</UID>
         <ID>3</ID>
         <Name>SubProj</Name>
         <Type>1</Type>
         . . .
         <Summary>1</Summary>
         <Critical>1</Critical>
         <IsSubproject>1</IsSubproject>
         <IsSubprojectReadOnly>0</IsSubprojectReadOnly>
         <SubprojectName>C:\Project\P12\XML\Samples\SubProj.mpp</SubprojectName>
         <ExternalTask>0</ExternalTask>
         . . .
         <Project xmlns="http://schemas.microsoft.com/project">
            . . .
            <Tasks>
               <Task>
                  . . .
               </Task>
               . . .
            </Tasks>
            . . .
         </Project>
      </Task>
   </Tasks>
   . . .
</Project>
```

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

