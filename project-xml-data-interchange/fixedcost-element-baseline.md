---
title: FixedCost Element (Baseline)
TOCTitle: FixedCost Element
ms:assetid: 4b64e229-c147-4b3a-9deb-cae32a27fb11
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968494(v=office.12)
ms:contentKeyID: 13188186
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- FixedCost element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# FixedCost Element (Baseline)

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

The fixed cost of the task when the baseline was saved.

    <FixedCost>
      FloatValue
    </FixedCost>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968599(v=office.12).md">Baseline</a></p></td>
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

A text value of type float is required.

## Remarks

Fixed costs are costs for a task that remain constant regardless of the task duration, the amount of work performed by the resource, and the number of assignment units.

## Example

The following example uses the FixedCost element to indicate that the task has no fixed cost.

``` xml
<Task>
  …
  <FixedCost>0</FixedCost>
  …
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

