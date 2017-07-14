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

### Advanced Search

If you need to search for a project, you just need to type the keywords on the Search Input.

In the case in which you need a more specific and advanced search, there are some Search Operators that can help you:

<table>
<thead>
<tr>
<th>If you are looking for a project where:</th>
<th>Type in:</th>
<th>Note</th>
</tr>
</thead>
<tbody>
<tr>
<td>the Name is Project1</td>
<td><i>project:project1</i></td>
<td></td>
</tr>
<tr>
<td>the ID is 8</td>
<td><i>id:8</i></td>
<td></td>
</tr>
<tr>
<td>the Value is 25</td>
<td><i>value:25</i></td>
<td></td>
</tr>
<tr>
<td>the Project Type is Internal</td>
<td><i>type:interna</i></td>
<td></td>
</tr>
<tr>
<td>the Probability is 50</td>
<td><i>prob:50</i></td>
<td></td>
</tr>
<tr>
<td>the Start Date is January 2016</td>
<td><i>start:0116</i></td>
<td>Write first the month and then the year</td>
</tr>
<tr>
<td>the End Date is December 2017</td>
<td><i>end:1217</i></td>
<td>Write firts the month and then the year</td>
</tr>
<tr>
<td>the Budget Status is Draft</td>
<td><i>status:0</i></td>
<td>Available values: <b>0(draft)</b>, <b>1(approval)</b>, <b>2(approved)</b></td>
</tr>
<tr>
<td>the Invoice Plan Status is manual</td>
<td><i>plan:1</i></td>
<td>Available values: <b>0(auto)</b>, <b>1(manual)</b></td>
</tr>
<tr>
<td>the Invoice Plan Offset is on</td>
<td><i>offset:on</i></td>
<td>Available values <b>on</b>, <b>off</b></td>
</tr>
<tr>
<td>the Client Name is wethodspa</td>
<td><i>client:wethodspa</i></td>
<td></td>
</tr>
<tr>
<td>the Client PO is 30</td>
<td><i>po:30</i></td>
<td></td>
</tr>
<tr>
<td>the PM Name or Surname is Luca</td>
<td><i>pm:luca</i></td>
<td></td>
</tr>
<tr>
<td>the Account Name or Surname is gb</td>
<td><i>account:gb</i></td>
<td></td>
</tr>
<tr>
<td>the Program Name is wethod</td>
<td><i>program:wethod</i></td>
<td></td>
</tr>
</tbody>
</table>

There are also some **Operators** that can help you searching projects, let’s have a look on them:

* If you want to search a project from**values greater than or equal** to x:    **“ x+ ”**

* If you want to search a project from **values less than or equal** to x:    **“ x- ”**

* If you want to search a project from **values greater or equal** to x **and less or equal** to y:  **“ x…y ”**

* If you want to search a project from **values not equal** to x: **“ !x ”**

You can also apply Operators:

* Operator1 **OR** Operator2:   **“ , ”**

* Operator1 **AND** Operator2:   **“ ; ”**

For example:

* **project:wethod, php ; start:0116+ ; prob:50…75 **

This search operator will find all the projects with name “wethod" or “php”, with a date start grater than January 2016 and a probability between 50% and 75%.

* **client:luca; value: 25- ; end:1217+**

This search operator will find all the projects of the client Luca, with value less or equal to 25 and with an end date in or after December 2017

* **pm:tomas, luca; prob:30…50; status:2 **

This search operator will find all the project whose PM is Tomas or Luca, with a probability between 30 and 50 and a budget status which is approved.

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