---
date: '2017-05-24T12:01:45+02:00'
title: Reports
weight: 60

---
## Overview

All the data you insert in WETHOD are used to generate, weekly and automatically, a set of reports useful to monitoring the projects' progress.

## Project Report

Each Monday, utilising data provided by [Timesheet]({{< relref "friday/index.md#timesheet" >}}), [Project Status]({{< relref "friday/index.md#project-status" >}}) and [Budget]({{< relref "budget/index.md" >}}), a Project Report is automatically created.

### Budget Consumption / Project Status

This section shows the [budget consumption]({{< relref "glossary/index.md#budget-consumption" >}}) of the project, compared to its [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}):

* If the project is **above the diagonal**: it's using a lot of days but it's progressing slowly than predictions based on budget;

* If the project is **under the diagonal**: it's using few days but it's progressing faster than predictions based on budget;

* If the project is **on the diagonal**: it’s planned and managed correctly.

By analizing the saved budget versions for the project, WETHOD can shows you:

* The **baseline** which answers the question "*what would the situation be if I hadn't changed the budget since its first version*?";

* The **forecast** which answers the question *"what's the situation right now?"*;

* The **projected** which answers the question "*what will be the situation at the end of the project with the current budget consumption?"*;

* The **wasted** which answers the question "*what's the situation right now, [wasted hours]({{< relref "glossary/index.md#wasted-hours" >}}) included?"*;

The grey dots shows you the forecast of the various past budget versions.

On the right of the graph you have:

1. **Baseline**: the first budget's hours amount;

1. The variations of the budget's hours amount since the baseline was approved;

1. [**Contingency**]({{< relref "budget/index.md#the-price-s-detail" >}});

1. **Forecast**: the current budget's hours amount (Baseline + variations + contingency);

1. A resume of the worked, planned, wasted and still available hours.

{{< img-center src="/uploads/2017/07/07/budg.con:Proj.status.png" >}}

### Invoices & Orders

Here are listed all the [orders]({{< relref "finance/index.md#orders" >}}) and [invoices]({{< relref "finance/index.md#invoices" >}}) linked to the project, clicking on one of them will take you to the related details.

### Economics

Here is shown the trend of various [budget's]({{< relref "budget/index.md" >}}) voices for the project:

* **Revenues**: the project's final net price;

* **Internal Cost**;

* **External Cost**: the sum of all external costs, travels and expenses excluded;

* **Travels**;

* **Expenses**;

* **Gross Margin**: the difference between final net price and costs (either internal and external);

* **Wasted**: the wasted money, which is the sum of the wasted hours multiplied by the cost of their [levels]({{< relref "settings/index.md#company" >}});

* **Net Margin**: the difference between gross margin and wasted.

For each indicator you can see its value for:

* The **baseline**: first approved budget's version & current progress;

* The **forecasts**: last approved budget's version (a.k.a. current version) & current progress;

* The **projected**: last approved budget's version & progress at 100%;

* The **delta vs baseline**: difference between projected and baseline;

* The **delta vs forecast**: difference between projected and forecast.

The grey percentage under *margin* refers to the *revenues*.

{{< img-center src="/uploads/2017/06/12/report-economics.png" >}}

### Timesheet / Project Status

This is the only place in WETHOD where you can see the weekly details of a given project. Here you can quickly appreciate the relation between **worked hours**, **days left**(taken from the project status) and** **<span style="font-size: 1rem;">[</span><span style="font-size: 1rem;"><b>roadrunner index</b></span><span style="font-size: 1rem;">]({{&lt; relref "glossary/index.md</span><span style="font-size: 1rem;">#roadrunner-index-rri</span><span style="font-size: 1rem;">" &gt;}}).</span>

When worked hours grows, days left must decrease. If this doesn't happen, you have a problem: your teammates are working on something which doesn't move forward.

### Hour / User

Here are reported, for each teammate who have worked to the project, the comparison between his/her worked hours and his/her planned hours.

## Budget Consumption

This is an overview of all Projects in terms of resources and time spent on the project, allowing you to analyse their health at a glance.

For each pipeline's project, its [budget consumption]({{< relref "glossary/index.md#budget-consumption" >}}) is compared to its [progress]({{< relref "glossary/index.md#absolute-project-progress" >}}):

* If the project is **above the diagonal**: it's using a lot of days but it's progressing slowly than predictions based on budget;

* If the project is **under the diagonal**: it's using few days but it's progressing faster than predictions based on budget;

* If the project is **on the diagonal**: it's planned and managed correctly.

Using filters, you can select the Projects you want to see and explore details such as billed hours, invoiced totals, and internal and external purchase orders.

{{< img-center src="/uploads/2017/05/25/bubbles_tour_01.jpg" >}}

## Revenue Progress

This report compares the projects' status with the percentage of their value which is already been invoiced.

How to read the project's position on the graph:

* If the project is **above the diagonal**: more work days than the actually done have been invoiced;

* If the project is **under the diagonal**: not al work days done for the project have been invoiced;

* If the project is **on the diagonal**: project status and invoiced percentage are consistent, this means that until now all the work days done has been invoiced.

{{< img-center src="/uploads/2017/07/06/Revenue%20Progress.png" >}}

## Revenue Pipeline

This report is composed by three sections which aggregate the [revenue pipeline]({{< relref "glossary/index.md#revenue-pipeline" >}}) **by probability**, **by client** or **by project type**.

Each section shows a column diagram, where each column refers to a particular year (previous, current, next) and its generated by the projects which invoice plan hits that year. Clicking on a column will show a right panel with further information linked to the column itself.

### By Probability

Each column is divided into subcolumns which group projects with different probability.

Clicking on a subcolumn will show a panel listing all the grouped projects with their:

* Name;

* Client's name;

* Value;

* Probability;

* [Expected value]({{< relref "glossary/index.md#expected-value" >}}).

{{< img-center src="/uploads/2017/07/06/REV.progress%20by%20probability.png">}}

### By Client

Clicking on a column will show a panel listing all the grouped projects with their:

* Client's name;

* Value;

* Percentage of influence on the [revenue pipeline]({{< relref "glossary/index.md#revenue-pipeline" >}}).

{{< img-center src="/uploads/2017/07/06/REV.prog%20by%20client.png">}}

### By Project Type

Clicking on a column will show a panel listing all the grouped projects with their:

* Client's name;

* Value;

* Percentage of influence on the [revenue pipeline]({{< relref "glossary/index.md#revenue-pipeline" >}}).

{{< img-center src="/uploads/2017/07/06/REv.prog%20by%20project%20type.png">}}

## Revenue Actuals

<div><p>This report is composed by two sections which aggregate the already made invoices by month or by client.</p><p>Each section shows a column diagram, where each column refers to a particular year (previous, current, next) and its generated by the invoices made that year. Clicking on a column will show a right panel with further information linked to the column itself.
</p><p>{{&lt; img-center src="/uploads/2017/07/06/Rev%20Actuals.png"&gt;}}</p>
<h3>By Month</h3>
<p>Clicking on a column will show a panel listing all the months for which an invoice exists with their:</p>
<ul>
<li>
<p>Name;</p>
</li>
<li>
<p>Invoices' value sum for that month;</p>
</li>
<li>
<p>Percentage of influence on the annual invoice amount.</p>
</li>
</ul>
<h3>By Client</h3>
<p>Clicking on a column will show a panel listing all the clients for which an invoice exists with their:</p>
<ul>
<li>
<p>Name;</p>
</li>
<li>
<p>Invoices' value sum for that client;</p>
</li>
<li>
<p>Percentage of influence on the annual invoice amount.</p>
</li>
</ul>
<h2>Production Value</h2>
<p>This is an overview of the annual projects' [production value]({{&lt; relref "glossary/index.md#production-value" &gt;}}). By clicking on a specific month you can access that month's production value grouped <strong>by client</strong>,&nbsp;<strong>by project</strong>&nbsp;or <strong>by week</strong>.</p>
<p>{{&lt; img-center src="/uploads/2017/06/12/production-value.png" &gt;}}</p>
<h3>By Week</h3>
<p>In this view you can see, for each project (and for the selected week):</p>
<ul>
<li>
<p>The [roadrunner index]({{&lt; relref "glossary/index.md#roadrunner-index-rri" &gt;}});</p>
</li>
<li>
<p>The <strong>lost production</strong>: let's say people worked on a project for&nbsp;<em>A</em> hours and the project progressed of&nbsp;<em>B</em> hours. If <em>A</em> is greater than <em>B</em> &nbsp;you've used more hours than expected and this value gives you how much production you've lost;</p>
</li>
<li>
<p>The <strong>production value</strong>;</p>
</li>
<li>
<p>The <strong>worked days</strong>: how many days people have worked on the project during the selected week;</p>
</li>
<li>
<p>The <strong>progress</strong>: how many days the project has progressed during the selected week, that is the difference between the selected week project status and the previous one;</p>
</li>
<li>
<p>The <strong>1D Value</strong>&nbsp;<strong>(Budget)</strong>: estimated daily production value, that is "what's the expected value that must be produced for the project by day?". This is calculated by dividing the project's estimate by the project's budget days;</p>
</li>
<li>
<p>The <strong>1D Value (Actual)</strong>: actual daily production value, that is "what's the value produced for the project by day?". This is calculated by dividing the project's production value by the project's worked days. This value is green if it's greater than <em>1D Value (Budget)</em>, red otherwise;</p>
</li>
<li>
<p>The <strong>external cost</strong>: project's external cost percentage on the total estimate.</p>
</li>
</ul>
<p>You can switch between month's week by using the selector placed at the top of this section.</p>
<h2>Timesheets</h2>
<p>This is a weekly overview of the [timesheets]({{&lt; relref "friday/index.md#timesheet" &gt;}}) made by your teammates, each timesheet is coloured as the&nbsp;[job order category]({{&lt; relref "settings/index.md#company" &gt;}}) of the project it's linked to and you can see the project's name by clicking on its timesheet.</p>
<p>On the top left corner you can filter the displayed people.</p>
<p>On the top right corner you can change the week of the displayed timesheets.</p>
<p>{{&lt; img-center src="/uploads/2017/07/06/Timesheets.png"&gt;}}</p>
<h2>Timesheet Roadrunner</h2>
<p>This report shows all the timesheets for the selected year, grouped by Job Order Category and compared&nbsp;to the&nbsp;<a href="http://support.wethod.com/glossary/index/#roadrunner-index-rri">Roadrunner Index</a>.</p>
<p>You can chose between monthly and weekly visualization via the selector on the top of the section, where you can also find the year selector.</p>
<p>{{&lt; img-center src="/uploads/2017/07/06/RRI.png"&gt;}}</p>
<h2>Changelog</h2>
<p>Here are listed all the changes done on value or probability of pipeline's projects.</p>
<p>For each change you can see:</p>
<ul>
<li>
<p>The name of the project which has been changed;</p>
</li>
<li>
<p>The name of the change's author;</p>
</li>
<li>
<p>The change's date;</p>
</li>
<li>
<p>The old value and the updated value;</p>
</li>
<li>
<p>The old probability and the updated probability;</p>
</li>
<li>
<p>The difference between the updated and the old <a href="glossary/index.md#expected-value">expected value</a>.</p>
</li>
</ul>
</div>