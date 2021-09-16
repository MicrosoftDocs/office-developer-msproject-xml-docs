---
title: Project Element
ms.date: 03/14/2018
monikerRange: '>= project-client-2010 || project-client-odc'
ms.localizationpriority: medium
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
<td><p><a href="saveversion-element.md">SaveVersion</a></p></td>
<td><p>Required</p></td>
<td><p>The version of Project that saved the project XML file. SaveVersion = 12 for Microsoft Office Project 2007.</p></td>
</tr>
<tr class="even">
<td><p><a href="buildnumber-element.md">BuildNumber</a></p></td>
<td><p>Optional</p></td>
<td><p>The build number of Microsoft Project that was used to create the xml file.</p></td>
</tr>
<tr class="odd">
<td><p><a href="guid-element-multiple-parents.md">GUID</a></p></td>
<td><p>Optional</p></td>
<td><p>The globally unique identifier (GUID) of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="uid-element.md">UID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID string for the project. Deprecated in Project 2007.</p></td>
</tr>
<tr class="odd">
<td><p><a href="name-element.md">Name</a></p></td>
<td><p>Optional</p></td>
<td><p>Project file name, for example, ProjectName.xml.</p></td>
</tr>
<tr class="even">
<td><p><a href="title-element-project.md">Title</a></p></td>
<td><p>Optional</p></td>
<td><p>Title of the project. Deprecated in Project 2007.</p></td>
</tr>
<tr class="odd">
<td><p><a href="subject-element.md">Subject</a></p></td>
<td><p>Optional</p></td>
<td><p>Subject of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="category-element.md">Category</a></p></td>
<td><p>Optional</p></td>
<td><p>Category the project belongs to.</p></td>
</tr>
<tr class="odd">
<td><p><a href="company-element.md">Company</a></p></td>
<td><p>Optional</p></td>
<td><p>Name of the company that created the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="manager-element.md">Manager</a></p></td>
<td><p>Optional</p></td>
<td><p>Manager of the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="author-element.md">Author</a></p></td>
<td><p>Optional</p></td>
<td><p>Author of the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="creationdate-element.md">CreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the project was created.</p></td>
</tr>
<tr class="odd">
<td><p><a href="revision-element.md">Revision</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of times that the project has been saved.</p></td>
</tr>
<tr class="even">
<td><p><a href="lastsaved-element.md">LastSaved</a></p></td>
<td><p>Optional</p></td>
<td><p>Date the project was last saved.</p></td>
</tr>
<tr class="odd">
<td><p><a href="schedulefromstart-element.md">ScheduleFromStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project is scheduled from its start date or finish date.</p></td>
</tr>
<tr class="even">
<td><p><a href="startdate-element.md">StartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a project is scheduled to begin; required if ScheduleFromStart is true.</p></td>
</tr>
<tr class="odd">
<td><p><a href="finishdate-element.md">FinishDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date and time that a project is scheduled to end; required if ScheduleFromStart is false.</p></td>
</tr>
<tr class="even">
<td><p><a href="fystartdate-element.md">FYStartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Month the fiscal year begins.</p></td>
</tr>
<tr class="odd">
<td><p><a href="criticalslacklimit-element.md">CriticalSlackLimit</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of days past its end date that a task can go before Project marks that task as a critical task.</p></td>
</tr>
<tr class="even">
<td><p><a href="currencydigits-element.md">CurrencyDigits</a></p></td>
<td><p>Optional</p></td>
<td><p>Number of digits that appear after the decimal when Project shows currency values.</p></td>
</tr>
<tr class="odd">
<td><p><a href="currencysymbol-element.md">CurrencySymbol</a></p></td>
<td><p>Optional</p></td>
<td><p>Currency symbol used to represent the type of currency used in the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="currencycode-element.md">CurrencyCode</a></p></td>
<td><p>Optional</p></td>
<td><p>New in Project 2007. Three-letter currency character code as defined in ISO 4217; for example, EUR for Euros.</p></td>
</tr>
<tr class="odd">
<td><p><a href="currencysymbolposition-element.md">CurrencySymbolPosition</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates the placement of the currency symbol in relation to the currency value:</p></td>
</tr>
<tr class="even">
<td><p><a href="calendaruid-element.md">CalendarUID</a></p></td>
<td><p>Optional</p></td>
<td><p>Unique ID for the calendar used in the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultstarttime-element.md">DefaultStartTime</a></p></td>
<td><p>Optional</p></td>
<td><p>Default start time for all new tasks.</p></td>
</tr>
<tr class="even">
<td><p><a href="defaultfinishtime-element.md">DefaultFinishTime</a></p></td>
<td><p>Optional</p></td>
<td><p>Default finish time for all new tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="minutesperday-element.md">MinutesPerDay</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of minutes per day.</p></td>
</tr>
<tr class="even">
<td><p><a href="minutesperweek-element.md">MinutesPerWeek</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of minutes per week.</p></td>
</tr>
<tr class="odd">
<td><p><a href="dayspermonth-element.md">DaysPerMonth</a></p></td>
<td><p>Optional</p></td>
<td><p>Default number of working days per month.</p></td>
</tr>
<tr class="even">
<td><p><a href="defaulttasktype-element.md">DefaultTaskType</a></p></td>
<td><p>Optional</p></td>
<td><p>Default type for all new tasks in the project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultfixedcostaccrual-element.md">DefaultFixedCostAccrual</a></p></td>
<td><p>Optional</p></td>
<td><p>Default part of the project when fixed costs are accrued (start, prorated, or end).</p></td>
</tr>
<tr class="even">
<td><p><a href="defaultstandardrate-element.md">DefaultStandardRate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default standard rate for new resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="defaultovertimerate-element.md">DefaultOvertimeRate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default overtime rate for new resources.</p></td>
</tr>
<tr class="even">
<td><p><a href="durationformat-element.md">DurationFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Default format for all durations in the project</p></td>
</tr>
<tr class="odd">
<td><p><a href="workformat-element.md">WorkFormat</a></p></td>
<td><p>Optional</p></td>
<td><p>Default format for all work durations in the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="editableactualcosts-element.md">EditableActualCosts</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project automatically calculates actual costs.</p></td>
</tr>
<tr class="odd">
<td><p><a href="honorconstraints-element.md">HonorConstraints</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project schedules tasks according to their constraint dates instead of any task dependencies.</p></td>
</tr>
<tr class="even">
<td><p><a href="earnedvaluemethod-element.md">EarnedValueMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Default method for calculating earned value.</p></td>
</tr>
<tr class="odd">
<td><p><a href="insertedprojectslikesummary-element.md">InsertedProjectsLikeSummary</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether inserted projects are treated as summary tasks rather than as separate projects for schedule calculation.</p></td>
</tr>
<tr class="even">
<td><p><a href="multiplecriticalpaths-element.md">MultipleCriticalPaths</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether Project calculates and displays a critical path for each independent network of tasks within a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="newtaskseffortdriven-element.md">NewTasksEffortDriven</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new tasks are effort-driven.</p></td>
</tr>
<tr class="even">
<td><p><a href="newtasksestimated-element.md">NewTasksEstimated</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether new tasks have estimated durations.</p></td>
</tr>
<tr class="odd">
<td><p><a href="splitsinprogresstasks-element.md">SplitsInProgressTasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether in-progress tasks may be split.</p></td>
</tr>
<tr class="even">
<td><p><a href="spreadactualcost-element.md">SpreadActualCost</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether actual costs are spread to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="spreadpercentcomplete-element.md">SpreadPercentComplete</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether percent complete is spread to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="taskupdatesresource-element.md">TaskUpdatesResource</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether updates to tasks update resources.</p></td>
</tr>
<tr class="odd">
<td><p><a href="fiscalyearstart-element.md">FiscalYearStart</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether fiscal year numbering is used.</p></td>
</tr>
<tr class="even">
<td><p><a href="weekstartday-element.md">WeekStartDay</a></p></td>
<td><p>Optional</p></td>
<td><p>Start day of the week.</p></td>
</tr>
<tr class="odd">
<td><p><a href="movecompletedendsback-element.md">MoveCompletedEndsBack</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the end of completed portions of tasks scheduled to begin after the status date, but begun early, should be moved back to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="moveremainingstartsback-element.md">MoveRemainingStartsBack</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether remaining portions of tasks scheduled to begin after the status date, but begun early, should be moved back to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="moveremainingstartsforward-element.md">MoveRemainingStartsForward</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether remaining portions of tasks scheduled to have begun late should be moved up to the status date.</p></td>
</tr>
<tr class="even">
<td><p><a href="movecompletedendsforward-element.md">MoveCompletedEndsForward</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether completed portions of tasks scheduled to have been completed before the status date, but begun late, should be moved up to the status date.</p></td>
</tr>
<tr class="odd">
<td><p><a href="baselineforearnedvalue-element.md">BaselineForEarnedValue</a></p></td>
<td><p>Optional</p></td>
<td><p>Specific baseline used to calculate variance values.</p></td>
</tr>
<tr class="even">
<td><p><a href="autoaddnewresourcesandtasks-element.md">AutoAddNewResourcesAndTasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to automatically add new resources to the resource pool.</p></td>
</tr>
<tr class="odd">
<td><p><a href="statusdate-element.md">StatusDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date used for calculation and reporting.</p></td>
</tr>
<tr class="even">
<td><p><a href="currentdate-element.md">CurrentDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The system date that Project generated the XML file.</p></td>
</tr>
<tr class="odd">
<td><p><a href="microsoftprojectserverurl-element.md">MicrosoftProjectServerURL</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project was created by a user who logged on with Windows authentication or Forms authentication.</p></td>
</tr>
<tr class="even">
<td><p><a href="autolink-element.md">Autolink</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to automatically link inserted or moved tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="newtaskstartdate-element.md">NewTaskStartDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Default start date for a new task.</p></td>
</tr>
<tr class="even">
<td><p><a href="defaulttaskevmethod-element.md">DefaultTaskEVMethod</a></p></td>
<td><p>Optional</p></td>
<td><p>Default earned value method for tasks.</p></td>
</tr>
<tr class="odd">
<td><p><a href="projectexternallyedited-element.md">ProjectExternallyEdited</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project was edited externally.</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedcreationdate-element.md">ExtendedCreationDate</a></p></td>
<td><p>Optional</p></td>
<td><p>Date used for calculation and reporting.</p></td>
</tr>
<tr class="odd">
<td><p><a href="actualsinsync-element.md">ActualsInSync</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether all actual work is synchronized with the project.</p></td>
</tr>
<tr class="even">
<td><p><a href="removefileproperties-element.md">RemoveFileProperties</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether to remove certain file properties on save, such as Author, Manager, and Company.</p></td>
</tr>
<tr class="odd">
<td><p><a href="adminproject-element.md">AdminProject</a></p></td>
<td><p>Optional</p></td>
<td><p>Indicates whether the project is an administrative project.</p></td>
</tr>
<tr class="even">
<td><p><a href="outlinecodes-element.md">OutlineCodes</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of local outline code definitions in a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="wbsmasks-element.md">WBSMasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Table of entries that define a work breakdown structure (WBS) mask.</p></td>
</tr>
<tr class="even">
<td><p><a href="extendedattributes-element.md">ExtendedAttributes</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of extended attribute (custom field) definitions in a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="calendars-element.md">Calendars</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of calendars associated with a project.</p></td>
</tr>
<tr class="even">
<td><p><a href="tasks-element.md">Tasks</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of tasks that make up a project.</p></td>
</tr>
<tr class="odd">
<td><p><a href="resources-element.md">Resources</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of resources that make up a project.</p></td>
</tr>
<tr class="even">
<td><p><a href="assignments-element.md">Assignments</a></p></td>
<td><p>Optional</p></td>
<td><p>Collection of assignments in a project.</p></td>
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

The following items were added for Project Online Desktop Client.

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
<td><p><a href="sprintlength-element.md">SprintLength</a></p></td>
<td><p>Optional</p></td>
<td><p>The default length in weeks for new sprints.</p></td>
</tr>
<tr class="even">
<td><p><a href="sprintcreationthroughdate-element.md">SprintCreationThroughDate</a></p></td>
<td><p>Optional</p></td>
<td><p>The date that sprints are generated for the project through.</p></td>
</tr>
<tr class="odd">
<td><p><a href="agilemode-element.md">AgileMode</a></p></td>
<td><p>Optional</p></td>
<td><p>A value that represents what mode the project is in.</p></td>
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

[Project Elements and XML Structure](project-elements-and-xml-structure.md)

[XML Schema for the Project Element](xml-schema-for-the-project-element.md)

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

[OutlineCode Elements and XML Structure](outlinecode-elements-and-xml-structure.md)

[XML Schema for the OutlineCodes Element](xml-schema-for-the-outlinecodes-element.md)

[WBSMask Elements and XML Structure](wbsmask-elements-and-xml-structure.md)

[XML Schema for the WBSMasks Element](xml-schema-for-the-wbsmasks-element.md)

[ExtendedAttribute Elements and XML Structure](extendedattribute-elements-and-xml-structure.md)

[XML Schema for the ExtendedAttributes Element](xml-schema-for-the-extendedattributes-element.md)

[Calendar Elements and XML Structure](calendar-elements-and-xml-structure.md)

[XML Schema for the Calendars Element](xml-schema-for-the-calendars-element.md)

[Task Elements and XML Structure](task-elements-and-xml-structure.md)

[XML Schema for the Tasks Element](xml-schema-for-the-tasks-element.md)

[Resource Elements and XML Structure](resource-elements-and-xml-structure.md)

[XML Schema for the Resources Element](xml-schema-for-the-resources-element.md)

[Assignment Elements and XML Structure](assignment-elements-and-xml-structure.md)

[XML Schema for the Assignments Element](xml-schema-for-the-assignments-element.md)

[TimephasedDataType Elements and XML Structure](timephaseddatatype-elements-and-xml-structure.md)

[XML Schema for the TimephasedDataType Complex Type](xml-schema-for-the-timephaseddatatype-complex-type.md)

