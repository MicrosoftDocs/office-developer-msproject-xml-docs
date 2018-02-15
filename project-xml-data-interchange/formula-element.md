---
title: Formula Element
TOCTitle: Formula Element
ms:assetid: 5fe72a47-57ae-4871-9fc0-a9efbe596351
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968523(v=office.12)
ms:contentKeyID: 13188215
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Formula element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Formula Element




The formula that Microsoft Office Project uses to populate a task custom field.

    <Formula>
      StringValue
    </Formula>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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

In the following example, the Test Duration task custom field uses the formula \[Duration\]\*3. Because the value is calculated, the ValueGUID in the task is zero. The Value in the project summary task (task UID = 0) is 168 hours, 0 minutes, 0 seconds (PT in PT168H0M0S stands for Project Time, for internal use). The rollup to summary tasks is the sum of values in subtasks (RollupType = 3).

``` xml
<ExtendedAttributes>
   <ExtendedAttribute>
      <FieldID>188743957</FieldID>
      <FieldName>Duration6</FieldName>
      <Alias>Test Duration</Alias>
      <SecondaryPID>255868973</SecondaryPID>
      <RollupType>3</RollupType>
      <CalculationType>1</CalculationType>
      <Formula>[Duration]*3</Formula>
   </ExtendedAttribute>
</ExtendedAttributes>
. . .
<Tasks>
   <Task>
      <UID>0</UID>
      <ID>0</ID>
      . . .
      <ExtendedAttribute>
         <FieldID>188743957</FieldID>
         <Value>PT168H0M0S</Value>
         <DurationFormat>21</DurationFormat>
         <ValueGUID>00000000-0000-0000-0000-000000000000</ValueGUID>
      </ExtendedAttribute>
   </Task>
</Tasks>
```

## See Also

#### Concepts

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

