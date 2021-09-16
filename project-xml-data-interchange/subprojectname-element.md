---
title: SubprojectName Element
TOCTitle: SubprojectName Element
ms:assetid: ba94763e-8c0a-4fe2-997c-cd85f5352ca3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968656(v=office.12)
ms:contentKeyID: 13188347
ms.date: 03/14/2018
mtps_version: v=office.12
f1_keywords:
- SubprojectName element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
ms.localizationpriority: medium
---

# SubprojectName Element




The source location of the inserted project.

    <SubprojectName>
      String(512)Value
    </SubprojectName>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="task-element.md">Task</a></p></td>
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

## Remarks

The subproject source can be a file or a project in Project Server.

## Example

The following example shows a local project file with the full path name C:\\Project\\P12\\XML\\Samples\\SubProj.mpp inserted as task ID 3 in a master project. The XML file for the master project includes the complete Project element for the inserted project as a child of task ID 3.

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

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

