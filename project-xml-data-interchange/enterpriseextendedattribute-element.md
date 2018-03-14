---
title: EnterpriseExtendedAttribute Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
---

# EnterpriseExtendedAttribute Element




An element representing the custom field value for the project, task, resoure, or assignment for enterprise custom fields with lookup tables.

    <EnterpriseExtendedAttribute>
      ComplexTypeValue
    </EnterpriseExtendedAttribute>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="project-element.md">Project</a>, <a href="task-element.md">Task</a>, <a href="resource-element.md">Resource</a>, <a href="assignment-element.md">Assignment</a></p></td>
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
<th><p>Required/Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="fieldidinhex-element.md">FieldIDInHex</a></p></td>
<td><p>Required</p></td>
<td><p>The ID of the row.</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldid-element.md">FieldID</a></p></td>
<td><p>Required</p></td>
<td><p>The field number of the lookup table value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="value-element.md">Value</a></p></td>
<td><p>Required</p></td>
<td><p>The value of the Enterprise Custom Field lookup table for the project, task, resource, or assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="fieldvalueguid-element.md">FieldValueGUID</a></p></td>
<td><p>Required</p></td>
<td><p>The GUID of the value of the Enterprise Custom Field lookup table.</p></td>
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
<p>Maximum: 450</p></td>
</tr>
</tbody>
</table>
