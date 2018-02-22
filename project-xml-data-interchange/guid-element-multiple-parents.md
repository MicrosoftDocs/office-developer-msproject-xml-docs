---
title: Guid Element (Multiple Parents)
ms.date: 05/05/2014
monikerRange: '>= project-client-2010 || project-client-odc'
---

# Guid Element (Multiple Parents)




The globally unique identifier (GUID) of an outline code, enterprise custom field, project, task, board column, sprint, assignment, resource, or calendar. The value is not loadable for the project, task, board column, sprint, assignment, resource, or calendar elements.

    <Guid>
        StringValue
    <Guid>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="calendar-element.md">Calendar</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a>, <a href="task-element.md">Task</a>, <a href="outlinecode-element.md">OutlineCode</a>, <a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
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
<td><p>Minimum: 0 for local custom fields, tasks, resources, assignments, calendars, board columns, sprints, and project; 1 for outline codes and enterprise custom fields.</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Text Value

A text value of type string is required. The string must be in the form "HHHHHHHH-HHHH-HHHH-HHHH-HHHHHHHHHHHH" where H represents a hexadecimal digit between 0 and F.

## Remarks

For the ExtendedAttribute element, Guid is the custom field GUID.

For the OutlineCode element, Guid is the outline code GUID. Local outline codes and enterprise custom fields and require the Guid element; local custom fields do not.

## Example

In the following example, Text1 is a local task custom field, which does not include the Guid element. Health is an enterprise custom field, which uses the Guid element to represent the GUID of the enterprise custom field.

``` xml
<ExtendedAttributes>
  <ExtendedAttribute>
    <FieldID>188743731</FieldID>
    <FieldName>Text1</FieldName>
    <Alias>Test Task CF</Alias>
    <Ltuid>ED2E65AD-00A1-4457-97FA-A3FC708C9183</Ltuid>
    <SecondaryPID>255869028</SecondaryPID>
  </ExtendedAttribute>
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
</ExtendedAttributes>
```

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

