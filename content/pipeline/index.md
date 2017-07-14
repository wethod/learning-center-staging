---
date: '2016-03-11T20:10:46+01:00'
title: Pipeline
weight: 30

---


## Overview

Everything starts from Pipeline, here is where opportunities and projects are listed, both of them are defined by a small amount of significant information:

* Name;

* Client;

* Value (in €k);

* Percentage of external costs;

* Category;

* Probability.

Pipeline has three subsections: Basket, Projects and Programs.

{{< img-center src="/uploads/2017/05/25/nav-pipeline.png" >}}

## Basket

The Basket contains all the project’s opportunity that are not well-defined yet. You can see it as a place where to put all the ideas that you usually write on a notebook or on a Post-It.The significant information listed above are not mandatory for an opportunity.

{{< note title="Note" >}}
**Opportunities usually have a probability between 1% and 99%.** {{< /note >}}

## Projects

Here you can find all the projects of the company, each project has significant information you can check and edit. Clicking on a project let you see more details and actions about it.

An opportunity evolves into a Project when things get serious, in order to take this step you must have an idea about the significant information listed above.

A Project can furthermore have an invoice plan and a budget.

A project is considered **started** if it has a start date in the past or if someone has submitted timesheets for it.

A project is considered **active** when its probability reaches 90%, only when this happens makes sense to plan people or to do timeheets for this project. An active project must have a job order.

{{< note title="Note" >}}
**Billable Projects must have a probability of 100%.**

**When a project status reach 0, it's a good practice to archive it.**

**When a project reach 50% of probability, it's a good practice to make a budget for it.**
{{< /note >}}

By clicking on a project you can edit its details or open its: [budget]({{< relref "budget/index.md#budget" >}}), [planning]({{< relref "planning/index.md#planning" >}}), [reports]({{< relref "reports/index.md#reports" >}}), [invoice plan]({{< relref "pipeline/index.md#invoice plan" >}})

{{< img-center src="/uploads/2017/05/25/projects.png" >}}

### Advenced Search

If you need to search for a project, you just need to type the keywords on the top of the section.

In the case in which you need a more specific and advanced search, there are some Search Operators that can help you!

<table>
<thead>
<tr>
<th>If you want to search a project from</th>
<th>Search Operators</th>
</tr>
</thead>
<tbody>
<tr>
<td>the Name</td>
<td><b>project:</b> project’s name</td>
</tr>
<tr>
<td>its ID</td>
<td><b>id: </b>project’s id</td>
</tr>
<tr>
<td>its Value</td>
<td><b>value:</b> project’s value</td>
</tr>
<tr>
<td>the Project Type</td>
<td><b>type:</b> project’s type</td>
</tr>
<tr>
<td>the Probability</td>
<td><b>prob:</b> project’s probability</td>
</tr>
<tr>
<td>the Start Date</td>
<td><b>start:</b> month year</td>
</tr>
<tr>
<td>the End Date</td>
<td><b>end:</b> month year</td>
</tr>
<tr>
<td>its Budget Status</td>
<td><b>status:</b> draft/0 , approval/1, approved/2</td>
</tr>
<tr>
<td>its Invoice Plan Status</td>
<td><b>plan:</b> auto/0, manual/1</td>
</tr>
<tr>
<td>its Invoice Plan Offset</td>
<td><b>offset:</b> on, off</td>
</tr>
<tr>
<td>the Client Name</td>
<td><b>client:</b> client’s name</td>
</tr>
<tr>
<td>the Client PO</td>
<td><b>po:</b> client’s PO</td>
</tr>
<tr>
<td>the PM Name or Surname</td>
<td><b>pm:</b> pm’s name</td>
</tr>
<tr>
<td>the Account Name or Surname</td>
<td><b>account:</b> account’s name/surname</td>
</tr>
<tr>
<td>the Program Name</td>
<td><b>program:</b> program’s name</td>
</tr>
</tbody>
</table>

### Invoice Plan

Here you can set when you plan to emit invoices for the project. This section is basically a calendar with some additional information:

* **Plan**: the amount you plan to invoice for a given month;

* **Invoiced**: the amount actually invoiced for a given month. This is automatically updated each time you create an invoice for the project;

* **Delta**: the difference between Plan and Invoiced for a given month.

An invoice plan can be:

* **Automatic**: an invoice is automatically planned for each project's duration month, the invoice amount is obtained by dividing project's estimate by project's duration;

* **Manual**: you need to manually insert each amount you plan to invoice. If you choose this mode, you can choose an offset amount to move back or forward in time.

You can find the invoices (listed in your plan) in the [Invoices widget]({{< relref "dashboard/index.md#invoices" >}}), there they're ready to be created and sent.

## Programs

Projects are often stages or parts of something bigger, you can use a Program to group together different projects in order to see their aggregate [economic reports]({{< relref "reports/index.md#economics" >}}).