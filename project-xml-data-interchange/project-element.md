---
title: Project Element
TOCTitle: Project Element
ms:assetid: d6c47ee7-56f0-480f-940c-a7b715e6c1c3
ms:mtpsurl: https://msdn.microsoft.com/en-us/library/Bb968701(v=office.12)
ms:contentKeyID: 13188391
ms.date: 05/05/2014
mtps_version: v=office.12
f1_keywords:
- Project element
monikerRange: '>= project-client-2007 || project-client-odc'
---

# Project Element




Project is the top level element of the document. Project child elements include all data for each project, including calendars, assignments, tasks, resources, extended attributes (custom fields), work breakdown structure (WBS codes), and custom outline codes.

    <Project>
      ComplexTypeValue
    </Project>

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
<td><p><a href="bb968654(v=office.12).md">SaveVersion</a></p></td>
<td><p>Required</p></td>
<td><p>New. The version of Project that saved the project XML file. SaveVersion = 12 for Microsoft Office Project 2007.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968590(v=office.12).md">UID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID string for the project. Deprecated in Project 2007.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968600(v=office.12).md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Project file name, for example, ProjectName.xml.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968746(v=office.12).md">Title</a></p></td>
<td><p>Optional</p></td>
<td><p>Title of the project. Deprecated in Project 2007.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968657(v=office.12).md">Subject</a></p></td>
<td><p>Optional</p></td>
<td><p>Subject of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968456(v=office.12).md">Category</a></p></td>
<td><p>Optional</p></td>
<td><p>Category the project belongs to.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968707(v=office.12).md">Company</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the company that created the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968670(v=office.12).md">Manager</a></p></td>
<td><p>Optional</p></td>
<td><p>Manager of the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968681(v=office.12).md">Author</a></p></td>
<td><p>Optional</p></td>
<td><p>Author of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968396(v=office.12).md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the project was created.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968601(v=office.12).md">Revision</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of times that the project has been saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968736(v=office.12).md">LastSaved</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the project was last saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968741(v=office.12).md">ScheduleFromStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project is scheduled from its start date or finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968562(v=office.12).md">StartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a project is scheduled to begin; required if ScheduleFromStart is true.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968517(v=office.12).md">FinishDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a project is scheduled to end; required if ScheduleFromStart is false.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968568(v=office.12).md">FYStartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Month the fiscal year begins.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968531(v=office.12).md">CriticalSlackLimit</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of days past its end date that a task can go before Project marks that task as a critical task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968638(v=office.12).md">CurrencyDigits</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of digits that appear after the decimal when Project shows currency values.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968502(v=office.12).md">CurrencySymbol</a></p></td>
<td><p>Optional</p></td>
<td><p>Currency symbol used to represent the type of currency used in the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968575(v=office.12).md">CurrencyCode</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Three-letter currency character code as defined in ISO 4217; for example, EUR for Euros.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968631(v=office.12).md">CurrencySymbolPosition</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the placement of the currency symbol in relation to the currency value:</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968514(v=office.12).md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the calendar used in the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968578(v=office.12).md">DefaultStartTime</a></p></td>
<td><p>Optional</p></td>
<td><p>Default start time for all new tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968593(v=office.12).md">DefaultFinishTime</a></p></td>
<td><p>Optional</p></td>
<td><p>Default finish time for all new tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968518(v=office.12).md">MinutesPerDay</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of minutes per day.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968627(v=office.12).md">MinutesPerWeek</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of minutes per week.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968592(v=office.12).md">DaysPerMonth</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of working days per month.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968603(v=office.12).md">DefaultTaskType</a></p></td>
<td><p>Optional</p></td>
<td><p>Default type for all new tasks in the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968743(v=office.12).md">DefaultFixedCostAccrual</a></p></td>
<td><p>Optional</p></td>
<td><p>Default part of the project when fixed costs are accrued (start, prorated, or end).</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968449(v=office.12).md">DefaultStandardRate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default standard rate for new resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968402(v=office.12).md">DefaultOvertimeRate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default overtime rate for new resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968637(v=office.12).md">DurationFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Default format for all durations in the project</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968538(v=office.12).md">WorkFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Default format for all work durations in the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968544(v=office.12).md">EditableActualCosts</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project automatically calculates actual costs.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968614(v=office.12).md">HonorConstraints</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project schedules tasks according to their constraint dates instead of any task dependencies.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968620(v=office.12).md">EarnedValueMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Default method for calculating earned value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968740(v=office.12).md">InsertedProjectsLikeSummary</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether inserted projects are treated as summary tasks rather than as separate projects for schedule calculation.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968750(v=office.12).md">MultipleCriticalPaths</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project calculates and displays a critical path for each independent network of tasks within a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968412(v=office.12).md">NewTasksEffortDriven</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new tasks are effort-driven.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968708(v=office.12).md">NewTasksEstimated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new tasks have estimated durations.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968513(v=office.12).md">SplitsInProgressTasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether in-progress tasks may be split.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968605(v=office.12).md">SpreadActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether actual costs are spread to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968498(v=office.12).md">SpreadPercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether percent complete is spread to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968594(v=office.12).md">TaskUpdatesResource</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether updates to tasks update resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968550(v=office.12).md">FiscalYearStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether fiscal year numbering is used.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968442(v=office.12).md">WeekStartDay</a></p></td>
<td><p>Optional</p></td>
<td><p>Start day of the week.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968457(v=office.12).md">MoveCompletedEndsBack</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the end of completed portions of tasks scheduled to begin after the status date, but begun early, should be moved back to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968650(v=office.12).md">MoveRemainingStartsBack</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether remaining portions of tasks scheduled to begin after the status date, but begun early, should be moved back to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968418(v=office.12).md">MoveRemainingStartsForward</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether remaining portions of tasks scheduled to have begun late should be moved up to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968463(v=office.12).md">MoveCompletedEndsForward</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether completed portions of tasks scheduled to have been completed before the status date, but begun late, should be moved up to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968527(v=office.12).md">BaselineForEarnedValue</a></p></td>
<td><p>Optional</p></td>
<td><p>Specific baseline used to calculate variance values.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968742(v=office.12).md">AutoAddNewResourcesAndTasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to automatically add new resources to the resource pool.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968628(v=office.12).md">StatusDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date used for calculation and reporting.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968629(v=office.12).md">CurrentDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The system date that Project generated the XML file.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968553(v=office.12).md">MicrosoftProjectServerURL</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project was created by a user who logged on with Windows authentication or Forms authentication.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968458(v=office.12).md">Autolink</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to automatically link inserted or moved tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968699(v=office.12).md">NewTaskStartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default start date for a new task.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968440(v=office.12).md">DefaultTaskEVMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Default earned value method for tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968674(v=office.12).md">ProjectExternallyEdited</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project was edited externally.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968606(v=office.12).md">ExtendedCreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date used for calculation and reporting.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968482(v=office.12).md">ActualsInSync</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether all actual work is synchronized with the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968622(v=office.12).md">RemoveFileProperties</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to remove certain file properties on save, such as Author, Manager, and Company.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968694(v=office.12).md">AdminProject</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project is an administrative project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968732(v=office.12).md">OutlineCodes</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of local outline code definitions in a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968580(v=office.12).md">WBSMasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Table of entries that define a work breakdown structure (WBS) mask.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968426(v=office.12).md">ExtendedAttributes</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of extended attribute (custom field) definitions in a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968499(v=office.12).md">Calendars</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of calendars associated with a project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968617(v=office.12).md">Tasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of tasks that make up a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="bb968730(v=office.12).md">Resources</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of resources that make up a project.</p></td>
</tr>
<tr class="even">
<td><p><a href="bb968684(v=office.12).md">Assignments</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of assignments in a project.</p></td>
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


> [!NOTE]
> There is a rounding error with the MoveCompletedEndsBack, MoveRemainingStartsBack, MoveRemainingStartsForward, and MoveCompletedEndsForward elements. The internal work values for these elements have eight digits; the values lose .001 seconds for every minute, causing a rounding error.


## See Also

#### Concepts

[Project Elements and XML Structure](bb968439\(v=office.12\).md)

[XML Schema for the Project Element](bb968695\(v=office.12\).md)

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

[OutlineCode Elements and XML Structure](bb968596\(v=office.12\).md)

[XML Schema for the OutlineCodes Element](bb968584\(v=office.12\).md)

[WBSMask Elements and XML Structure](bb968416\(v=office.12\).md)

[XML Schema for the WBSMasks Element](bb968565\(v=office.12\).md)

[ExtendedAttribute Elements and XML Structure](bb968579\(v=office.12\).md)

[XML Schema for the ExtendedAttributes Element](bb968705\(v=office.12\).md)

[Calendar Elements and XML Structure](bb968563\(v=office.12\).md)

[XML Schema for the Calendars Element](bb968557\(v=office.12\).md)

[Task Elements and XML Structure](bb968475\(v=office.12\).md)

[XML Schema for the Tasks Element](bb968415\(v=office.12\).md)

[Resource Elements and XML Structure](bb968445\(v=office.12\).md)

[XML Schema for the Resources Element](bb968511\(v=office.12\).md)

[Assignment Elements and XML Structure](bb968738\(v=office.12\).md)

[XML Schema for the Assignments Element](bb968414\(v=office.12\).md)

[TimephasedDataType Elements and XML Structure](bb968722\(v=office.12\).md)

[XML Schema for the TimephasedDataType Complex Type](bb968734\(v=office.12\).md)

