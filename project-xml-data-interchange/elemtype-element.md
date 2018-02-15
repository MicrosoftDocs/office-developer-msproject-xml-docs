---
title: ElemType Element
TOCTitle: ElemType Element
ms:assetid: b9db69dd-41c2-4247-9e88-efa1fa74cff1
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968655(v=office.12)
ms:contentKeyID: 13188346
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- ElemType element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# ElemType Element




The type of entity (task, resource, or assignment) with which the custom field definition is associated.

    <ElemType>
      IntegerValue
    </ElemType>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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

A text value of type integer is required.

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
<td><p>20</p></td>
<td><p>Task</p></td>
</tr>
<tr class="even">
<td><p>21</p></td>
<td><p>Resource</p></td>
</tr>
<tr class="odd">
<td><p>23</p></td>
<td><p>Assignment</p></td>
</tr>
</tbody>
</table>

## Remarks

Custom field definitions must specify the type of project entity with which they are associated. For example, a custom field named Team Name, where ElemType = 21, is associated with a resource entity. For enterprise project custom fields, all tasks in a project have the same custom field value.

## Example

In the following example, the Health enterprise custom field, of type Text (CFType = 7), is associated with the task entity (ElemType = 20). The decimal value of FieldID corresponds to the b408001 element name in tasks, where the lookup table value for task UID 1 is On Schedule and the lookup table value for task UID 2 is Late.

The Plant ID enterprise project custom field value is associated with all tasks, including the project summary task (UID = 0). The FieldID decimal value 190873613 = the hexadecimal value of the b60800d element name. The Plant ID custom field value is Plant 47 in all tasks.

``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188776449</FieldID>
      <FieldName>Health</FieldName>
      <CFType>7</CFType>
      <Guid>0000E8D9-65F1-4769-9BD2-819D38036FCC</Guid>
      <ElemType>20</ElemType>
      <MaxMultiValues>1</MaxMultiValues>
      <UserDef>1</UserDef>
      <SecondaryPID>255885314</SecondaryPID>
      <DefaultGuid>000079D2-4A43-41FC-B264-98D23FADD84B</DefaultGuid>
   </ExtendedAttribute>
   <ExtendedAttribute>
      <FieldID>190873613</FieldID>
      <FieldName>Plant ID</FieldName>
      <CFType>7</CFType>
      <Guid>F162D66B-BF32-4030-998D-C2AA7BEAD285</Guid>
      <ElemType>20</ElemType>
      <MaxMultiValues>1</MaxMultiValues>
      <UserDef>1</UserDef>
   </ExtendedAttribute>
</ExtendedAttributes>
. . .
<Tasks>
   <Task>
      <UID>0</UID>
      <ID>0</ID>
      . . .
      <b60800d>Plant 47</b60800d>
   </Task>
   <Task>
      <UID>1</UID>
      <ID>1</ID>
      . . .
      <b408001>0000BB21-B2AE-410A-88B6-82C108903823</b408001>
      <b60800d>Plant 47</b60800d>
   </Task>
   <Task>
      <UID>2</UID>
      <ID>2</ID>
      . . .
      <b408001>0000C45D-8A43-4EB0-9B74-E535B391988A</b408001>
      <b60800d>Plant 47</b60800d>
   </Task>
</Tasks>
```

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

