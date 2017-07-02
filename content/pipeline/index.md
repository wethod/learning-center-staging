---
date: '2016-03-11T20:10:46+01:00'
title: Pipeline
weight: 30

---


{{< img-center src="/uploads/2017/05/25/nav-pipeline.png" >}}

## Overview

Everything starts from Pipeline, here is where opportunities and projects are listed, both of them are defined by a small amount of significant information:

* Name;

* Client;

* Value (in €k);

* Percentage of external costs;

* Category;

* Probability.

Pipeline has three subsections: Basket, Projects and Programs.

## Basket

<div><p>The Basket contains all the project’s opportunity that are not well-defined yet. You can see it as a place where to put all the ideas that you usually write on a notebook or on a Post-It.</p><p>The significant information listed above are <i>not mandatory</i> for an opportunity.</p><p><b>Opportunities usually have a probability between 1% and 99%.</b></p></div>

## Projects

<div><p>Here you can find all the projects of the company, each project has significant information you can check and edit. Clicking on a project let you see more details and actions about it.</p><p>An opportunity evolves into a Project when things get serious, in order to take this step you must have an idea about the significant information listed above.</p><p>A Project can furthermore have an invoice plan and a budget.</p><p>A project is considered <b>started</b> if it has a start date in the past or if someone has submitted timesheets for it.<br></p>
	<p>
		A project is considered <b>active</b> when its probability reaches 90%, only when this happens makes sense to plan people or to do timeheets for this project. An active project must have a job order.</p>
        {{&lt; note title="Note" &gt;}}
**<p>Billable Projects must have a probability of 100%.</p>**
**<p>When a project status reach 0, it's a good practice to archive it.</p>**
**<p>When a project reach 50% of probability, it's a good practice to make a budget for it.</p>**
{{&lt; /note &gt;}}
<p>{{&lt; img-center src="/uploads/2017/05/25/projects.png" &gt;}}</p>
<p>By clicking on a project you can edit its details or open its: <em>budget</em>, <em>planning</em>, <em>report</em>, <em>invoice plan</em>.</p>
<h3>Invoice Plan</h3>
<p>Here you can set when you plan to emit invoices for the project. This section is basically a calendar with some additional information:</p>
<ul>
<li>
<p><strong>Plan</strong>: the amount you plan to invoice for a given month;</p>
</li>
<li>
<p><strong>Invoiced</strong>: the amount actually invoiced for a given month. This is automatically updated each time you create an invoice for the project;</p>
</li>
<li>
<p><strong>Delta</strong>: the difference between Plan and Invoiced for a given month.</p>
</li>
</ul>
<p>An invoice plan can be:</p>
<ul>
<li>
<p><strong>Automatic</strong>: an invoice is automatically planned for each project's duration month, the invoice amount is obtained by dividing project's estimate by project's duration;</p>
</li>
<li>
<p><strong>Manual</strong>: you need to manually insert each amount you plan to invoice. If you choose this mode, you can choose an <strong>offset</strong>&nbsp;amount to move back or forward in time.</p>
</li>
</ul>
<p>You can find the invoices (listed in your plan) in the [Invoices widget]({{&lt; relref "dashboard/index.md#invoices" &gt;}}), there they're ready to be created and sent.</p>
</div>

## Programs

Projects are often stages or parts of something bigger, you can use a Program to group together different projects in order to see their aggregate [economic reports]({{< relref "reports/index.md#economics" >}}).