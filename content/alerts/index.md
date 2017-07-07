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

{{< note title="Note" >}}
To solve the problem the pm have to send the orders
{{< /note >}}

### Opportunity Due Date

This alert is shown to the project manager who have created an opportunity that's expiring in 3 days or that's already expired.

{{< note title="Note" >}}
You have to create a budget in order to transform the opportuniy in a project or simply change the timeline.
{{< /note >}}

### Project Probability / Invoice Plan

This alert is shown to the project manager of a project which has:

* An [invoice plan]({{< relref "pipeline/index.md#invoice plan" >}}) manually set;

* A probability lower than 90%.

{{< note title="Note" >}}
Solution: the project can be considered active if its probability is higher or equal to 90%.
{{< /note >}}

### Budget Submitted

This alert is shown if you have the permission to approve budgets and **there's a budget waiting for approval**.

* Project id, project id budget, project status

* Budget id, budget status

* Employee id, employee id person, employee type

* Roles

### Budget Consumption Too Fast

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% greater than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

The problem depends on:

* Project probability

* The last project status added

* Sum of the timetracking hours on the project

* Margin

**Increase your project's progress until it's greater then Budget Consumption**

### Budget Consumption Too Slow

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% lower than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

### Project Status / Archived

This alert is shown if you're manager of a finished project which isn't already been archived.

{{< note title="Note" >}}
It's a good practice to archive your projects when their project status reach 0.
{{< /note >}}

### Project Probability / Budget

This alert is shown if you're manager of a project with probability greater than 50% but with budget in draft or missing.<span style="font-size: 1rem;">&nbsp;</span>

The aim of this alert is to show to the project manager, given the inconsistent probability, maybe **it should be useful to do as much as possible in order to work with an approved budget**.

### Planning or Timesheet but Probability < 90%

This alert is shown if you're manager of a project with probability lower than 90% but which already have a planning and/or timesheets.

{{< note title="Note" >}}
**Remember**: a project is considered active only if it has a probability greater or equal to 90%.
For a project that is not active yet, it is a no sense to plan resources or to register a timesheet.
{{< /note >}}

### Planning > Project Status

This alert is shown if you're manager of a project for which are planned (in the future) more days than the last project status days. What's the meaning of requiring more resources than what you really need?
**The project manager have to require the right number of resources.**

Notice that:
**Future Planned Days**: the days that are planned for the project in the future
**Project Status Days**: the days left to the realization of the project

### Client PO

This alert is shown to the project manager if one of the following situations happens:

* Project has probability of 100% or has some Invoices but there isn't a Purchase Order set for the project

* A Purchase Order is set for the project despite its probability is lower than 100%

{{< note title="Note" >}}
A **Purchase Order** is needed to emit invoices, so it's strange that a 100% probability project hasn't a Purchase Order or vice versa.
As a result if you have a project with a probability of 100%, then organize your Purchase Order
{{< /note >}}

### Project Start

This alert is shown to the project manager if one of the following situations happens:

* **A project is started but its probability is lower than 90%**

* **A project is going to start during the current month but its probability is lower than 75%**

{{< note title="Note" >}}
**Ready to start your project?**
A project is considered started if it has a start date in the past or if someone has submitted timesheets for it.
{{< /note >}}

### Project Status

If there is a project whose [timesheet]({{< relref "friday/index.md#timesheet" >}}) is settled but the project status not then there is this alert in order to remind the manager of a project who forgot to update the [project status]({{< relref "friday/index.md#project status" >}}) in the last two weeks.

**On Friday a project manager have to settle the project status**

### Timesheet - Time Tracking Alert

This alert is shown to the employee of a project who forgot to submit the timesheet in the last two weeks.

**A solution? Do the timesheet as soon as possible!**

## RED Alerts

### Project Duration / Timesheet

This alert is shown to the manager of a project which has some timesheets done before the start date or after the end date.

**Why are your teammates doing timesheets for a non active project?**

### Invoice Plan / Budget Final Net Price

This alert is shown to the manager of a project if the following situations happens:

* **The invoice plan is set as manual**

* **Invoice plan's total amount and final net price  mismatch**

{{< note title="Note" >}}
This can happen when you edit budget after setting invoice plan as manual.
{{< /note >}}

### Job Order / Project Probability

This alert is shown to the manager of a project if one of the following situations happens:

* **The probability si greater than 90% but the project has't a job order**

* **The probability si lower than 90% and the project has a job order**

{{< note title="Note" >}}
Remind that only active projects, which means projects with a probability greater or equal to 90% must have a [job order]({{< relref "glossary/index.md#job-order" >}}).
{{< /note >}}

### Planning / Project End

This alert is shown to the manager of a project for which are planned people even after the project's end date.

### Planning / Budget Status

This alert is shown to the manager of a project which has future planned resources but hasn't an approved [budget]({{< relref "budget/index.md#budget" >}})

The planned resources show that the project is active but the budget is not approved, so the alert remind you to approve it as soon as possible.
You cannot plan resources if you haven't a budget which gives you the right to do it, as a consequence **you should increase your budget.**

### Non Chargeable / Budget Final Net Price

This alert is shown to the manager of a non chargeable project which has a final net price greater than zero. This is a paradox because non chargeable project can't have revenues by definition.

{{< note title="Note" >}}
It depends on:

* project type and project budget

* chargeable project

* budget/final net price

### Empty Planning

This alert is shown to you if you're not planned for tomorrow (Saturday and Sunday excluded).

**What are you waiting for? Go [planning]({{< relref "planning/index.md#planning" >}})!**

### Orders / External Cost

This alert shows to the manager of a project where the sum of orders, travels and expenses go over the [budget external cost]({{< relref "budget/index.md#budget external cost" >}})

**You don't want to spend money you don't have, do you?**