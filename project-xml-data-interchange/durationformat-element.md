---
title: DurationFormat Element
ms.date: 02/24/2018
monikerRange: '>= project-client-2010 || project-client-odc'
---

# DurationFormat Element




For an item such as a task, it is the format for the duration. This paired with the duration value determine the actual duration of the item.


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
<td><p><a href="task-element.md">Task</a>, <a href="project-element.md">Project</a></p></td>
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


## See Also

#### Concepts

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

