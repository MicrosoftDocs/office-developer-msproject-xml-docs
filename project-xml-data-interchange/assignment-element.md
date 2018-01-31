---
title: Assignment Element
TOCTitle: Assignment Element
ms:assetid: 9e3ad85f-0226-4c99-8d3e-93c217f95308
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968611(v=office.12)
ms:contentKeyID: 13188302
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Assignment element
---

# Assignment Element

This content is outdated and is no longer being maintained. It is provided as a courtesy for individuals who are still using these technologies. This page may contain URLs that were valid when originally published, but now link to sites or pages that no longer exist.

There must be at least one assignment in each Assignments collection.

    <Assignment>
      ComplexTypeValue
    </Assignment>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968684(v=office.12).md">Assignments</a></p></td>
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
<th><p>Required / Optional</p></th>
<th><p>Description</p></th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td><p><a href="bb968590(v=office.12).md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>The unique ID for the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968646(v=office.12).md">TaskUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968535(v=office.12).md">ResourceUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The unique ID for the resource.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968608(v=office.12).md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of an assignment, expressed as the percentage of the assignment's work that has been completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968591(v=office.12).md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for work already performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968472(v=office.12).md">ActualFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time when an assignment was actually completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968431(v=office.12).md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The cost incurred for overtime work already performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968413(v=office.12).md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The actual amount of overtime work already performed by a resource on an assigned task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968713(v=office.12).md">ActualStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assignment actually began.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968429(v=office.12).md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of work that has already been done by a resource on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968717(v=office.12).md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The costs incurred for work already performed by a resource on a task up to the project status date or today's date; also called actual cost of work performed.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968559(v=office.12).md">Confirmed</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource assigned to a task has accepted or rejected the task assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled (or projected) cost for an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968541(v=office.12).md">CostRateTable</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates which cost rate table to use for a resource on an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968683(v=office.12).md">CostVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between the baseline cost and total cost for an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968685(v=office.12).md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between how much it should have cost to achieve the current level of completion on the assignment and how much it has actually cost.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968678(v=office.12).md">Delay</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time a resource is to wait after the task start date before starting work on an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968534(v=office.12).md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assigned resource is scheduled to complete work on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968724(v=office.12).md">FinishVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline finish date and its scheduled finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968729(v=office.12).md">Hyperlink</a></p></td>
<td><p>Optional</p></td>
<td><p>The title or explanatory text for a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968561(v=office.12).md">HyperlinkAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>The address for a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968602(v=office.12).md">HyperlinkSubAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>The specific location in a document within a hyperlink associated with an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968689(v=office.12).md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968547(v=office.12).md">HasFixedRateUnits</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an assignment has fixed rate units.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968521(v=office.12).md">FixedMaterial</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the consumption of the assigned material resource occurs in a single, fixed amount.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968397(v=office.12).md">LevelingDelay</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that an assignment is to be delayed from the scheduled start date as a result of resource leveling.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968448(v=office.12).md">LevelingDelayFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>The format for expressing the duration of the delay.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968484(v=office.12).md">LinkedFields</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether there are OLE links to the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968520(v=office.12).md">Milestone</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the assignment task is a milestone.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968616(v=office.12).md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes about an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968615(v=office.12).md">OverAllocated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a resource is assigned to more work on a specific task than can be done within the resource's normal working capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968407(v=office.12).md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total overtime cost for a resource assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968609(v=office.12).md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime to be performed by a resource on a task; charged at the resource's overtime rate.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968582(v=office.12).md">RegularWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of non-overtime work scheduled to be performed by a resource assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968728(v=office.12).md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The costs associated with completing all remaining scheduled work by any resources on a specific task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968690(v=office.12).md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>The remaining scheduled overtime expense for an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968473(v=office.12).md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of overtime work that remains on an assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968720(v=office.12).md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time required by a resource assigned to a task to complete an assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968477(v=office.12).md">ResponsePending</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an answer has been received from a message sent to a resource assigned to a task notifying the resource of the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968645(v=office.12).md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that an assigned resource is scheduled to begin working on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="https://msdn.microsoft.com/en-us/library/office%7cps12con%7c%7e%5chtml%5c3b4f7a6c-e08d-456e-85b4-186090f7791.htm(v=office.12)">Stop</a></p></td>
<td><p>Optional</p></td>
<td><p>The date the assignment was stopped.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968423(v=office.12).md">Resume</a></p></td>
<td><p>Optional</p></td>
<td><p>The date the assignment was resumed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968588(v=office.12).md">StartVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between an assignment's baseline start date and its currently scheduled start date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968468(v=office.12).md">Summary</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. Indicates whether an assignment is for a summary task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968647(v=office.12).md">SV</a></p></td>
<td><p>Optional</p></td>
<td><p>The earned value schedule variance, through the project status date</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968642(v=office.12).md">Units</a></p></td>
<td><p>Optional</p></td>
<td><p>The number of units for which a resource is assigned to a task, expressed as a percentage.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968735(v=office.12).md">UpdateNeeded</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a TeamUpdate message should be sent to the resource assigned to a task because of changes to the start date, finish date, or resource reassignments.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968455(v=office.12).md">VAC</a></p></td>
<td><p>Optional</p></td>
<td><p>The variance at completion (VAC) between the baseline cost and the total cost for an assignment on a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968571(v=office.12).md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>The total amount of work scheduled to be performed by a resource on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968726(v=office.12).md">WorkContour</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how work for an assignment is to be distributed across the duration of the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of work scheduled on the assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>The budgeted cost of the work performed on the assignment to-date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968505(v=office.12).md">BookingType</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the booking type of the assignment (committed or proposed).</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968400(v=office.12).md">ActualWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual work is protected.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968676(v=office.12).md">ActualOvertimeWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual overtime work is protected.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968396(v=office.12).md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The date that the assignment was created.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968408(v=office.12).md">AssnOwner</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The name of the assignment owner.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968551(v=office.12).md">AssnOwnerGuid</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The GUID of the assignment owner.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968532(v=office.12).md">BudgetCost</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The budgeted amount for cost resources on this assignment.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968506(v=office.12).md">BudgetWork</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. The budgeted work amount for work or material resources on this assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>The value of an extended attribute (custom field).</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968599(v=office.12).md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>The collection of baseline values associated with the assignment.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968556(v=office.12).md">f404000 - f4040c8 Elements</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. An assignment-level local custom field value.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968688(v=office.12).md">f408000 - f417fff Elements</a></p></td>
<td><p>Optional</p></td>
<td><p>New for Project 2007. An assignment-level enterprise custom field value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>Information about the assignment that is distributed over time.</p></td>
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
<p>Maximum: Unbounded</p></td>
</tr>
</tbody>
</table>

## See Also

#### Concepts

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

