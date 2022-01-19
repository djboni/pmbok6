# Baselines

## Contents

- [Scope baseline](#scope-baseline)
- [Schedule baseline](#schedule-baseline)
- [Cost baseline](#cost-baseline)

## Scope baseline

"The approved version of a scope statement, work breakdown structure (WBS), and
its associated WBS dictionary, which is used as a basis for comparison."
[[1]](../home.md#references)

- Project scope statement
- WBS
- Work package
- Planning package
- WBS dictionary

### Work breakdown structure (WBS)

```ascii
            +-----+
            | 1.0 |
            +-----+
               |
   +-------+---+---+-------+
   |       |       |       |
+-----+ +-----+ +-----+ +-----+
| 1.1 | | 1.2 | | 1.3 | | 1.4 |
+-----+ +-----+ +-----+ +-----+
```

```mermaid
graph TD;
    %% Mermaid graph
    %% Works on GitLab, not on GitHub
    A1[1.0]
    A1---B1[1.1];
    A1---B2[1.2];
    A1---B3[1.3];
    A1---B4[1.4];
```

## Schedule baseline

"The approved version of the schedule model that is used as a basis for
comparison to the actual results." [[1]](../home.md#references)

- Documentation of the basis of the estimate
- Documentation of all assumptions made
- Documentation of any known constraints
- Indication of the range of possible estimates
- Indication of the confidence level of the final estimate
- Documentation of individual project risks influencing this estimate

```ascii
Section 1 | Task A    |
                      | Task B      |

Section 2   | Task C  |
                      | Task D                |
```

```mermaid
gantt
    %% Mermaid graph
    %% Works on GitLab, not on GitHub
    title Schedule diagram
    dateFormat YYYY-MM-DD
    excludes weekends
    section Section 1
        Task A : a1, 2022-01-24, 12d
        Task B : after a1, 14d
    section Section 2
        Task C : 2022-01-26, 10d
        Task D : 24d
```

## Cost baseline

"The approved version of the time-phased project budget that is used as a basis
for comparison to the actual results." [[1]](../home.md#references)
