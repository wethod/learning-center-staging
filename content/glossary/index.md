---
date: '2017-05-22T17:31:29+02:00'
title: Glossary
weight: 200
last: true

---
### Budget Consumption

This value indicates, for a project, the percentage of the budget days already used. This is calculated by comparing timesheet hours and budget days.

### Pipeline Value

This value indicates the total estimated value of the pipeline's projects, weighted on their probability.

### Production Value

This value indicates *how much a project has produced *at a specific moment in time. This is calculated by multiplying the project's value for the project's percentage of completion (obtained from the Project Status).For example, a project with:

* Budget days: _100_;

* Last project status: _40_;

* Project's value: _10 K_;

Has a production value of: _10 K * ( ( 100 - 40 ) / 100 )_.

### Roardunner Index (RRI)

This value indicates, for a given week, the ratio between [project status]({{< relref "friday/index.md#project-status" >}}) and [timesheet]({{< relref "friday/index.md#timesheet" >}}):

* If ratio is _greater than 1_: last week an hour of work led to a project's progress greater than one hour. This means that project advanced faster than expected;
* If ratio is _equal to 1_: last week project's progress (based on Project Status) was consistent with the worked hours (based on Timesheet);
* If ratio is _lower than 1_: last week an hour of work led to a project's progress lower than one hour. This means that project advanced slower than expected.&nbsp;

_The perfect managed project has a constant RRI of 1_.