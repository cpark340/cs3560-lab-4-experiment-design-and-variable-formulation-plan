## 2. Hypothesis Formulation

| ID   | Alternative hypothesis (H1)                                                                                 | Null hypothesis (H0)                                                                                                 |
|------|-------------------------------------------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------|
| H1-A | Participants using the Treatment will complete the elective task in less time than when using the Baseline. | There is no statistically significant difference in Task_Completion_Time_sec between the Treatment and the Baseline. |
| H1-B | Participants using the Treatment will make fewer errors than when using the Baseline.                       | There is no statistically significant difference in Error_Count_Total between the Treatment and the Baseline.        |
| H1-C | Participants will give the Treatment a higher Single Ease Question rating than the Baseline.                | There is no statistically significant difference in SEQ_Rating between the Treatment and the Baseline.               |
| H1-D | Participants will give the Treatment a higher System Usability Scale score than the Baseline.               | There is no statistically significant difference in SUS_Score between the Treatment and the Baseline.                |

The significance level is alpha = 0.05, one-tailed, because the
direction of each prediction comes from the Phase 1 findings.

## 3. Variable Formulation & Operationalization

### 3.1 Independent Variable

| Variable                  | Levels                                                               | Type                               | Assignment                                                                  |
|---------------------------|----------------------------------------------------------------------|------------------------------------|-----------------------------------------------------------------------------|
| Interface                 | Baseline (current modal replica) vs. Treatment (Find Electives page) | Within-subjects, manipulated       | Every participant uses both; order is counterbalanced (Section 4.2)         |
| Task_Version (controlled) | T1: Tuesday/Thursday; T2: Monday/Wednesday                           | Controlled, crossed with Interface | Counterbalanced so each interface is paired with each version equally often |

### 3.2 Dependent Variables

| Variable                              | Operational definition                                                                                                                                                                                                                                     | Scale / unit                        | How measured                                   |
|---------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|-------------------------------------|------------------------------------------------|
| Task_Completion_Time_sec (efficiency) | Seconds from the researcher saying "begin" (start screen displayed) until the participant says "done" and names two courses. Capped at 300 s.                                                                                                              | Seconds (ratio)                     | Stopwatch checked against the screen recording |
| Error_Count_Total (effectiveness)     | Number of the two chosen courses that break a task rule (0 to 2). A course is an error if no section of it meets all three rules: offered in Fall 2026, at least 1 open seat, and meets on the task's days (online and Friday-only sections do not match). | Count, 0 to 2                       | Scored against the answer key                  |
| Task_Success_Binary (effectiveness)   | 1 if exactly two different courses were named and Error_Count_Total = 0; otherwise 0. A timeout counts as 0.                                                                                                                                               | 0 or 1                              | Scored against the answer key                  |
| SEQ_Rating (satisfaction)             | Asked right after each task: "Overall, how easy or difficult was this task?"                                                                                                                                                                               | 1 (very difficult) to 7 (very easy) | Verbal response, recorded on the sheet         |
| SUS_Score (satisfaction)              | 10-item System Usability Scale after each interface. Odd items: response minus 1. Even items: 5 minus response. Sum of items times 2.5.                                                                                                                    | 0 to 100                            | Paper or form questionnaire                    |

Recorded but not tested: Prior_CatTracks_Familiarity (1 to 5, from
screening), Screenshot_Taken (0 or 1, an observed workaround),
Task_Timed_Out (0 or 1), the two selected courses, and observer notes.

### 3.3 Confounding Variables & Controls

| Confound                                | Why it matters                                                             | Control                                                                                                                                                              |
|-----------------------------------------|----------------------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Prior system familiarity                | Experienced students may find the modal easier than newcomers do.          | Screening question recorded as a covariate. Within-subjects design means each person is compared with themselves.                                                    |
| Learning and practice effects           | The second task may feel easier because of practice.                       | Counterbalanced order (Section 4.2) and two different task versions.                                                                                                 |
| Carryover (knowing the course list)     | Both conditions use the same 14 courses.                                   | Task versions have different correct answers. Carryover is checked in the analysis (Section 4.5).                                                                    |
| Task difficulty differences             | T1 might be harder than T2.                                                | Both tasks have 4 valid courses and the same kinds of distractors (full section, not offered in Fall, online, wrong days). Task versions are crossed with interface. |
| Fatigue                                 | Later performance may slow down.                                           | Session of 25 minutes or less, a 2-minute break between conditions, counterbalanced order.                                                                           |
| Input hardware and display              | A different mouse, trackpad or screen changes time.                        | All sessions use the same laptop, browser, fixed screen resolution and an external mouse.                                                                            |
| Ambient environment                     | Glare, noise and interruptions affect performance.                         | Same quiet room, fixed screen brightness, phones silenced.                                                                                                           |
| Researcher effects                      | I built the Treatment and could hint without meaning to.                   | Written scripts, no hints during tasks, scoring rules fixed before sessions.                                                                                         |
| Participant expectations                | People may favor what looks newer.                                         | The interfaces are called Version A and Version B. Which is the redesign is revealed only at debrief.                                                                |
| Prior exposure to the redesign          | People from the Phase 1 or Phase 2 studies have seen the design direction. | Exclude them (Section 4.3).                                                                                                                                          |
| Browser zoom and accessibility settings | Settings change layout and reading speed.                                  | Default 100% zoom. If a participant needs a change, allow it and note it.                                                                                            |
