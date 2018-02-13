---
title: Type Element (Multiple Parents)
TOCTitle: Type Element
ms:assetid: 222dd5ab-8885-4858-b5c3-87f0d1636d2d
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968434(v=office.12)
ms:contentKeyID: 13188127
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Type element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Type Element (Multiple Parents)




As a child of the Mask or WBSMask elements, Type is the type of code string for first-level tasks (numbers, letters, or unordered characters).

In a Task element, Type is the type of task (fixed units, fixed duration, or fixed work).

In a PredecessorLink element, Type is the type of task link (FF, FS, SF or SS).

In a Resource element, Type is the type of resource (material or work).

In an Exception element, Type is the calendar exception type (daily, weekly, and so on).

In a Value element, Type is the type of outline code (date, duration, text, and so on).

In TimephasedData element, Type is one of the 76 types of timephased data.

    <Type>
      IntegerValue
    </Type>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968659(v=office.12).md">Mask</a>, <a href="bb968641(v=office.12).md">WBSMask</a>, <a href="bb968487(v=office.12).md">Task</a>, <a href="bb968712(v=office.12).md">PredecessorLink</a>, <a href="bb968715(v=office.12).md">Resource</a>, <a href="bb968492(v=office.12).md">Exception Element</a>, <a href="bb968696(v=office.12).md">Value Element</a>, <a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
</tr>
</tbody>
</table>

### Element Properties for Mask or WBSMask:

The Type element has an integer value that represents the type of code string for first-level tasks.

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
<td><p>0</p></td>
<td><p>Numbers (ordered); a numeric WBS code for this level (default).</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Uppercase Letters (ordered); uppercase, alphabetical WBS codes (for example, A, B, and C for the first three summary tasks in the project).</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Lowercase Letters (ordered); lowercase, alphabetical WBS codes (for example, a, b, and c for the first three summary tasks in the project).</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>Characters (unordered); any combination of numbers and uppercase or lowercase letters; for example, Arch1, Const1, or Insp1 for the first three summary tasks in the project. Project 2007 displays an asterisk (*) in the custom outline field until you type or enter a string of characters for the code.</p></td>
</tr>
</tbody>
</table>

### Element Properties for Task:

The Type element has an integer value that represents the type of task.

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
<td><p>0</p></td>
<td><p>Fixed units</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Fixed duration</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Fixed work</p></td>
</tr>
</tbody>
</table>

### Element Properties for PredecessorLink:

The Type element has an integer value that represents the type of task link.

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
<td><p>0</p></td>
<td><p>FF (finish-to-finish)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>FS (finish-to-start)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>SF (start-to-finish)</p></td>
</tr>
<tr class="even">
<td><p>3</p></td>
<td><p>SS (start-to-start)</p></td>
</tr>
</tbody>
</table>

### Element Properties for Resource:

The Type element has an integer value that represents the resource type (work, material, or cost).

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
<td><p>0</p></td>
<td><p>Material (consumable supplies like steel, concrete, or soil)</p></td>
</tr>
<tr class="even">
<td><p>1</p></td>
<td><p>Work (people and equipment)</p></td>
</tr>
<tr class="odd">
<td><p>2</p></td>
<td><p>Cost resource</p></td>
</tr>
</tbody>
</table>

### Element Properties for Exception:

The Type element has an integer value that represents the calendar exception type.

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
<td><p>1</p></td>
<td><p>Daily</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>Yearly by day of the month</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>Yearly by position</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>Monthly by day of the month</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>Monthly by position</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>Weekly</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>By day count</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>By weekday count</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>No exception type</p></td>
</tr>
</tbody>
</table>

### Element Properties for Value:

The Type element has an integer value that represents the type of outline code.

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
<td><p>4</p></td>
<td><p>Date</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>Duration</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>Cost</p></td>
</tr>
<tr class="even">
<td><p>15</p></td>
<td><p>Number</p></td>
</tr>
<tr class="odd">
<td><p>17</p></td>
<td><p>Flag</p></td>
</tr>
<tr class="even">
<td><p>21</p></td>
<td><p>Text</p></td>
</tr>
<tr class="odd">
<td><p>27</p></td>
<td><p>Finish date</p></td>
</tr>
</tbody>
</table>

### Element Properties for TimephasedData:

The Type element has an integer value that represents the type of timephased data.

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
<td><p>1</p></td>
<td><p>Assignment Remaining Work</p></td>
</tr>
<tr class="even">
<td><p>2</p></td>
<td><p>Assignment Actual Work</p></td>
</tr>
<tr class="odd">
<td><p>3</p></td>
<td><p>Assignment Actual Overtime Work</p></td>
</tr>
<tr class="even">
<td><p>4</p></td>
<td><p>Assignment Baseline Work</p></td>
</tr>
<tr class="odd">
<td><p>5</p></td>
<td><p>Assignment Baseline Cost</p></td>
</tr>
<tr class="even">
<td><p>6</p></td>
<td><p>Assignment Actual Cost</p></td>
</tr>
<tr class="odd">
<td><p>7</p></td>
<td><p>Resource Baseline Work</p></td>
</tr>
<tr class="even">
<td><p>8</p></td>
<td><p>Resource Baseline Cost</p></td>
</tr>
<tr class="odd">
<td><p>9</p></td>
<td><p>Task Baseline Work</p></td>
</tr>
<tr class="even">
<td><p>10</p></td>
<td><p>Task Baseline Cost</p></td>
</tr>
<tr class="odd">
<td><p>11</p></td>
<td><p>Task Percent Complete</p></td>
</tr>
<tr class="even">
<td><p>16</p></td>
<td><p>Assignment Baseline 1 Work</p></td>
</tr>
<tr class="odd">
<td><p>17</p></td>
<td><p>Assignment Baseline 1 Cost</p></td>
</tr>
<tr class="even">
<td><p>18</p></td>
<td><p>Task Baseline 1 Work</p></td>
</tr>
<tr class="odd">
<td><p>19</p></td>
<td><p>Task Baseline 1 Cost</p></td>
</tr>
<tr class="even">
<td><p>20</p></td>
<td><p>Resource Baseline 1 Work</p></td>
</tr>
<tr class="odd">
<td><p>21</p></td>
<td><p>Resource Baseline 1 Cost</p></td>
</tr>
<tr class="even">
<td><p>22</p></td>
<td><p>Assignment Baseline 2 Work</p></td>
</tr>
<tr class="odd">
<td><p>23</p></td>
<td><p>Assignment Baseline 2 Cost</p></td>
</tr>
<tr class="even">
<td><p>24</p></td>
<td><p>Task Baseline 2 Work</p></td>
</tr>
<tr class="odd">
<td><p>25</p></td>
<td><p>Task Baseline 2 Cost</p></td>
</tr>
<tr class="even">
<td><p>26</p></td>
<td><p>Resource Baseline 2 Work</p></td>
</tr>
<tr class="odd">
<td><p>27</p></td>
<td><p>Resource Baseline 2 Cost</p></td>
</tr>
<tr class="even">
<td><p>28</p></td>
<td><p>Assignment Baseline 3 Work</p></td>
</tr>
<tr class="odd">
<td><p>29</p></td>
<td><p>Assignment Baseline 3 Cost</p></td>
</tr>
<tr class="even">
<td><p>30</p></td>
<td><p>Task Baseline 3 Work</p></td>
</tr>
<tr class="odd">
<td><p>31</p></td>
<td><p>Task Baseline 3 Cost</p></td>
</tr>
<tr class="even">
<td><p>32</p></td>
<td><p>Resource Baseline 3 Work</p></td>
</tr>
<tr class="odd">
<td><p>33</p></td>
<td><p>Resource Baseline 3 Cost</p></td>
</tr>
<tr class="even">
<td><p>34</p></td>
<td><p>Assignment Baseline 4 Work</p></td>
</tr>
<tr class="odd">
<td><p>35</p></td>
<td><p>Assignment Baseline 4 Cost</p></td>
</tr>
<tr class="even">
<td><p>36</p></td>
<td><p>Task Baseline 4 Work</p></td>
</tr>
<tr class="odd">
<td><p>37</p></td>
<td><p>Task Baseline 4 Cost</p></td>
</tr>
<tr class="even">
<td><p>38</p></td>
<td><p>Resource Baseline 4 Work</p></td>
</tr>
<tr class="odd">
<td><p>39</p></td>
<td><p>Resource Baseline 4 Cost</p></td>
</tr>
<tr class="even">
<td><p>40</p></td>
<td><p>Assignment Baseline 5 Work</p></td>
</tr>
<tr class="odd">
<td><p>41</p></td>
<td><p>Assignment Baseline 5 Cost</p></td>
</tr>
<tr class="even">
<td><p>42</p></td>
<td><p>Task Baseline 5 Work</p></td>
</tr>
<tr class="odd">
<td><p>43</p></td>
<td><p>Task Baseline 5 Cost</p></td>
</tr>
<tr class="even">
<td><p>44</p></td>
<td><p>Resource Baseline 5 Work</p></td>
</tr>
<tr class="odd">
<td><p>45</p></td>
<td><p>Resource Baseline 5 Cost</p></td>
</tr>
<tr class="even">
<td><p>46</p></td>
<td><p>Assignment Baseline 6 Work</p></td>
</tr>
<tr class="odd">
<td><p>47</p></td>
<td><p>Assignment Baseline 6 Cost</p></td>
</tr>
<tr class="even">
<td><p>48</p></td>
<td><p>Task Baseline 6 Work</p></td>
</tr>
<tr class="odd">
<td><p>49</p></td>
<td><p>Task Baseline 6 Cost</p></td>
</tr>
<tr class="even">
<td><p>50</p></td>
<td><p>Resource Baseline 6 Work</p></td>
</tr>
<tr class="odd">
<td><p>51</p></td>
<td><p>Resource Baseline 6 Cost</p></td>
</tr>
<tr class="even">
<td><p>52</p></td>
<td><p>Assignment Baseline 7 Work</p></td>
</tr>
<tr class="odd">
<td><p>53</p></td>
<td><p>Assignment Baseline 7 Cost</p></td>
</tr>
<tr class="even">
<td><p>54</p></td>
<td><p>Task Baseline 7 Work</p></td>
</tr>
<tr class="odd">
<td><p>55</p></td>
<td><p>Task Baseline 7 Cost</p></td>
</tr>
<tr class="even">
<td><p>56</p></td>
<td><p>Resource Baseline 7 Work</p></td>
</tr>
<tr class="odd">
<td><p>57</p></td>
<td><p>Resource Baseline 7 Cost</p></td>
</tr>
<tr class="even">
<td><p>58</p></td>
<td><p>Assignment Baseline 8 Work</p></td>
</tr>
<tr class="odd">
<td><p>59</p></td>
<td><p>Assignment Baseline 8 Cost</p></td>
</tr>
<tr class="even">
<td><p>60</p></td>
<td><p>Task Baseline 8 Work</p></td>
</tr>
<tr class="odd">
<td><p>61</p></td>
<td><p>Task Baseline 8 Cost</p></td>
</tr>
<tr class="even">
<td><p>62</p></td>
<td><p>Resource Baseline 8 Work</p></td>
</tr>
<tr class="odd">
<td><p>63</p></td>
<td><p>Resource Baseline 8 Cost</p></td>
</tr>
<tr class="even">
<td><p>64</p></td>
<td><p>Assignment Baseline 9 Work</p></td>
</tr>
<tr class="odd">
<td><p>65</p></td>
<td><p>Assignment Baseline 9 Cost</p></td>
</tr>
<tr class="even">
<td><p>66</p></td>
<td><p>Task Baseline 9 Work</p></td>
</tr>
<tr class="odd">
<td><p>67</p></td>
<td><p>Task Baseline 9 Cost</p></td>
</tr>
<tr class="even">
<td><p>68</p></td>
<td><p>Resource Baseline 9 Work</p></td>
</tr>
<tr class="odd">
<td><p>69</p></td>
<td><p>Resource Baseline 9 Cost</p></td>
</tr>
<tr class="even">
<td><p>70</p></td>
<td><p>Assignment Baseline 10 Work</p></td>
</tr>
<tr class="odd">
<td><p>71</p></td>
<td><p>Assignment Baseline 10 Cost</p></td>
</tr>
<tr class="even">
<td><p>72</p></td>
<td><p>Task Baseline 10 Work</p></td>
</tr>
<tr class="odd">
<td><p>73</p></td>
<td><p>Task Baseline 10 Cost</p></td>
</tr>
<tr class="even">
<td><p>74</p></td>
<td><p>Resource Baseline 10 Work</p></td>
</tr>
<tr class="odd">
<td><p>75</p></td>
<td><p>Resource Baseline 10 Cost</p></td>
</tr>
<tr class="even">
<td><p>76</p></td>
<td><p>Physical Percent Complete</p></td>
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

## See Also

#### Concepts

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

[XML Schema for the WBSMasks Element](bb968565\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

