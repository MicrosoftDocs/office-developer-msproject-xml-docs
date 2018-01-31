---
title: UID Element
TOCTitle: UID Element
ms:assetid: 90074e2d-5cbf-475c-b456-5649c1b2949b
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968590(v=office.12)
ms:contentKeyID: 13188281
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- UID element
---

# UID Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The UID element is a unique identifier. UID specifies the data record of any of its parent elements within one project.

    <UID>
      String(16): for Project
      Integer: for all other parent elements
    </UID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a>, <a href="bb968481(v=office.12).md">Calendar</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968611(v=office.12).md">Assignment</a>, <a href="bb968487(v=office.12).md">Task</a>, <a href="bb968669(v=office.12).md">ExtendedAttribute</a>, <a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
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
<td><p>Minimum: 1</p>
<p>Maximum: 1</p></td>
</tr>
</tbody>
</table>

## Remarks

The UID element is a string only for the Project element. The UID child element in Project is deprecated in Microsoft Office Project 2007.

For its other parent elements, UID is an integer. UID values are unique only within a project, not across multiple projects.

For a task, each UID is used only once within the project. If you create a task named T3 with UID = 3 and ID = 3, delete the task, and then create a new task named T3 with ID = 3, the new task UID is 4.

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

