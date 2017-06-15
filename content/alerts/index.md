---
date: '2017-06-13T18:08:29+02:00'
title: Alerts
weight: 21

---


## Overview

This widget shows all the inconsistencies regarding the user. Each alert has a priority (indicated by its color):

* Red alerts have an high priority and must be solved as soon as possible;

* Yellow alerts have a low priority and can be seen more as advices.

Hovering on an alert will display a description of the problem.

## Description

### Unsent Order

This alert is shown to the project manager who have created orders not sent yet.

### Opportunity Due Date

This alert is shown to the project manager who have created an opportunity that's expiring in 3 days or that's already expired.

### Project Probability / Invoice Plan

This alert is shown to the project manager of a project which has:

* An invoice plan manually set;

* A probability lower than 90%.

### Budget Submitted

This alert is shown if you have the permission to approve budgets and there's a budget waiting for approval.

### Budget Consumption Too Fast

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% greater than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

### Budget Consumption Too Slow

This alert is shown if you're manager of a project where the [budget consumption]({{< relref "reports/index.md#budget-consumption" >}}) is more than 20% lower than the project's [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}).

### Project Status / Archived

This alert is shown if you're manager of a finished project which isn't already been archived.

It's a good practice to archive your projects when their project status reach 0.

### Project Probability / Budget

This alert is shown if you're manager of a project with probability greater than 50% but with budget in draft or missing.<span style="font-size: 1rem;">&nbsp;</span>

### Planning or Timesheet but Probability < 90%

This alert is shown if you're manager of a project with probability lower than 90% but which already have a planning and/or timesheets.

### Planning > Project Status

This alert is shown if you're manager of a project for which are planned (in the future) more days than the last project status days. What's the meaning of requiring more resources than what you really need?

### Client PO / Project Probablity

This alert is shown to the project manager if one of the following situations happens:

* Project has probability of 100% but there isn't a Purchase Order set for the project;

* A Purchase Order is set for the project despite its probability is lower than 100%.

A Purchase Order is needed to emit invoices, so it's strange that a 100% probability project hasn't a Purchase Order or vice versa.

### Project Start

This alert is shown to the project manager who have created orders not sent yet.

### Project Status

This alert is shown to the project manager who have created orders not sent yet.

### Timesheet

This alert is shown to the project manager who have created orders not sent yet.