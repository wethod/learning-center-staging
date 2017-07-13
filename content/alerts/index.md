---
date: '2017-06-13T18:08:29+02:00'
title: Alerts
weight: 21

---
## Overview

This widget shows all the inconsistencies regarding the user. Each alert has a priority (indicated by its color):

* **Yellow alerts** have a low priority and can be seen more as advices.

* **Red alerts** have an high priority and must be solved as soon as possible;

Hovering on an alert will display a description of the problem.

## YELLOW Alerts

### Unsent Order

This alert is shown to the project manager who have created orders not sent yet.

*How to solve? Just send all the waiting orders.*

### Opportunity Due Date

This alert is shown to the project manager who have created an opportunity that's expiring in 3 days or that's already expired.

*How to solve?  You have to create a budget in order to transform the opportuniy in a project or simply change the timeline. *

### Project Probability / Invoice Plan

This alert is shown to the project manager of a project which has:

* **An [invoice plan]({{< relref "pipeline/index.md#invoice plan" >}}) manually set;**

* **A probability lower than 90%.**

*How to solve? The project can be considered active if its probability is higher or equal to 90%. *

### Budget Submitted

This alert is shown if you have the permission to approve budgets and there's a budget waiting for approval.

*How to solve? Approve the budget in question*

### Budget Consumption Too Fast

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% greater than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

{{< img-center src="/uploads/2017/07/13/too%20fast%20.png" >}}

It means that your Budget Consumption which is equal to the days of your project’s timesheet is higher then the Project Status.

For example if you have a Timesheet = 11/12, this means that you have 1 day left.

On the other hand with a Project Status = 8/12, according to your PM you will have other 4 days of work.

As a result you are in a very bad situation because you will have to do the work of 4 days imposted by the project status in only 1 day left indicated by the Timesheet.

In order to solve this problem you should control if effectively the data of the Timesheet and of the Project Status are right. If these data are right, the PM have to increase the days of work so as a consequence approve also a new Budget.

*How to solve? In order to solve this problem you should control if effectively the data of the Timesheet and of the Project Status are right. If these data are right, the PM have to increase the days of work so as a consequence approve also a new Budget.*

### Budget Consumption Too Slow

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% lower than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

It means that your Budget Consumption which is equal to the days of your project’s timesheet is lower then the Project Status.

For example if you have a Timesheet = 8/12, this means that you have 4 days left.

On the other hand with a Project Status = 11/12, according to your PM you will have only another day of work.

In this case you are in trouble, in fact according to your Timesheet the PM have planned an excessive Timesheet so the project is spending too much.

*How to solve? The solution to this yellow alert is to first of all check if the data of the project’s Timesheet and Project Status a re right, if they are, the PM have to delete days of work and increase your margin decreasing the budget.*

### Project Status / Archived

This alert is shown if you're manager of a finished project which isn't already been archived.

*How to solve?  It's a good practice to archive your projects when their project status reach 0. *

### Project Probability / Budget

This alert is shown if you're manager of a project with probability greater than 50% but with budget in draft or missing.

The aim of this alert is to show to the project manager, given the inconsistent probability.

*How to solve?  It is useful to do as much as possible in order to work with an approved budget.*

### Planning or Timesheet but Probability < 90%

This alert is shown if you're manager of a project with probability lower than 90% but which already have a planning and/or timesheets.

*How to solve? Remember that a project is considered active only if it has a probability greater or equal to 90%.
For a project that is not active yet, it is a no sense to plan resources or to register a timesheet. *

### Planning > Project Status

This alert is shown if you're manager of a project for which are planned (in the future) more days than the last project status days. What's the meaning of requiring more resources than what you really need?

*How to solve? The project manager have to require the right number of resources. *

Notice that:
**Future Planned Days**: the days that are planned for the project in the future
**Project Status Days**: the days left to the realization of the project

### Client PO

This alert is shown to the project manager if one of the following situations happens:

* **Project has probability of 100% or has some Invoices but there isn't a Purchase Order set for the project**

* **A Purchase Order is set for the project despite its probability is lower than 100%**

### Project Start

This alert is shown to the project manager if one of the following situations happens:

* **A project is started but its probability is lower than 90%**

* **A project is going to start during the current month but its probability is lower than 75%**

*How to solve? Ready to start your project?
A project is considered started if it has a start date in the past or if someone has submitted timesheets for it. *

### Project Status

If there is a project whose [timesheet]({{< relref "friday/index.md#timesheet" >}}) is settled but the project status not then there is this alert in order to remind the manager of a project who forgot to update the [project status]({{< relref "friday/index.md#project status" >}}) in the last two weeks.

*How to solve? On Friday a project manager have to settle the project status *

### Timesheet - Time Tracking Alert

This alert is shown to the employee of a project who forgot to submit the timesheet in the last two weeks.

*<How to solve? Do the timesheet as soon as possible!*

## RED Alerts

### Project Duration / Timesheet

This alert is shown to the manager of a project which has some timesheets done before the start date or after the end date.

*How to solve? Understand your teammates are doing timesheets for a non active project*

### Invoice Plan / Budget Final Net Price

This alert is shown to the manager of a project if the following situations happens:

* **The invoice plan is set as manual**

* **Invoice plan's total amount and final net price  mismatch**

*How to solve? This can happen when you edit budget after setting invoice plan as manual. As a result what a project manager have to do is to try to match invoice plan and final net price*

### Job Order / Project Probability

This alert is shown to the manager of a project if one of the following situations happens:

* **The probability si greater than 90% but the project has't a job order**

* **The probability si lower than 90% and the project has a job order**

*How to solve?
Remind that only active projects, which means projects with a probability greater or equal to 90% must have a [job order]({{< relref "glossary/index.md#job-order" >}})*

### Planning / Project End

This alert is shown to the manager of a project for which are planned people even after the project's end date.

*How to solve? The project is ended, you have no reason to plan people in it*

### Planning / Budget Status

This alert is shown to the manager of a project which has future planned resources but hasn't an approved [budget]({{< relref "budget/index.md#budget" >}})

The planned resources show that the project is active but the budget is not approved, so the alert remind you to approve it as soon as possible.

*How to solve? You cannot plan resources if you haven't a budget which gives you the right to do it, as a consequence you should increase your budget*

### Non Chargeable / Budget Final Net Price

This alert is shown to the manager of a non chargeable project which has a final net price greater than zero. This is a paradox because non chargeable project can't have revenues by definition.

*How to solve? If there is a non chargeable project, you do not have to fix a final net price.*

### Empty Planning

This alert is shown to you if you're not planned for tomorrow (Saturday and Sunday excluded).

*How to solve? What are you waiting for? Go [planning]({{< relref "planning/index.md#planning" >}})!*

### Orders / External Cost

This alert shows to the manager of a project where the sum of orders, travels and expenses go over the [budget external cost]({{< relref "budget/index.md#budget external cost" >}})

*How to solve? You don't want to spend money you don't have, do you? You do not have to go over the budget!*