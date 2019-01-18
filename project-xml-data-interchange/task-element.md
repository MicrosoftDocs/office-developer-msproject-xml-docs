---
title: Task Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
localization_priority: Normal
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
<td><p><a href="tasks-element.md">Tasks</a></p></td>
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
<tr class="even">
<td><p><a href="guid-element-multiple-parents.md">GUID</a></p></td>
<td><p>Optional</p></td>
<td><p>GUID for the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>Required</p></td>
<td><p>Unique ID for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="id-element.md">ID</a></p></td>
<td><p>Optional</p></td>
<td><p>Position identifier of the task in the list of tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="type-element-multiple-parents.md">Type</a></p></td>
<td><p>Optional</p></td>
<td><p>Type of the task (fixed units, fixed duration, or fixed work).</p></td>
</tr>
<tr class="odd">
<td><p><a href="isnull-element.md">IsNull</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is null.</p></td>
</tr>
<tr class="even">
<td><p><a href="createdate-element.md">CreateDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task was added to a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="contact-element.md">Contact</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the individual who is responsible for a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="wbs-element.md">WBS</a></p></td>
<td><p>Optional</p></td>
<td><p>A unique code (work breakdown structure) used to represent a task's position within the hierarchical structure of tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="wbslevel-element.md">WBSLevel</a></p></td>
<td><p>Optional</p></td>
<td><p>Right-most level of the task. For example, if the task WBS is A.01.03, the right-most level is 03.</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinenumber-element.md">OutlineNumber</a></p></td>
<td><p>Optional</p></td>
<td><p>Number that indicates the level of a task in the project outline hierarchy.</p></td>
</tr>
<tr class="odd">
<td><p><a href="outlinelevel-element.md">OutlineLevel</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the exact position of a task in the outline.</p></td>
</tr>
<tr class="even">
<td><p><a href="priority-element.md">Priority</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the level of importance assigned to a task</p></td>
</tr>
<tr class="odd">
<td><p><a href="start-element.md">Start</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task is scheduled to begin.</p></td>
</tr>
<tr class="even">
<td><p><a href="finish-element.md">Finish</a></p></td>
<td><p>Optional</p></td>
<td><p>The date and time that a task is scheduled to be completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="duration-element.md">Duration</a></p></td>
<td><p>Optional</p></td>
<td><p>Total span of active working time for a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="durationformat-element.md">DurationFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Format used to show the duration of the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="work-element.md">Work</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of work scheduled to be performed on a task by all assigned resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="stop-element.md">Stop</a></p></td>
<td><p>Optional</p></td>
<td><p>Date that represents the end of the actual portion of a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="resume-element.md">Resume</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the remaining portion of a task is scheduled to resume.</p></td>
</tr>
<tr class="even">
<td><p><a href="resumevalid-element.md">ResumeValid</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task can be resumed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="effortdriven-element.md">EffortDriven</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether scheduling for a task is effort-driven.</p></td>
</tr>
<tr class="even">
<td><p><a href="recurring-element.md">Recurring</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a recurring task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overallocated-element.md">OverAllocated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether an assigned resource on a task has more work than can be done within the normal working capacity.</p></td>
</tr>
<tr class="even">
<td><p><a href="estimated-element.md">Estimated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task's duration is flagged as an estimate.</p></td>
</tr>
<tr class="odd">
<td><p><a href="milestone-element.md">Milestone</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a milestone.</p></td>
</tr>
<tr class="even">
<td><p><a href="summary-element.md">Summary</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task is a summary task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="critical-element.md">Critical</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether a task has room in the schedule to slip, or if it is on the critical path.</p></td>
</tr>
<tr class="even">
<td><p><a href="issubproject-element.md">IsSubproject</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task is an inserted project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="issubprojectreadonly-element.md">IsSubprojectReadOnly</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the inserted project is a read-only project.</p></td>
</tr>
<tr class="even">
<td><p><a href="subprojectname-element.md">SubprojectName</a></p></td>
<td><p>Optional</p></td>
<td><p>Source location of the inserted project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="externaltask-element.md">ExternalTask</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the task is linked from another project or whether it originated in the current project.</p></td>
</tr>
<tr class="even">
<td><p><a href="externaltaskproject-element.md">ExternalTaskProject</a></p></td>
<td><p>Optional</p></td>
<td><p>Source of an external task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="earlystart-element.md">EarlyStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The earliest date that a task can begin, based on the early start dates of predecessor and successor tasks and other constraints.</p></td>
</tr>
<tr class="even">
<td><p><a href="earlyfinish-element.md">EarlyFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The earliest date that a task can finish, based on early finish dates of predecessor and successor tasks, other constraints, and any leveling delay.</p></td>
</tr>
<tr class="odd">
<td><p><a href="latestart-element.md">LateStart</a></p></td>
<td><p>Optional</p></td>
<td><p>The latest date that a task can start without delaying the finish of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="latefinish-element.md">LateFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>The latest date that a task can finish without delaying the finish of the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="startvariance-element.md">StartVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a task's baseline start date and its currently scheduled start date.</p></td>
</tr>
<tr class="even">
<td><p><a href="finishvariance-element.md">FinishVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that represents the difference between a task's baseline finish date and its current finish date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="workvariance-element.md">WorkVariance</a></p></td>
<td><p>Optional</p></td>
<td><p>The difference between a task's baseline work and the currently scheduled work.</p></td>
</tr>
<tr class="even">
<td><p><a href="freeslack-element.md">FreeSlack</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time that a task can be delayed without delaying any successor tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="totalslack-element.md">TotalSlack</a></p></td>
<td><p>Optional</p></td>
<td><p>The amount of time a task can be delayed without delaying a project's finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="fixedcost-element-baseline.md">FixedCost</a></p></td>
<td><p>Optional</p></td>
<td><p>A task expense that is not associated with a resource cost.</p></td>
</tr>
<tr class="odd">
<td><p><a href="fixedcostaccrual-element.md">FixedCostAccrual</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates how fixed costs are to be charged, or accrued, to the cost of a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="percentcomplete-element.md">PercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of a task, expressed as the percentage of the task's duration that has been completed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="percentworkcomplete-element.md">PercentWorkComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>The current status of a task, expressed as the percentage of the task's work that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="cost-element.md">Cost</a></p></td>
<td><p>Optional</p></td>
<td><p>The total scheduled, or projected, cost for a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="overtimecost-element.md">OvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Sum of the actual overtime cost for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="overtimework-element.md">OvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of overtime scheduled to be performed by all resources assigned to a task and charged at overtime rates.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualstart-element.md">ActualStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task actually began.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualfinish-element.md">ActualFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a task actually finished.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualduration-element.md">ActualDuration</a></p></td>
<td><p>Optional</p></td>
<td><p>Span of actual working time for a task so far, based on the scheduled duration and current remaining work or percent complete.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualcost-element.md">ActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for work already performed by all resources on a task, along with any other recorded costs associated with the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimecost-element.md">ActualOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for overtime work already performed on a task by all assigned resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualwork-element.md">ActualWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of work that has already been done by the resources assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimework-element.md">ActualOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Actual amount of overtime work already performed by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="regularwork-element.md">RegularWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of non-overtime work scheduled to be performed by all resources assigned to a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingduration-element.md">RemainingDuration</a></p></td>
<td><p>Optional</p></td>
<td><p>Total amount of non-overtime work scheduled to be performed by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingcost-element.md">RemainingCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of time required to complete the unfinished portion of a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingwork-element.md">RemainingWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Remaining scheduled expense of a task that will be incurred in completing the remaining scheduled work by all resources assigned to a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="remainingovertimecost-element.md">RemainingOvertimeCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Remaining scheduled overtime expense for a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="remainingovertimework-element.md">RemainingOvertimeWork</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of remaining overtime scheduled by all assigned resources to complete a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="acwp-element.md">ACWP</a></p></td>
<td><p>Optional</p></td>
<td><p>Costs incurred for work already done on a task, up to the project status date or today's date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="cv-element.md">CV</a></p></td>
<td><p>Optional</p></td>
<td><p>Difference between how much it should have cost to achieve the current level of completion on the task and how much it has actually cost.</p></td>
</tr>
<tr class="even">
<td><p><a href="constrainttype-element.md">ConstraintType</a></p></td>
<td><p>Optional</p></td>
<td><p>Start or finish constraint on a scheduled task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>Refers to a valid UID for a project calendar.</p></td>
</tr>
<tr class="even">
<td><p><a href="constraintdate-element.md">ConstraintDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the constrained start or finish date as defined in ConstraintType.</p></td>
</tr>
<tr class="odd">
<td><p><a href="deadline-element.md">Deadline</a></p></td>
<td><p>Optional</p></td>
<td><p>Date entered as a deadline for the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="levelassignments-element.md">LevelAssignments</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the leveling function can delay and split individual assignments (rather than the entire task) to resolve overallocations.</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingcansplit-element.md">LevelingCanSplit</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the resource leveling function can cause splits on remaining work on a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="levelingdelay-element.md">LevelingDelay</a></p></td>
<td><p>Optional</p></td>
<td><p>Amount of time that a task is to be delayed from its early start date as a result of resource leveling.</p></td>
</tr>
<tr class="odd">
<td><p><a href="levelingdelayformat-element.md">LevelingDelayFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Format for expressing the duration of the delay.</p></td>
</tr>
<tr class="even">
<td><p><a href="preleveledstart-element.md">PreLeveledStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Start date of a task as it was before resource leveling was done.</p></td>
</tr>
<tr class="odd">
<td><p><a href="preleveledfinish-element.md">PreLeveledFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>Finish date of a task as it was before resource leveling was done.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlink-element.md">Hyperlink</a></p></td>
<td><p>Optional</p></td>
<td><p>Title or explanatory text for a hyperlink associated with a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="hyperlinkaddress-element.md">HyperlinkAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>Address for a hyperlink associated with a task.</p></td>
</tr>
<tr class="even">
<td><p><a href="hyperlinksubaddress-element.md">HyperlinkSubAddress</a></p></td>
<td><p>Optional</p></td>
<td><p>Specific location in a document within a hyperlink associated with a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="ignoreresourcecalendar-element.md">IgnoreResourceCalendar</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the scheduling of the task takes into account the calendars of the resources assigned to the task.</p></td>
</tr>
<tr class="even">
<td><p><a href="notes-element.md">Notes</a></p></td>
<td><p>Optional</p></td>
<td><p>Notes entered about a task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="hidebar-element.md">HideBar</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the Gantt bars and Calendar bars for a task are hidden.</p></td>
</tr>
<tr class="even">
<td><p><a href="rollup-element.md">Rollup</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the summary task in a Gantt chart displays information rolled up from subtasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bcws-element.md">BCWS</a></p></td>
<td><p>Optional</p></td>
<td><p>Cumulative timephased baseline costs up to the status date or today's date; also known as budgeted cost of work scheduled.</p></td>
</tr>
<tr class="even">
<td><p><a href="bcwp-element.md">BCWP</a></p></td>
<td><p>Optional</p></td>
<td><p>Cumulative value of the task's timephased percent complete multiplied by the task's timephased baseline cost, up to the status date or today's date; also known as budgeted cost of work performed.</p></td>
</tr>
<tr class="odd">
<td><p><a href="physicalpercentcomplete-element.md">PhysicalPercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>Physical percent of the total work on a task that has been completed.</p></td>
</tr>
<tr class="even">
<td><p><a href="earnedvaluemethod-element.md">EarnedValueMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the type of earned value method to use.</p></td>
</tr>
<tr class="odd">
<td><p><a href="predecessorlink-element.md">PredecessorLink</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the predecessor task of the current task.</p></td>
</tr>
<tr class="even">
<td><p><a href="actualworkprotected-element.md">ActualWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual work is protected.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualovertimeworkprotected-element.md">ActualOvertimeWorkProtected</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the duration through which actual overtime work is protected.</p></td>
</tr>
<tr class="even">
<td><p><a href="baseline-element.md">Baseline</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of baseline values of the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="ispublished-element.md">IsPublished</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Microsoft Office Project 2007. Indicates whether the task is published.</p></td>
</tr>
<tr class="even">
<td><p><a href="statusmanager-element.md">StatusManager</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Name of the task status manager.</p></td>
</tr>
<tr class="odd">
<td><p><a href="commitmentstart-element.md">CommitmentStart</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Start date of the deliverable.</p></td>
</tr>
<tr class="even">
<td><p><a href="commitmentfinish-element.md">CommitmentFinish</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Finish date of the deliverable.</p></td>
</tr>
<tr class="odd">
<td><p><a href="commitmenttype-element.md">CommitmentType</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Indicates whether the task has an associated deliverable or a dependency on an associated deliverable.</p></td>
</tr>
<tr class="even">
<td><p><a href="b408000-b417fff-elements.md">b408000 – b417fff</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. A task-level enterprise custom field value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="b608000-b617fff-elements.md">b608000 – b617fff</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. A project-level enterprise custom field value.</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattribute-element.md">ExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the value of a task custom field.</p></td>
</tr>
<tr class="odd">
<td><p><a href="outlinecode-element.md">OutlineCode</a></p></td>
<td><p>Optional</p></td>
<td><p>Specifies the value of a task outline code.</p></td>
</tr>
<tr class="even">
<td><p><a href="timephaseddata-element.md">TimephasedData</a></p></td>
<td><p>Optional</p></td>
<td><p>Timephased data associated with the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="project-element.md">Project</a></p></td>
<td><p>Optional</p></td>
<td><p>If the task is a subproject, specifies the inserted subproject data.</p></td>
</tr>
<tr class="even">
<td><p><a href="notecontainsobjects-element.md">NoteContainsObjects</a></p></td>
<td><p>Optional</p></td>
<td><p>This value is true if the note for a task contains an object.</p></td>
</tr>
<tr class="odd">
<td><p><a href="enterpriseextendedattribute-element.md">
EnterpriseExtendedAttribute</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of Enterprise Custom Fields with lookup table values.</p></td>
</tr>
</tbody>
</table>

::: moniker range="project-client-odc"

The following items were added for Project Online Desktop Client

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
<tr class="even">
<td><p><a href="boardstatuscolumnorderingid-element.md">BoardStatusColumnOrderingID</a></p></td>
<td><p>Optional</p></td>
<td><p>Used for ordering tasks in the Task Board view when the view is arranged by the Board Status column.</p></td>
</tr>
<tr class="odd">
<td><p><a href="sprintcolumnorderingid-element.md">SprintColumnOrderingID</a></p></td>
<td><p>Optional</p></td>
<td><p>Used for ordering tasks in the Task Board view when the view is arranged by the Board Status column.</p></td>
</tr>
<tr class="even">
<td><p><a href="nextavailableboardstatuscolumnorderingid-element.md">NextAvailableBoardStatusColumnOrderingID</a></p></td>
<td><p>Optional</p></td>
<td><p>Used internally for ordering tasks in the Task Board view when the view is arranged by the Board Status column.</p></td>
</tr>
<tr class="odd">
<td><p><a href="nextavailablesprintorderingid-element.md">NextAvailableSprintOrderingID</a></p></td>
<td><p>Optional</p></td>
<td><p>Used internally for ordering tasks in the Task Board view when the view is arranged by Sprints.</p></td>
</tr>
<tr class="even">
<td><p><a href="sprintuid-element.md">SprintUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The UID of the Sprint value associated with the task.</p></td>
</tr>
<tr class="odd">
<td><p><a href="boardcolumnuid-element.md">BoardColumnUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The UID of the Board Column value associated with the task.</p></td>
</tr>
</tbody>
</table>

::: moniker-end

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

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

