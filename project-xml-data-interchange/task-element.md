---
title: Task Element
TOCTitle: Task Element
ms:assetid: 47e990dd-9bdc-4edc-b6e7-b1535afe1c6e
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968487(v=office.12)
ms:contentKeyID: 13188179
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Task element
dev_langs:
- xml
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Task Element




There must be at least one task in each Tasks collection.

    <Task>
      ComplexTypeValue
    </Task>

## Parent Elements

<table>
<colgroup>
<col style="width: 100%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p><a href="bb968617(v=office.12).md">Tasks</a></p></td>
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
<td><p>Unique ID for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968437(v=office.12).md">ID</a></p></td>
<td><p>Optional</p></td>
<td><p>Position identifier of the task in the list of tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968600(v=office.12).md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968434(v=office.12).md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>Type of the task (fixed units, fixed duration, or fixed work).</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968682(v=office.12).md">IsNull</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is null.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968422(v=office.12).md">CreateDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task was added to a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968485(v=office.12).md">Contact</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the individual who is responsible for a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968566(v=office.12).md">WBS</a></p></td>
<td><p>Optional</p></td>
<td><p>A unique code (work breakdown structure) used to represent a task's position within the hierarchical structure of tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968653(v=office.12).md">WBSLevel</a></p></td>
<td><p>Optional</p></td>
<td><p>Right-most level of the task. For example, if the task WBS is A.01.03, the right-most level is 03.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968651(v=office.12).md">OutlineNumber</a></p></td>
<td><p>Optional</p></td>
<td><p>Number that indicates the level of a task in the project outline hierarchy.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968465(v=office.12).md">OutlineLevel</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the exact position of a task in the outline.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968643(v=office.12).md">Priority</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the level of importance assigned to a task</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968645(v=office.12).md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task is scheduled to begin.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968534(v=office.12).md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a task is scheduled to be completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968640(v=office.12).md">Duration</a></p></td>
<td><p>Optional</p></td>
<td><p>Total span of active working time for a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968637(v=office.12).md">DurationFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Format used to show the duration of the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968571(v=office.12).md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of work scheduled to be performed on a task by all assigned resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968470(v=office.12).md">Stop</a></p></td>
<td><p>Optional</p></td>
<td><p>Date that represents the end of the actual portion of a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968423(v=office.12).md">Resume</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the remaining portion of a task is scheduled to resume.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968677(v=office.12).md">ResumeValid</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task can be resumed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968574(v=office.12).md">EffortDriven</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether scheduling for a task is effort-driven.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968731(v=office.12).md">Recurring</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a recurring task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968615(v=office.12).md">OverAllocated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an assigned resource on a task has more work than can be done within the normal working capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968711(v=office.12).md">Estimated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task's duration is flagged as an estimate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968520(v=office.12).md">Milestone</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a milestone.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968468(v=office.12).md">Summary</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a summary task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968692(v=office.12).md">Critical</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task has room in the schedule to slip, or if it is on the critical path.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968630(v=office.12).md">IsSubproject</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task is an inserted project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968461(v=office.12).md">IsSubprojectReadOnly</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the inserted project is a read-only project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968656(v=office.12).md">SubprojectName</a></p></td>
<td><p>Optional</p></td>
<td><p>Source location of the inserted project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968595(v=office.12).md">ExternalTask</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task is linked from another project or whether it originated in the current project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968537(v=office.12).md">ExternalTaskProject</a></p></td>
<td><p>Optional</p></td>
<td><p>Source of an external task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968432(v=office.12).md">EarlyStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The earliest date that a task can begin, based on the early start dates of predecessor and successor tasks and other constraints.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968483(v=office.12).md">EarlyFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The earliest date that a task can finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968576(v=office.12).md">LateStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The latest date that a task can start without delaying the finish of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968671(v=office.12).md">LateFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The latest date that a task can finish without delaying the finish of the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968588(v=office.12).md">StartVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a task's baseline start date and its currently scheduled start date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968724(v=office.12).md">FinishVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that represents the difference between a task's baseline finish date and its current finish date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968689(v=office.12).md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a task's baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968623(v=office.12).md">FreeSlack</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that a task can be delayed without delaying any successor tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968632(v=office.12).md">TotalSlack</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time a task can be delayed without delaying a project's finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968494(v=office.12).md">FixedCost</a></p></td>
<td><p>Optional</p></td>
<td><p>A task expense that is not associated with a resource cost.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968493(v=office.12).md">FixedCostAccrual</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how fixed costs are to be charged, or accrued, to the cost of a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968546(v=office.12).md">PercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of a task, expressed as the percentage of the task's duration that has been completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968608(v=office.12).md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of a task, expressed as the percentage of the task's work that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968522(v=office.12).md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled, or projected, cost for a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968407(v=office.12).md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Sum of the actual overtime cost for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968609(v=office.12).md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of overtime scheduled to be performed by all resources assigned to a task and charged at overtime rates.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968713(v=office.12).md">ActualStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task actually began.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968472(v=office.12).md">ActualFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task actually finished.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968446(v=office.12).md">ActualDuration</a></p></td>
<td><p>Optional</p></td>
<td><p>Span of actual working time for a task so far, based on the scheduled duration and current remaining work or percent complete.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968591(v=office.12).md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for work already performed by all resources on a task, along with any other recorded costs associated with the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968431(v=office.12).md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for overtime work already performed on a task by all assigned resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968429(v=office.12).md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of work that has already been done by the resources assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968413(v=office.12).md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Actual amount of overtime work already performed by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968582(v=office.12).md">RegularWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of non-overtime work scheduled to be performed by all resources assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968613(v=office.12).md">RemainingDuration</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of non-overtime work scheduled to be performed by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968728(v=office.12).md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of time required to complete the unfinished portion of a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968720(v=office.12).md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Remaining scheduled expense of a task that will be incurred in completing the remaining scheduled work by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968690(v=office.12).md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Remaining scheduled overtime expense for a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968473(v=office.12).md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of remaining overtime scheduled by all assigned resources to complete a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968717(v=office.12).md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for work already done on a task, up to the project status date or today's date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968685(v=office.12).md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>Difference between how much it should have cost to achieve the current level of completion on the task and how much it has actually cost.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968703(v=office.12).md">ConstraintType</a></p></td>
<td><p>Optional</p></td>
<td><p>Start or finish constraint on a scheduled task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968514(v=office.12).md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>Refers to a valid UID for a project calendar.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968552(v=office.12).md">ConstraintDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the constrained start or finish date as defined in ConstraintType.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968639(v=office.12).md">Deadline</a></p></td>
<td><p>Optional</p></td>
<td><p>Date entered as a deadline for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968452(v=office.12).md">LevelAssignments</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the leveling function can delay and split individual assignments (rather than the entire task) to resolve overallocations.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968467(v=office.12).md">LevelingCanSplit</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource leveling function can cause splits on remaining work on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968397(v=office.12).md">LevelingDelay</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of time that a task is to be delayed from its early start date as a result of resource leveling.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968448(v=office.12).md">LevelingDelayFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Format for expressing the duration of the delay.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968725(v=office.12).md">PreLeveledStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Start date of a task as it was before resource leveling was done.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968501(v=office.12).md">PreLeveledFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>Finish date of a task as it was before resource leveling was done.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968729(v=office.12).md">Hyperlink</a></p></td>
<td><p>Optional</p></td>
<td><p>Title or explanatory text for a hyperlink associated with a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968561(v=office.12).md">HyperlinkAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>Address for a hyperlink associated with a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968602(v=office.12).md">HyperlinkSubAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>Specific location in a document within a hyperlink associated with a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968540(v=office.12).md">IgnoreResourceCalendar</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the scheduling of the task takes into account the calendars of the resources assigned to the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968616(v=office.12).md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes entered about a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968691(v=office.12).md">HideBar</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the Gantt bars and Calendar bars for a task are hidden.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968489(v=office.12).md">Rollup</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the summary task in a Gantt chart displays information rolled up from subtasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968411(v=office.12).md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>Cumulative timephased baseline costs up to the status date or today's date; also known as budgeted cost of work scheduled.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968714(v=office.12).md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>Cumulative value of the task's timephased percent complete multiplied by the task's timephased baseline cost, up to the status date or today's date; also known as budgeted cost of work performed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968424(v=office.12).md">PhysicalPercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>Physical percent of the total work on a task that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968620(v=office.12).md">EarnedValueMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the type of earned value method to use.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968712(v=office.12).md">PredecessorLink</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the predecessor task of the current task.</p></td>
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
<td><p><a href="bb968599(v=office.12).md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of baseline values of the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968507(v=office.12).md">IsPublished</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Microsoft Office Project 2007. Indicates whether the task is published.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968633(v=office.12).md">StatusManager</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Name of the task status manager.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968530(v=office.12).md">CommitmentStart</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Start date of the deliverable.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968464(v=office.12).md">CommitmentFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Finish date of the deliverable.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968709(v=office.12).md">CommitmentType</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the task has an associated deliverable or a dependency on an associated deliverable.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968719(v=office.12).md">b408000 – b417fff</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. A task-level enterprise custom field value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968536(v=office.12).md">b608000 – b617fff</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. A project-level enterprise custom field value.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968669(v=office.12).md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the value of a task custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968410(v=office.12).md">OutlineCode</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the value of a task outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968479(v=office.12).md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>Timephased data associated with the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968701(v=office.12).md">Project</a></p></td>
<td><p>Optional</p></td>
<td><p>If the task is a subproject, specifies the inserted subproject data.</p></td>
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

## Example

In the following example, the task UID = 4 although the task ID = 3, because a task was deleted before task T3 was created. UID values must be unique within a project. Because there is no custom WBSMask defined, the task WBS value is the same as the OutlineNumber.

``` xml
<Task>
   <UID>4</UID>
   <ID>3</ID>
   <Name>T3</Name>
   <Type>1</Type>
   <IsNull>0</IsNull>
   <CreateDate>2007-11-13T14:33:00</CreateDate>
   <WBS>1.2</WBS>
   <WBSLevel>2</WBSLevel>
   <OutlineNumber>1.2</OutlineNumber>
   <OutlineLevel>2</OutlineLevel>
   <Priority>500</Priority>
   <Start>2007-11-14T08:00:00</Start>
   <Finish>2007-11-15T17:00:00</Finish>
   <Duration>PT16H0M0S</Duration>
   <DurationFormat>53</DurationFormat>
   <Work>PT0H0M0S</Work>
   <ResumeValid>0</ResumeValid>
   <EffortDriven>0</EffortDriven>
   <Recurring>0</Recurring>
   <OverAllocated>0</OverAllocated>
   <Estimated>1</Estimated>
   <Milestone>0</Milestone>
   <Summary>1</Summary>
   <Critical>1</Critical>
   <IsSubproject>0</IsSubproject>
   <IsSubprojectReadOnly>0</IsSubprojectReadOnly>
   <ExternalTask>0</ExternalTask>
   <EarlyStart>2007-11-14T08:00:00</EarlyStart>
   <EarlyFinish>2007-11-15T17:00:00</EarlyFinish>
   <LateStart>2007-11-14T08:00:00</LateStart>
   <LateFinish>2007-11-15T17:00:00</LateFinish>
   <StartVariance>0</StartVariance>
   <FinishVariance>0</FinishVariance>
   <WorkVariance>0</WorkVariance>
   <FreeSlack>0</FreeSlack>
   <TotalSlack>0</TotalSlack>
   <FixedCost>0</FixedCost>
   <FixedCostAccrual>3</FixedCostAccrual>
   <PercentComplete>0</PercentComplete>
   <PercentWorkComplete>0</PercentWorkComplete>
   <Cost>0</Cost>
   <OvertimeCost>0</OvertimeCost>
   <OvertimeWork>PT0H0M0S</OvertimeWork>
   <ActualDuration>PT0H0M0S</ActualDuration>
   <ActualCost>0</ActualCost>
   <ActualOvertimeCost>0</ActualOvertimeCost>
   <ActualWork>PT0H0M0S</ActualWork>
   <ActualOvertimeWork>PT0H0M0S</ActualOvertimeWork>
   <RegularWork>PT0H0M0S</RegularWork>
   <RemainingDuration>PT16H0M0S</RemainingDuration>
   <RemainingCost>0</RemainingCost>
   <RemainingWork>PT0H0M0S</RemainingWork>
   <RemainingOvertimeCost>0</RemainingOvertimeCost>
   <RemainingOvertimeWork>PT0H0M0S</RemainingOvertimeWork>
   <ACWP>0</ACWP>
   <CV>0</CV>
   <ConstraintType>0</ConstraintType>
   <CalendarUID>-1</CalendarUID>
   <LevelAssignments>1</LevelAssignments>
   <LevelingCanSplit>1</LevelingCanSplit>
   <LevelingDelay>0</LevelingDelay>
   <LevelingDelayFormat>8</LevelingDelayFormat>
   <IgnoreResourceCalendar>0</IgnoreResourceCalendar>
   <HideBar>0</HideBar>
   <Rollup>1</Rollup>
   <BCWS>0</BCWS>
   <BCWP>0</BCWP>
   <PhysicalPercentComplete>0</PhysicalPercentComplete>
   <EarnedValueMethod>0</EarnedValueMethod>
   <IsPublished>1</IsPublished>
   <CommitmentType>0</CommitmentType>
</Task>
```

## See Also

#### Concepts

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

