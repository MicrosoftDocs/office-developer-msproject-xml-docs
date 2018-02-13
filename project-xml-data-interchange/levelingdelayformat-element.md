---
title: LevelingDelayFormat Element
TOCTitle: LevelingDelayFormat Element
ms:assetid: 2c22da44-4968-417b-887f-a2a1e05bdec9
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968448(v=office.12)
ms:contentKeyID: 13188140
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- LevelingDelayFormat element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# LevelingDelayFormat Element




 LevelingDelayFormat is the format for expressing the LevelingDelay duration in a task or assignment.

    <LevelingDelayFormat>
      IntegerValue
    </LevelingDelayFormat>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968487(v=office.12).md">Task</a>, <a href="bb968611(v=office.12).md">Assignment</a></p></td>
</tr>
</tbody>
</table>

### Element Properties

The LevelingDelayFormat element has an integer value that represents one of the following time units.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<thead>
<tr class="header">
<th><p><strong>Value</strong></p></th>
<th><p><strong>Description</strong></p></th>
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

A LevelingDelay requires the LevelingDelayFormat to be specified. For example, a leveling delay of 3 days in a task is expressed as follows:

``` xml
<Task>
    ...
    <LevelingDelay>3</LevelingDelay>
    <LevelingDelayFormat>7</LevelingDelayFormat>
    ...
</Task>
```

## See Also

#### Reference

[LevelingDelay Element](bb968397\(v=office.12\).md)

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

