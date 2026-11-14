## 4. Experimental Design Architecture & Counterbalancing

## 4.1 Subject Design: Within-Subjects

- With 8 participants, a between-subjects design would leave only 4 per
  condition, below the N of 5 required. Within-subjects gives 8
  observations per condition.
- Students vary a lot in speed and CatTracks experience. Each person
  acts as their own control, which removes much of that variation.
- The cost is learning and carryover effects, handled by
  counterbalancing and by using two parallel tasks.

## 4.2 Counterbalancing

Two interface orders crossed with two task orders give four sequences (a
Latin square). Participants are assigned in rotation: P01 to S1, P02 to
S2, P03 to S3, P04 to S4, then P05 to S1, and so on.

| Sequence | Participants | First session              | Second session             |
|----------|--------------|----------------------------|----------------------------|
| S1       | P01, P05     | Baseline with Task 1 (T1)  | Treatment with Task 2 (T2) |
| S2       | P02, P06     | Baseline with Task 2 (T2)  | Treatment with Task 1 (T1) |
| S3       | P03, P07     | Treatment with Task 1 (T1) | Baseline with Task 2 (T2)  |
| S4       | P04, P08     | Treatment with Task 2 (T2) | Baseline with Task 1 (T1)  |

Each interface appears first and second 4 times each, and each task
version is paired with each interface 4 times, so order and task
difficulty are balanced across conditions.

## 4.3 Participant Sampling Plan

- **Persona:** A WSU undergraduate in Computer Science (junior or
  senior) who has to pick CS electives and has used CatTracks.
- **Inclusion:** 18 or older, currently enrolled at WSU, CS major or
  minor, has opened a CatTracks degree evaluation at least once, can use
  a mouse and keyboard (with or without assistive settings).
- **Exclusion:** Anyone who took part in the Phase 1 interviews or the
  Phase 2 card sort, or who has seen the redesign; non-WSU students.
- **Sample size:** N = 8 (2 per sequence), giving 8 observations per
  condition, which meets N of 5 or more per condition. This is limited
  by class resources, so the study can only detect large effects and is
  treated as an early test.
- **Recruitment:** In-person invitation or class and club channels.
  Participation is voluntary.
- **Accessibility:** Participants may use browser zoom or their
  preferred input device. Any change is noted and analyzed separately.
  Testing with screen reader users is recommended as follow-up work.

## 4.4 Session Procedure (about 25 minutes)

| Step | Time  | What happens                                                                              |
|------|-------|-------------------------------------------------------------------------------------------|
| 1    | 3 min | Read the briefing script and get verbal consent.                                          |
| 2    | 1 min | Screening question: familiarity with CatTracks (1 to 5). Assign the next sequence.        |
| 3    | 6 min | First condition: read the task, press start, timed task, SEQ question, SUS questionnaire. |
| 4    | 2 min | Break. Reset the browser.                                                                 |
| 5    | 6 min | Second condition: same steps with the other interface and task version.                   |
| 6    | 3 min | Short debrief and thanks.                                                                 |

Participants are not asked to think aloud during timed tasks, because
that would slow them down. If a participant reaches 300 seconds, stop
the task and record Task_Timed_Out = 1.

## 4.5 Analysis Plan

- Each participant gives one pair of values per measure. The unit of
  analysis is the difference (Treatment minus Baseline).
- Test time, errors, SEQ and SUS with a Wilcoxon signed-rank test
  (one-sided, alpha = 0.05). With 8 pairs, the smallest possible
  one-sided p-value is 1/256 (about 0.004), so significance needs nearly
  every participant to move in the predicted direction.
- Report Task_Success_Binary as counts per condition (descriptive only).
- Report the median paired difference, percent change and the
  rank-biserial correlation for every measure, with each participant's
  pair shown in a plot.
- Practical thresholds, set before data collection (proposed): 20% or
  more reduction in median time, at least 1 fewer error, at least 1
  point higher SEQ, at least 10 points higher SUS.
- Order check: compare the differences of the 4 Baseline-first and 4
  Treatment-first participants, and repeat the comparison using
  first-session data only (Section 6, question 2).
- Treat the four tests as exploratory and report exact p-values.

## 5. Ethical Protocol Safeguards

## 5.1 Briefing and Consent Script

"Thank you for helping with my class project. Today I am comparing two
versions of a course lookup page for CS electives. I am testing the
software, not you. There are no right or wrong ways to use it, and if
something is hard to find or confusing, that tells me the design needs
work, not that you did something wrong.

You will do one short task on each version, and after each task I will
ask a few quick questions about how it felt. The session takes about 25
minutes. I will time each task and record the screen. I will not record
your face, and I will only write down a participant number, not your
name. The course data in both versions is made up for this study.

Taking part is voluntary. You can skip any question, take a break, or
stop at any time without giving a reason, and it will not affect your
grades or anything else. While you work I can't help with the task,
because I want to see how the page works on its own. If you get stuck,
do what you would normally do. Please tell me when you are done and name
the two courses you picked.

Do you have any questions? Are you willing to take part?"

Record the answer as Consent_Verbal = Y or N on the data sheet. If N,
thank the person and end the session.

## 5.2 Task Instructions

| Task        | Instruction read to the participant                                                                                                                                             |
|-------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Task 1 (T1) | "You need two upper-division CS electives for Fall 2026. Find two that have open seats and meet on Tuesdays and Thursdays. Tell me when you are done and name the two courses." |
| Task 2 (T2) | "You need two upper-division CS electives for Fall 2026. Find two that have open seats and meet on Mondays and Wednesdays. Tell me when you are done and name the two courses." |

Standard reply if asked for help: "I can't help with that part. Do what
you would normally do."

## 5.3 Data Handling

- Participants are identified only as P01 to P08. No names are stored
  with the data.
- Screen recordings stay on the researcher's device and are deleted
  after times and errors are scored.
- Results are reported in aggregate or by participant number.

## 5.4 Debrief Script

"Thank you. Both versions used made-up course data. One was a copy of
how CatTracks works now, and the other was a design idea I am testing.
Your results will only be reported with a participant number. Do you
have any questions? I can share the findings when I finish."
