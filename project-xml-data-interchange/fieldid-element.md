---
title: FieldID Element
TOCTitle: FieldID Element
ms:assetid: 3ed97e9e-cb2a-4aea-911c-a192b9e11891
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968474(v=office.12)
ms:contentKeyID: 13188166
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- FieldID element
---

# FieldID Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

In an OutlineCode, FieldID is the field number (project ID, or PID) of the outline code.

In an ExtendedAttribute, it corresponds to the enumeration value of a local custom field (Text1, Text2, Duration1, Duration2, and so on).

    <FieldID>
      IntegerValue
    </FieldID>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968410(v=office.12).md">OutlineCode</a>, <a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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

You should not use FieldID to identify uniqueness across multiple projects or versions of Microsoft Office Project.

For an enterprise custom field, the integer value of FieldID is the decimal equivalent of the hexadecimal enterprise custom field element name. For example, if an enterprise resource custom field element is c408005, the FieldID value is 205553669. For more information, see [c408000 - c417fff Elements](bb968524\(v=office.12\).md).

For a local custom field, the FieldID corresponds to PjCustomField enumeration value. For example, the FieldID 188743731 matches the pjCustomTaskText1 value in [PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx).


> [!NOTE]
> Some values of FieldID are currently missing in the PjCustomField documentation. However, you can find all of the enumeration values in the Object Browser in the Project Visual Basic editor (VBE). For example, the FieldID 205521019 is for pjCustomResourceCost1.


## See Also

#### Concepts

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

#### Other Resources

[PjCustomField Enumeration](http://msdn2.microsoft.com/en-ca/library/bb221982.aspx)

