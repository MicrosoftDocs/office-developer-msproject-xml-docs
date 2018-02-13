---
title: DurationFormat Element
TOCTitle: DurationFormat Element
ms:assetid: ac69c48f-4758-4462-a9c3-edf085d52437
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968637(v=office.12)
ms:contentKeyID: 13188328
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- DurationFormat element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# DurationFormat Element




For Project, DurationFormat is the default format for all durations in the project.

For Task , it is the format used to show the duration of the task.

For Baseline, it is the format for expressing the duration of the task baseline.

For ExtendedAttribute, it is the format for the duration of the extended attribute, such as a duration custom field.

    <DurationFormat>
      IntegerValue
    </DurationFormat>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a>, <a href="bb968487(v=office.12).md">Task</a>, <a href="bb968599(v=office.12).md">Baseline</a>, <a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
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


> [!NOTE]
> Elapsed time counts all time, including non-working time specified in the project, resource, or task calendar. For example, if the calendar specifies Saturday and Sunday as non-working days, a duration of 7d is seven working days such as Monday – Friday and the following Monday and Tuesday. A duration of 7ed is seven elapsed days, such as Monday – Sunday.


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
<td><p>3</p></td>
<td><p>m (minutes)</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>em (elapsed minutes)</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>h (hours)</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>eh (elapsed hours)</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>d (days)</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>ed (elapsed days)</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>w (weeks)</p></td>
</tr>
<tr class="even">
<td><p>10</p></td>
<td><p>ew (elapsed weeks)</p></td>
</tr>
<tr class="odd">
<td><p>11</p></td>
<td><p>mo (months)</p></td>
</tr>
<tr class="even">
<td><p>12</p></td>
<td><p>emo (elapsed months)</p></td>
</tr>
<tr class="odd">
<td><p>19</p></td>
<td><p>% (percent)</p></td>
</tr>
<tr class="even">
<td><p>20</p></td>
<td><p>e% (elapsed percent)</p></td>
</tr>
<tr class="odd">
<td><p>21</p></td>
<td><p>Null</p></td>
</tr>
<tr class="even">
<td><p>35</p></td>
<td><p>m? (estimated minutes)</p></td>
</tr>
<tr class="odd">
<td><p>36</p></td>
<td><p>em? (estimated elapsed minutes)</p></td>
</tr>
<tr class="even">
<td><p>37</p></td>
<td><p>h? (estimated hours)</p></td>
</tr>
<tr class="odd">
<td><p>38</p></td>
<td><p>eh? (estimated elapsed hours)</p></td>
</tr>
<tr class="even">
<td><p>39</p></td>
<td><p>d? (estimated days)</p></td>
</tr>
<tr class="odd">
<td><p>40</p></td>
<td><p>ed? (estimated elapsed days)</p></td>
</tr>
<tr class="even">
<td><p>41</p></td>
<td><p>w? (estimated weeks)</p></td>
</tr>
<tr class="odd">
<td><p>42</p></td>
<td><p>ew? (estimated elapsed weeks)</p></td>
</tr>
<tr class="even">
<td><p>43</p></td>
<td><p>mo? (estimated months)</p></td>
</tr>
<tr class="odd">
<td><p>44</p></td>
<td><p>emo? (estimated elapsed months)</p></td>
</tr>
<tr class="even">
<td><p>51</p></td>
<td><p>%? (estimated percent)</p></td>
</tr>
<tr class="odd">
<td><p>52</p></td>
<td><p>e%? (estimated elapsed percent)</p></td>
</tr>
<tr class="even">
<td><p>53</p></td>
<td><p>Null</p></td>
</tr>
</tbody>
</table>

## Remarks

A DurationFormat can be included within a Baseline or ExtendedAttribute in a Resource or Assignment, as well as in a Task. It is used to override the default duration format in the Project element.

## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

