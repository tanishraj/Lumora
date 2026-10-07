# Statistics Notebook — Our Complete Growing School Story

> **Purpose:** Preserve the definitions, examples, analogies, formulas, and “why did we need this?” teaching pattern from our Statistics discussions, organised into the order in which the ideas are best studied.
>
> **Running story:** A school wants to understand student performance. We begin with raw observations, organise categories, summarise marks, describe spread and position, and then investigate relationships between tutoring, study time, and results.

This is the detailed discussion notebook, not the abbreviated PDF or JSON summary. The original height example, school marks, club survey, rating tables, bus journey, weighted grades, combined classes, and association examples are retained. Repeated transitions are consolidated so the same lesson is not copied several times. Where an earlier explanation needed a mathematical qualification, the clarification is made in the relevant lesson and recorded in the correction notes.

**How each lesson works**

```text
School situation
      ↓
What problem occurred?
      ↓
Why is the previous tool not enough for this question?
      ↓
New concept and definition
      ↓
Formula and meaning of symbols, when applicable
      ↓
Same example worked step by step
      ↓
What does the answer mean?
      ↓
Cross-question / common confusion / memory trick
      ↓
Two practice questions with expandable answers
```

Read from top to bottom for the storyline, or use the tree and links below for revision. Practice answers are in expandable blocks; a plain-text editor will still show their full contents. Mathematical expressions use standard Markdown `$...$` and `$$...$$` notation. Use a Markdown viewer with math support to render them.

**Scope and conventions**

The examples are illustrative teaching data, not evidence about real schools. Marks are out of 100 unless an example explicitly uses a different scale. Different mini-datasets belong to the same growing school scenario; they are not claimed to be one unchanged set of students across every lesson.

“Why introduced?” explains the practical or mathematical need. It is not a claim that the concepts were historically invented in this exact school-story order.

The main quartile example keeps our original results **52, 66.5, 77**. The percentile lesson states its sample-quantile convention. Population and sample SD/covariance denominators are kept explicit. The point-biserial lesson includes the corrected, convention-matched formulas.

**Tree key:** `[L]` = worked lesson; `[I]` = introduced or briefly discussed; `[P]` = named / still pending. Organising data, numerical summaries, and observed association are all descriptive work; they are separated below for learning order.

## Master concept tree — Parent → child, in study order

```text
STATISTICS — learning sequence
├── [L] 1. Foundations — What are we trying to understand?
│   ├── [L] 1.1 Statistics — Meaning and why it is called Statistics
│   ├── [L] 1.2 Types of Statistics — Descriptive vs Inferential
│   ├── [L] 1.3 Data, variables, observations, and paired observations
│   ├── [L] 1.4 Population, sample, parameters, and statistics — the notation bridge
│   ├── [L] 1.5 Types of data — Categorical, numerical, discrete, continuous
│   └── [L] 1.6 Scales of measurement — Which comparisons make sense?
│       ├── [L] 1.6.1 Nominal — Naming only
│       ├── [L] 1.6.2 Ordinal — Order without guaranteed equal gaps
│       ├── [L] 1.6.3 Interval — Equal gaps, but no true zero
│       └── [L] 1.6.4 Ratio — Equal gaps and a meaningful zero
├── [L] 2. Categorical data — Organise, show, and summarise the categories
│   ├── [L] 2.1 Categorical data — Why the usual arithmetic does not work
│   ├── [L] 2.2 Frequency distribution — Turn a messy list into counts
│   ├── [L] 2.3 Relative and percentage frequency — Counts need a denominator
│   ├── [L] 2.4 Cumulative frequency — How many have we reached so far?
│   ├── [L] 2.5 Bar chart — Make category comparison visible
│   ├── [L] 2.6 Pie chart — Show each category as part of one whole
│   ├── [L] 2.7 Mode for categorical data — The most common category
│   └── [L] 2.8 Median for categorical data — No order, no median
├── [L] 3. Numerical data — From many marks to a meaningful center
│   ├── [L] 3.1 Numerical frequency distributions — Values, intervals, and midpoints
│   ├── [L] 3.2 Measures of central tendency — Why do we need one number?
│   ├── [L] 3.3 The mean family — What exactly are we averaging?
│   │   ├── [L] 3.3.1 Arithmetic Mean — The equal-share and balance-point story
│   │   │   ├── [L] 3.3.1.1 Direct / simple method — Use the values as they are
│   │   │   ├── [L] 3.3.1.2 Assumed mean method — Use a nearby starting point
│   │   │   ├── [L] 3.3.1.3 Step-deviation method — Shrink the offsets, then restore them
│   │   │   └── [L] 3.3.1.4 Weighted Mean — Some values get more votes
│   │   │       └── [L] 3.3.1.4.1 Combined Mean — Group size becomes the weight
│   │   ├── [L] 3.3.2 Geometric Mean — Preserve the multiplied result
│   │   └── [L] 3.3.3 Harmonic Mean — Equal-distance rate problems
│   ├── [L] 3.4 Median — Why mean is not always the typical student
│   ├── [L] 3.5 Mode — The most frequently observed score
│   └── [L] 3.6 Mean vs Median vs Mode — Choose the question before the formula
├── [L] 4. Numerical data — Spread, position, and the five-number picture
│   ├── [L] 4.1 Measures of dispersion — Why the center is not enough
│   ├── [L] 4.2 Range — The first attempt, and why two endpoints are not enough
│   ├── [L] 4.3 Signed deviations and Mean Absolute Deviation — Keep distance, ignore direction
│   ├── [L] 4.4 Variance — Average the squared distances
│   ├── [L] 4.5 Standard Deviation — Bring spread back to the original unit
│   ├── [I] 4.6 Sample variance and SD — Why two denominators appear
│   ├── [L] 4.7 Quartiles — Why median alone is not enough
│   ├── [L] 4.8 Percentiles — Finer landmarks, not percentage marks
│   │   └── [I] 4.8.1 Deciles — A named extension of percentile landmarks
│   ├── [L] 4.9 Interquartile Range — Focus on the middle half
│   ├── [L] 4.10 Five-number summary — Five checkpoints across the class
│   ├── [L] 4.11 Coefficient of Variation — Spread relative to what?
│   └── [I] 4.12 Other dispersion measures we mentioned briefly
│       ├── [I] 4.12.1 Quartile Deviation / Semi-IQR
│       ├── [I] 4.12.2 Coefficient of Range
│       └── [I] 4.12.3 Coefficient of Quartile Deviation
├── [I] 5. Distribution shape and outliers — Connections already introduced
│   ├── [I] 5.1 Symmetry, skewness, and the mean–median–mode pattern
│   ├── [I] 5.2 Outliers — A rule for flagging, not automatic deletion
│   └── [I] 5.3 Box plot — Draw the five-number landmarks
├── [L] 6. Week 4 — Association: What changes when we study two variables?
│   ├── [L] 6.1 Contingency tables — Preserve how categories occur together
│   ├── [L] 6.2 Relative frequencies in contingency tables — Always ask “out of what?”
│   ├── [L] 6.3 Association and independence between categorical variables
│   ├── [L] 6.4 Scatterplots — See how two numerical variables behave together
│   ├── [L] 6.5 Covariance — Turn paired deviations into a number
│   ├── [L] 6.6 Pearson correlation — Standardise covariance
│   └── [L] 6.7 Point-biserial correlation — Two groups, numerical outcomes
└── [P] 7. Named but unfinished branches — Do not confuse a roadmap with a completed lesson
    ├── [P] 7.1 Numerical graphs — Histogram, polygon, ogive, stem-and-leaf
    ├── [P] 7.2 Index of dispersion — Named, not yet developed
    └── [P] 7.3 Probability, sampling, estimation, and tests — The later branch
```

## Jump to a parent chapter

[1. Foundations](#foundations) | [2. Categorical data](#categorical) | [3. Numerical data](#numerical-center) | [4. Numerical data](#spread-position) | [5. Distribution shape and outliers](#shape-previews) | [6. Week 4](#association) | [7. Named but unfinished branches](#roadmap)

[Rapid revision and formula index](#rapid-revision) · [Accuracy notes](#accuracy-notes) · [Technical checks](#technical-references)

<a id="clickable-topic-index"></a>
## Clickable topic index

- [1. Foundations — What are we trying to understand?](#foundations)
  - [1.1 Statistics — Meaning and why it is called Statistics](#statistics-meaning)
  - [1.2 Types of Statistics — Descriptive vs Inferential](#types-statistics)
  - [1.3 Data, variables, observations, and paired observations](#data-basics)
  - [1.4 Population, sample, parameters, and statistics — the notation bridge](#population-sample)
  - [1.5 Types of data — Categorical, numerical, discrete, continuous](#data-types)
  - [1.6 Scales of measurement — Which comparisons make sense?](#scales)
    - [1.6.1 Nominal — Naming only](#nominal-scale)
    - [1.6.2 Ordinal — Order without guaranteed equal gaps](#ordinal-scale)
    - [1.6.3 Interval — Equal gaps, but no true zero](#interval-scale)
    - [1.6.4 Ratio — Equal gaps and a meaningful zero](#ratio-scale)
- [2. Categorical data — Organise, show, and summarise the categories](#categorical)
  - [2.1 Categorical data — Why the usual arithmetic does not work](#categorical-data)
  - [2.2 Frequency distribution — Turn a messy list into counts](#frequency-distribution)
  - [2.3 Relative and percentage frequency — Counts need a denominator](#relative-frequency)
  - [2.4 Cumulative frequency — How many have we reached so far?](#cumulative-frequency)
  - [2.5 Bar chart — Make category comparison visible](#bar-chart)
  - [2.6 Pie chart — Show each category as part of one whole](#pie-chart)
  - [2.7 Mode for categorical data — The most common category](#categorical-mode)
  - [2.8 Median for categorical data — No order, no median](#categorical-median)
- [3. Numerical data — From many marks to a meaningful center](#numerical-center)
  - [3.1 Numerical frequency distributions — Values, intervals, and midpoints](#numerical-frequency)
  - [3.2 Measures of central tendency — Why do we need one number?](#central-tendency)
  - [3.3 The mean family — What exactly are we averaging?](#mean-family)
    - [3.3.1 Arithmetic Mean — The equal-share and balance-point story](#arithmetic-mean)
      - [3.3.1.1 Direct / simple method — Use the values as they are](#direct-mean)
      - [3.3.1.2 Assumed mean method — Use a nearby starting point](#assumed-mean)
      - [3.3.1.3 Step-deviation method — Shrink the offsets, then restore them](#step-deviation)
      - [3.3.1.4 Weighted Mean — Some values get more votes](#weighted-mean)
        - [3.3.1.4.1 Combined Mean — Group size becomes the weight](#combined-mean)
    - [3.3.2 Geometric Mean — Preserve the multiplied result](#geometric-mean)
    - [3.3.3 Harmonic Mean — Equal-distance rate problems](#harmonic-mean)
  - [3.4 Median — Why mean is not always the typical student](#numerical-median)
  - [3.5 Mode — The most frequently observed score](#numerical-mode)
  - [3.6 Mean vs Median vs Mode — Choose the question before the formula](#choose-center)
- [4. Numerical data — Spread, position, and the five-number picture](#spread-position)
  - [4.1 Measures of dispersion — Why the center is not enough](#dispersion)
  - [4.2 Range — The first attempt, and why two endpoints are not enough](#range)
  - [4.3 Signed deviations and Mean Absolute Deviation — Keep distance, ignore direction](#mean-deviation)
  - [4.4 Variance — Average the squared distances](#variance)
  - [4.5 Standard Deviation — Bring spread back to the original unit](#standard-deviation)
  - [4.6 Sample variance and SD — Why two denominators appear](#sample-variance-sd) — introduced
  - [4.7 Quartiles — Why median alone is not enough](#quartiles)
  - [4.8 Percentiles — Finer landmarks, not percentage marks](#percentiles)
    - [4.8.1 Deciles — A named extension of percentile landmarks](#deciles-preview) — introduced
  - [4.9 Interquartile Range — Focus on the middle half](#iqr)
  - [4.10 Five-number summary — Five checkpoints across the class](#five-number-summary)
  - [4.11 Coefficient of Variation — Spread relative to what?](#coefficient-variation)
  - [4.12 Other dispersion measures we mentioned briefly](#other-dispersion) — introduced
    - [4.12.1 Quartile Deviation / Semi-IQR](#quartile-deviation) — introduced
    - [4.12.2 Coefficient of Range](#coefficient-range) — introduced
    - [4.12.3 Coefficient of Quartile Deviation](#coefficient-quartile) — introduced
- [5. Distribution shape and outliers — Connections already introduced](#shape-previews) — introduced
  - [5.1 Symmetry, skewness, and the mean–median–mode pattern](#shape-skewness) — introduced
  - [5.2 Outliers — A rule for flagging, not automatic deletion](#outliers) — introduced
  - [5.3 Box plot — Draw the five-number landmarks](#box-plot) — introduced
- [6. Week 4 — Association: What changes when we study two variables?](#association)
  - [6.1 Contingency tables — Preserve how categories occur together](#contingency-table)
  - [6.2 Relative frequencies in contingency tables — Always ask “out of what?”](#contingency-relative)
  - [6.3 Association and independence between categorical variables](#categorical-association)
  - [6.4 Scatterplots — See how two numerical variables behave together](#scatterplots)
  - [6.5 Covariance — Turn paired deviations into a number](#covariance)
  - [6.6 Pearson correlation — Standardise covariance](#pearson)
  - [6.7 Point-biserial correlation — Two groups, numerical outcomes](#point-biserial)
- [7. Named but unfinished branches — Do not confuse a roadmap with a completed lesson](#roadmap) — pending
  - [7.1 Numerical graphs — Histogram, polygon, ogive, stem-and-leaf](#numerical-graphics-roadmap) — pending
  - [7.2 Index of dispersion — Named, not yet developed](#index-dispersion-roadmap) — pending
  - [7.3 Probability, sampling, estimation, and tests — The later branch](#inference-roadmap) — pending


---
<a id="foundations"></a>
## 1. Foundations — What are we trying to understand?

Our notebook began with student heights. We then chose **a school and student marks** as the main running story. Both are retained: the original example introduces the idea, and the school story grows from there.

The principal's questions become more demanding one chapter at a time. We do not introduce a formula until there is a question for it to answer.

[Back to the topic index](#clickable-topic-index)


<a id="statistics-meaning"></a>
### 1.1 Statistics — Meaning and why it is called Statistics

**Statistics is the science of collecting, organizing, analyzing, and interpreting data so that we can understand what the data is telling us.**

**Simple example — our original discussion**

Suppose we have the heights of 5 students:

```text
Student →   A    B    C    D    E
Height  →  160  165  170  175  180 cm
```

Just having these numbers is **data**.

Statistics helps us ask questions such as:

- What is the **average height**?
- Which height is most common?
- How much do the heights differ?
- Can these 5 students tell us something about a larger group?

So think:

> **Data = numbers/information**  
> **Statistics = making sense of that data**

**Why is it called “Statistics”?**

The word **statistics** is historically connected to information about the **state**. Governments collected information about population, births and deaths, taxes, land, and military resources to understand the condition of the state.

Over time, the subject expanded beyond government information to students, businesses, medicine, sports, science, and other kinds of data. This is the historical connection discussed in our chat; the later “why needed?” stories explain mathematical motivation, not a claim that every concept was invented by one person in that exact sequence.

**Our story changes to school marks**

Imagine a school has **100 students** who took a Mathematics exam:

```text
Student A → 72
Student B → 85
Student C → 61
Student D → 90
Student E → 74
...
100 students
```

The principal asks:

> How is the class performing overall?  
> What is the typical mark?  
> How many students are struggling?  
> Are students scoring similarly, or are their marks very different?

Simply looking at 100 numbers will not answer these questions easily. We need ways to turn observations into understanding.

> **Statistics is the study of data and the methods used to turn data into useful information.**

```text
Collect data
     ↓
Organize it
     ↓
Summarize it
     ↓
Analyze it
     ↓
Understand what it means
     ↓
Make a decision
```

**Formula?** There is no single formula for Statistics. Each question will introduce its own appropriate tool.

**Memory:** **Statistics = Data → Understand → Decision.**

**Try it yourself**

1. Are the five heights themselves Statistics, or data?
2. Find the mean of the original heights. What does the result tell us?

<details>
<summary>Answers and explanations — open after trying</summary>

1. They are observations: data. Organizing or summarizing them, for example by calculating the mean, is a statistical operation.

2. The total is 850 cm. The mean is 850/5 = 170 cm: the equal-share height of these five students. It does not by itself establish the mean height of the whole school.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="types-statistics"></a>
### 1.2 Types of Statistics — Descriptive vs Inferential

Let’s continue our **school marks story**. The principal can ask two different kinds of questions.

**Problem 1: “What happened in the students whose marks I have?”**

He might report a class average, the highest and lowest marks, or the percentage passing. He is describing the observed group.

> **Descriptive Statistics = Summarizing and describing existing data.**

```text
100 students' marks
        ↓
Summarize them
        ↓
“What does this group look like?”
```

Descriptive work includes tables, graphs, mean, median, mode, spread, and observed association. Organizing and presenting data are part of descriptive statistics too; they appear earlier in our study order because we need them before many calculations.

**Problem 2: “Can this smaller group tell me something about everyone?”**

Now imagine the school actually has **2,000 students**, but the principal studies only **100**. Suppose their average is 72.

> “Can I use these 100 students to estimate how all 2,000 students are performing?”

Now we are going beyond what was directly observed.

> **Inferential Statistics = Using a sample to reason about a larger population, while accounting for uncertainty.**

```text
100 students → study their marks → estimate → all 2,000 students
```

The sample average is not automatically the population average. How students were selected matters. Taking only the highest-scoring class would not give a fair picture of the whole school.

**The three big descriptive questions**

```text
                    STUDENT MARKS
                         ↓
              Descriptive Statistics
                         ↓
        ┌────────────────┼────────────────┐
        ↓                ↓                ↓
      Center           Spread           Shape
        ↓                ↓                ↓
Where is a typical   How different   How are values
      value?         are students?     distributed?
```

Later, **association** adds: “How do two variables behave together?”

**Cross-question:** Can a sample have descriptive statistics? Yes. Describing the 100 students is descriptive; using them to estimate all 2,000 is inferential. The distinction is the claim, not merely whether a sample was collected.

**Memory:** **Descriptive = describe what we have. Inferential = reason beyond what we directly observed.**

**Try it yourself**

1. “These 100 students averaged 72.” Is this descriptive or inferential?
2. “Therefore all 2,000 students average exactly 72.” What is missing?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Descriptive: it reports a feature of the observed group.

2. An inference and its uncertainty need justification. The sample design may be biased, and the population mean need not equal the sample mean.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="data-basics"></a>
### 1.3 Data, variables, observations, and paired observations

The principal adds columns to the school register:

| Student | House | Marks | Study hours | Tutoring |
|---|---|---:|---:|---|
| A | Blue | 50 | 1 | No |
| B | Red | 60 | 2 | Yes |
| C | Blue | 70 | 3 | Yes |

**The problem:** Before choosing a statistical tool, we must know what one row and one column represent.

An **observational unit** is the thing being studied: here, a student. A **variable** is a characteristic recorded for each unit: marks, house, or study hours. An **observation** is a recorded value; one student's complete record contains observations on several variables.

**Why this matters later**

If student A studied 1 hour and scored 50, the pair is:

$$
(x_A,y_A)=(1,50).
$$

Here $x_A$ is A's study time and $y_A$ is A's mark. We must not independently sort the study hours and marks and accidentally pair one student's hours with another student's result.

```text
One column → distribution of one variable
Two correctly paired columns → association between variables
```

**Cross-question:** Are numerical labels automatically measurements? No. Student ID 101 is an identifier, not a quantity of “student-ness.”

**Memory:** **Row = whose record? Column = which characteristic? Pair = the same student's two values.**

**Try it yourself**

1. In the table, what is the variable and what is the observational unit for Marks?
2. Can you sort the hours and marks separately before computing correlation?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Marks is the variable; each student is an observational unit.

2. No. That can destroy or fabricate the relationship by changing the student-by-student pairings.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="population-sample"></a>
### 1.4 Population, sample, parameters, and statistics — the notation bridge

**The story:** The school has 2,000 students. The principal measures 100 because studying everyone is difficult.

> **Population = the entire group we want to understand.**  
> **Sample = the subset we actually observe.**

A **parameter** describes the population. A **statistic** is calculated from a sample. This distinction explains why different symbols appear in formulas.

| Quantity | Population | Sample |
|---|---|---|
| Number of observations | $N$ | $n$ |
| Mean | $\mu$ | $\bar{x}$ |
| Variance | $\sigma^2$ | $s^2$ |
| Standard deviation | $\sigma$ | $s$ |
| Correlation | $\rho$ | $r$ |

Read $\mu$ as **mu**, $\sigma$ as **sigma**, $\rho$ as **rho**, and $\bar{x}$ as **x-bar**.

**Mean formulas**

$$
\mu=\frac{\sum_{i=1}^{N}x_i}{N},
\qquad
\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}.
$$

$x_i$ means the value for observation $i$. The summation symbol $\sum$ means add all indicated terms; $i=1$ to $n$ means start with the first and finish with the last sample observation.

**Why this is not merely a class-size distinction**

Five students can be a population if the question is specifically about those five students. The same five can be a sample if the goal is to estimate a larger school.

**Status:** We discussed this distinction and the notation. Sampling methods, estimation, confidence intervals, and hypothesis testing remain later chapters, not completed topics.

**Memory:** **Population → parameter. Sample → statistic.**

**Try it yourself**

1. You measure every student in Class A but want to understand the whole school. Population or sample?
2. Which symbol represents the population SD: Σ or σ?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Relative to the whole-school question, Class A is a sample. Relative to a question only about Class A, it is the complete population.

2. Lowercase σ represents population standard deviation. Uppercase Sigma/the summation operator Σ or ∑ tells us to add terms.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="data-types"></a>
### 1.5 Types of data — Categorical, numerical, discrete, continuous

Until now, we have mostly worked with marks. But the school also records house, club, result, height, and study time.

**The problem:** We cannot treat every column as the same kind of number.

> **Categorical data tells us “which group?” rather than “how much?”**

Examples: Blue House, Music Club, Pass, Good. **Numerical data** records quantities: number of absences, marks, height, study duration.

```text
DATA
├── Qualitative / Categorical
│   ├── Nominal → names with no natural order
│   └── Ordinal → categories with a meaningful order
└── Quantitative / Numerical
    ├── Discrete → distinct countable possible values
    └── Continuous → a quantity modeled on a continuum
```

**Discrete vs continuous — a short foundational bridge**

The principal counts absences: 0, 1, 2, 3 days. Under a whole-day attendance rule, 2.37 absences is not a possible count. That variable is discrete.

Study duration can be 2 hours, 2.1 hours, or 2.125 hours. The underlying duration is continuous, even if a form rounds it to whole hours.

**Cross-question:** Does “has decimals” mean continuous? No. Marks awarded in half-point steps are still discrete. Does “recorded as a whole number” mean discrete? Not necessarily: a rounded height is a recorded version of a continuous measurement.

**Formula?** No special formula identifies a data type. Ask what the possible values mean, not just what they look like.

**Memory:** **Categories classify. Numbers quantify. Counts are discrete; measurements may be continuous.**

**Try it yourself**

1. Classify school house, number of students, and measured height.
2. Poor = 1, Average = 2, Good = 3. Have these labels become numerical measurements?

<details>
<summary>Answers and explanations — open after trying</summary>

1. House: categorical nominal. Number of students: numerical discrete. Measured height: numerical continuous.

2. No. They are ordered category codes unless an equal-interval measurement interpretation is separately justified.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="scales"></a>
### 1.6 Scales of measurement — Which comparisons make sense?

The principal asks:

> “Can we perform the same mathematical operations on every kind of data?”

Can we calculate Blue + Red? Does 2nd rank mean twice 1st rank? Is 20°C twice 10°C in temperature? These questions expose the need for **scales of measurement**.

> **A scale of measurement tells us the level of information contained in a variable and what comparisons or mathematical operations are meaningful.**

```text
Nominal  → Name
Ordinal  → Name + Order
Interval → Name + Order + Equal intervals
Ratio    → Name + Order + Equal intervals + True zero
```

The scale is about meaning. It is not decided by whether a spreadsheet cell contains a digit.

**Memory:** **N-O-I-R: Name → Order → Intervals → Real zero.**

**Try it yourself**

1. Why do we need measurement scales before choosing an average?
2. What extra property distinguishes ratio from interval measurement?

<details>
<summary>Answers and explanations — open after trying</summary>

1. They tell us whether categories, ordering, numerical differences, and ratios are meaningful, which affects the interpretation of the average.

2. A meaningful absolute zero, which makes ratios of values meaningful.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="nominal-scale"></a>
#### 1.6.1 Nominal — Naming only

The school records:

```text
Student A → Blue House
Student B → Red House
Student C → Green House
Student D → Blue House
```

**The problem:** Blue and Red are distinct, but neither is naturally greater than the other. We need to summarize categories without inventing arithmetic.

> **Nominal scale classifies observations into different categories or names without any meaningful order.**

We can count Blue House students and find the most common house. We cannot calculate a meaningful “average house.”

If the coding is Blue = 1, Red = 2, Green = 3, the coding does not create equal gaps or a meaningful mean. Changing the codes must not change the substantive conclusion.

**Useful calculations:** frequency $f_i$, proportion $f_i/n$, percentage $(f_i/n)\times100\%$, and mode. Here $f_i$ is category $i$'s count and $n$ is the total count.

**Memory:** **Nominal = Name only.**

**Try it yourself**

1. Is student ID 103 greater than ID 101 in a quantitative statistical sense?
2. Which center can summarize house membership: mean, median, or mode?

<details>
<summary>Answers and explanations — open after trying</summary>

1. No. The IDs identify students; subtraction between them does not measure a student characteristic.

2. Mode: the most frequent house. There is no natural median or arithmetic mean of the house categories.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="ordinal-scale"></a>
#### 1.6.2 Ordinal — Order without guaranteed equal gaps

The principal ranks students:

```text
1st → 95 marks
2nd → 94 marks
3rd → 80 marks
```

**The new information:** We know who is ahead. **The remaining problem:** Ranks do not tell us how far ahead.

```text
1st to 2nd → 1 mark
2nd to 3rd → 14 marks
```

> **Ordinal scale classifies observations into categories that have a meaningful order, but the distance between categories is not necessarily equal or measurable.**

Another example:

```text
Poor < Average < Good < Very Good < Excellent
```

We can find the middle category, the most common category, and cumulative frequencies in this order. But “Excellent is twice Average” is not justified merely because the categories were coded 4 and 2.

**Formula?** Median position can be located using $(n+1)/2$ for odd $n$; for even $n$, inspect positions $n/2$ and $n/2+1$. We do not average category names.

**Memory:** **Ordinal = Order, not equal distance.**

**Try it yourself**

1. The top three students are ranked 1, 2, 3. Must adjacent students differ by equal marks?
2. Are medians possible for Poor, Average, Good, Excellent?

<details>
<summary>Answers and explanations — open after trying</summary>

1. No. Ranking preserves order, not numerical gaps.

2. Yes, because the categories can be ordered. If two central observations differ, a category-median convention must be stated rather than averaging arbitrary codes.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="interval-scale"></a>
#### 1.6.3 Interval — Equal gaps, but no true zero

The school records classroom temperature:

```text
Room A → 10°C
Room B → 20°C
Room C → 30°C
```

Now the differences are meaningful:

$$
20-10=10,\qquad30-20=10.
$$

Both gaps represent the same temperature difference. But 0°C is not an absence of temperature.

> **Interval scale has ordered values with equal and meaningful differences between them, but it does not have a true absolute zero.**

**The problem it solves:** It distinguishes valid comparisons of differences from invalid ratios of raw readings.

“20°C is twice 10°C” is not an invariant temperature-ratio claim. Convert the same readings to Fahrenheit: 68°F and 50°F. The ratio changes because the origin changes.

Means and SDs can meaningfully summarize temperatures on a given interval scale; the mean transforms with the origin and unit, while SD responds to the unit but not an added constant.

**Formula illustration:** $F=(9/5)C+32$, where $C$ and $F$ are Celsius and Fahrenheit readings. The added 32 shows why ratios of raw readings depend on the scale's zero.

**Memory:** **Interval → differences are meaningful; raw-value ratios are not.**

**Try it yourself**

1. Does 0°C mean no temperature?
2. Can you make Celsius ratio-scale merely by subtracting the lowest classroom reading?

<details>
<summary>Answers and explanations — open after trying</summary>

1. No. It is a chosen reference point on the Celsius scale.

2. No. An arbitrary recentering does not create a physically meaningful absolute zero. Converting to an absolute temperature scale is different from inventing a baseline.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="ratio-scale"></a>
#### 1.6.4 Ratio — Equal gaps and a meaningful zero

The school records study duration:

```text
Student A → 2 hours
Student B → 4 hours
```

Zero hours means no elapsed study time. Four hours is genuinely twice two hours.

> **Ratio scale has ordered values, equal intervals, and a true absolute zero, so both differences and ratios are meaningful.**

Examples include height, distance, elapsed time, mass, and counts of students or correct answers.

$$
\frac{4\text{ hours}}{2\text{ hours}}=2.
$$

The same ratio holds in minutes: $240/120=2$. This invariance is exactly what fails for raw Celsius ratios.

**Why this matters for our later CV chapter:** Dividing SD by the mean depends on a meaningful zero. Changing an arbitrary baseline changes that ratio even if the spread stays unchanged.

**Marks need interpretation.** On the same scoring system, 80 points is twice 40 points earned; it does not establish twice the knowledge or ability. A zero score means no points under that scoring rule, not necessarily no knowledge. We keep marks as our teaching example without making unsupported ability-ratio claims.

**Memory:** **Ratio → “how much more?” AND “how many times?”**

**Try it yourself**

1. Is 0 students a true zero for student count?
2. Is someone scoring 80 necessarily twice as knowledgeable as someone scoring 40?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Yes. It represents the absence of students in the counted group.

2. No. Ratios of earned points do not automatically measure ratios of underlying knowledge or ability.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="categorical"></a>
## 2. Categorical data — Organise, show, and summarise the categories

The principal now asks students about clubs and satisfaction. Marks alone cannot answer these questions. We move from **how much?** to **which group?**, while staying in the same school.

```text
Raw category answers
        ↓
Frequency distribution
        ↓
Relative and percentage frequencies
        ↓
Bar chart / pie chart
        ↓
Most common category → Mode
        ↓
Middle ordered category → Median, when order exists
```

[Back to the topic index](#clickable-topic-index)


<a id="categorical-data"></a>
### 2.1 Categorical data — Why the usual arithmetic does not work

Suppose the school asks 10 students:

> “Which club do you prefer?”

```text
Music, Sports, Music, Coding, Sports,
Music, Drama, Coding, Music, Sports
```

**The problem:** We cannot calculate `(Music + Sports + Coding) / 3`. The responses are not measurements on a numerical scale.

> **Categorical data is data that places observations into groups or categories based on qualities, labels, or characteristics rather than measurable numerical amounts.**

This classification tells us to use counts, proportions, and categories rather than arithmetic on the labels.

```text
Club = categorical variable
Music / Sports / Coding / Drama = categories
```

With club preference, there is no natural order: **nominal**. With performance ratings `Poor < Average < Good < Excellent`, there is a natural order: **ordinal**.

**Cross-question — what about Pass = 1 and Fail = 0?**

The mean of arbitrary nominal codes is generally meaningless. But a deliberately defined **0/1 indicator** has a useful special interpretation:

$$
\frac{1+0+1+1+0}{5}=\frac35=0.60.
$$

It is the proportion passing, not an “average label.” This distinction will matter again for point-biserial correlation.

**Memory:** **Categorical data asks “which group?” Numerical data asks “how much?”**

**Try it yourself**

1. What are the four frequencies in the 10-student club list?
2. Why is averaging arbitrary club codes different from averaging a Pass indicator?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Music = 4, Sports = 3, Coding = 2, Drama = 1. Total = 10.

2. Club codes have no meaningful numerical scale. An indicator is explicitly 1 when a condition holds and 0 otherwise, so its mean counts the proportion satisfying that condition.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="frequency-distribution"></a>
### 2.2 Frequency distribution — Turn a messy list into counts

Let’s continue our **school categorical-data story**. The school now asks **20 students** which extracurricular club they prefer.

```text
Music
Sports
Coding
Music
Drama
Sports
Music
Coding
Sports
Music
Music
Drama
Coding
Sports
Music
Sports
Coding
Music
Drama
Sports
```

**What problem occurred?**

The principal keeps rereading the list:

> “How many chose Music? Which club is most popular? How many chose Coding?”

The observations are valid, but the pattern is hard to inspect. So we count each category once and record its total.

> **Frequency means how many times something occurs.**

> **A frequency distribution is a table or summary that shows each category and the number of observations belonging to that category.**

| Club | Frequency |
|---|---:|
| Music | 7 |
| Sports | 6 |
| Coding | 4 |
| Drama | 3 |
| **Total** | **20** |

**Why “distribution”?** We are seeing how the 20 answers are distributed across categories.

```text
20 separate answers
        ↓
Music 7 / Sports 6 / Coding 4 / Drama 3
```

**Formula and symbols**

$$
\boxed{\sum_{i=1}^{k}f_i=n}
$$

$f_i$ is the frequency of category $i$; $k$ is the number of categories; $n$ is the total number of observations. Here $k=4$, and $7+6+4+3=20$.

This identity assumes each student contributes exactly one classified answer. If students may choose several clubs, the total frequency counts **selections**, not necessarily distinct students. We must say which is being counted.

**Cross-question:** Does averaging 7, 6, 4, 3 give an average club? No. $20/4=5$ is the average number of students **per listed category**, not an average club preference.

**Memory:** **Frequency = how often. Distribution = how the total is shared across categories.**

**Try it yourself**

1. How many students selected something other than Music?
2. The table totals 25 for a 20-student survey. Is that automatically an error?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 20 − 7 = 13 students.

2. Not if multiple selections were allowed. But then the unit is selections, and a percentage-of-students or part-of-whole interpretation requires care.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="relative-frequency"></a>
### 2.3 Relative and percentage frequency — Counts need a denominator

The principal knows Music has 7 supporters out of 20. Another school reports 70 Music supporters. Is Music more popular there?

**The new problem:** The other school may have 1,000 students. Bigger counts can simply reflect bigger groups.

> **Relative frequency is the fraction or proportion of the relevant total belonging to a category.**

We change the question from **“How many?”** to **“How many out of how many?”**

$$
\boxed{\text{Relative frequency}_i=\frac{f_i}{n}}
$$

$$
\boxed{\text{Percentage frequency}_i=\frac{f_i}{n}\times100\%}
$$

$f_i$ is category frequency; $n$ is total observations. Multiplication by $100\%$ expresses the proportion as a percentage.

| Club | Frequency | Relative frequency | Percentage |
|---|---:|---:|---:|
| Music | 7 | 0.35 | 35% |
| Sports | 6 | 0.30 | 30% |
| Coding | 4 | 0.20 | 20% |
| Drama | 3 | 0.15 | 15% |
| **Total** | **20** | **1.00** | **100%** |

For Music:

$$
\frac7{20}=0.35=35\%.
$$

That is the observed share in this survey. It does not automatically establish the share in every school.

**The unequal-school example from our discussion**

| School | Music supporters | Total students | Music share |
|---|---:|---:|---:|
| A | 40 | 100 | 40% |
| B | 60 | 300 | 20% |

School B has **more Music supporters**, but School A has the **higher proportion**.

```text
Raw frequency → 60 > 40
Relative frequency → 20% < 40%
```

Both statements are correct; they answer different questions.

**Cross-question:** Do percentages always total exactly 100% on the printed table? The unrounded proportions do, for mutually exclusive exhaustive categories. Independently rounded percentages may total 99.9% or 100.1%.

**Memory:** **Count answers “how many?” Proportion answers “how much of the relevant whole?”**

**Try it yourself**

1. What fraction and percentage selected Coding or Drama?
2. Group A has 20 passes out of 25; Group B has 20 out of 40. Which has the higher pass rate?

<details>
<summary>Answers and explanations — open after trying</summary>

1. (4 + 3)/20 = 7/20 = 0.35 = 35%.

2. A: 80%; B: 50%. Equal raw counts do not imply equal rates.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="cumulative-frequency"></a>
### 2.4 Cumulative frequency — How many have we reached so far?

Club categories have no natural order. But suppose students rate a lesson:

```text
Poor < Average < Good < Very Good < Excellent
```

The principal asks:

> “How many students rated the lesson Good or below?”

**The problem:** A category frequency counts only Good. We need all observations up to that point in the meaningful order.

> **Cumulative frequency is the running total of frequencies up to a given ordered category or value.**

| Rating | Frequency | Cumulative frequency | Positions occupied |
|---|---:|---:|---|
| Poor | 2 | 2 | 1–2 |
| Average | 5 | 7 | 3–7 |
| Good | 8 | 15 | 8–15 |
| Very Good | 4 | 19 | 16–19 |
| Excellent | 1 | 20 | 20 |

$$
\boxed{F_i=\sum_{j=1}^{i}f_j}
$$

$F_i$ is the cumulative count through category $i$; $f_j$ is the frequency of category $j$; $j=1$ to $i$ means add from the first category up to the current one.

For Good:

$$
F_{\text{Good}}=2+5+8=15,
\qquad\frac{15}{20}\times100\%=75\%.
$$

**What does this solve?** We can now locate thresholds and middle positions without expanding every repeated label. This is exactly what we will need for an ordinal median.

**Cross-question:** Could we mechanically accumulate Music, Sports, Coding, Drama? Yes, but the result changes with an arbitrary ordering and is not a natural “at or below” summary of club preference. Cumulative frequencies are useful when the order means something.

**Memory:** **Frequency = in this category. Cumulative frequency = up to this category.**

**Try it yourself**

1. How many students rated the lesson Average or below?
2. Which category contains observation 17?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 2 + 5 = 7 students, or 35%.

2. Very Good, because that category occupies positions 16–19.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="bar-chart"></a>
### 2.5 Bar chart — Make category comparison visible

The frequency table is already better than the raw list:

```text
Music  → 7
Sports → 6
Coding → 4
Drama  → 3
```

But the principal asks:

> “Can I understand the comparison even faster?”

**The problem:** Reading exact numbers is useful, but the overall ordering can be shown directly by length.

> **A bar chart is a graph used to represent categorical data using rectangular bars whose lengths or heights are proportional to the frequency, percentage, or value of each category.**

```text
Preferred club — 20 students
Each block = one student

Music   ███████  7
Sports  ██████   6
Coding  ████     4
Drama   ███      3
```

We can immediately see that Music is highest, Drama lowest, and Sports close to Music.

**What goes on the axes?**

In a vertical chart, categories usually go on the horizontal axis and counts or percentages on the vertical axis. A horizontal chart reverses those roles and is useful for long category names.

**Formula?** The chart itself needs no new statistical formula:

$$
\text{Bar length}\propto f_i.
$$

The symbol $\propto$ means “is proportional to.” A percentage chart uses $(f_i/n)\times100\%$ instead. Scaling all bars from counts to percentages preserves their relative pattern for one fixed total.

**Why are there gaps?**

Music and Sports are separate categories, not adjacent numerical intervals. Gaps emphasize that distinction.

```text
Bar chart → separate categories → separate bars
Histogram → adjacent numerical intervals → touching rectangles
```

The variable type is the real distinction, not gaps alone. A histogram can also have an empty interval.

**Order matters differently**

Nominal bars can be alphabetic or sorted by frequency. Ordinal bars should generally preserve `Poor → Average → Good → Very Good → Excellent` rather than sorting away the meaning.

**Important reading checks**

Use a zero baseline when bar lengths encode magnitude. Otherwise, a small difference such as 7 versus 6 can look enormous. Use equal-width bars, clear labels, and consistent units. A count chart compares absolute numbers; a percentage chart compares shares when group sizes differ.

**Cross-question:** Why not connect club categories with a line? That suggests a progression between nominal categories that does not exist.

**Memory:** **Bar chart = compare categories. Tallest bar = modal category.**

**Try it yourself**

1. Does the Music bar become relatively taller if all counts are converted to percentages?
2. Should Poor, Average, Good, Very Good, Excellent be sorted by frequency?

<details>
<summary>Answers and explanations — open after trying</summary>

1. No. 7/20 and 6/20 keep the same ratio as 7 and 6. Only the axis unit changes.

2. Normally preserve their ordinal order; otherwise the ordered meaning becomes harder to see.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="pie-chart"></a>
### 2.6 Pie chart — Show each category as part of one whole

The principal now asks a different question:

> “Can I show how much of the whole class belongs to each category?”

A bar chart can show percentages, but a circle offers a direct whole-and-parts picture.

> **A Pie Chart is a circular graph divided into sectors, where each sector represents the proportion or percentage of the whole belonging to a category.**

```text
Entire class = 20 students = 100%
Entire circle = 360°
Category's fraction of class = same fraction of circle
```

**Where does the angle formula come from?**

$$
\boxed{\theta_i=\frac{f_i}{n}\times360^\circ}
$$

$\theta_i$ (theta) is the sector angle; $f_i$ is category count; $n$ is total count. A half of the students should occupy a half of the circle: $180^\circ$.

| Club | Frequency | Percentage | Sector angle |
|---|---:|---:|---:|
| Music | 7 | 35% | $126^\circ$ |
| Sports | 6 | 30% | $108^\circ$ |
| Coding | 4 | 20% | $72^\circ$ |
| Drama | 3 | 15% | $54^\circ$ |
| **Total** | **20** | **100%** | **$360^\circ$** |

For Music:

$$
\frac7{20}\times360^\circ=126^\circ.
$$

For Sports, Coding, and Drama:

$$
\frac6{20}\times360^\circ=108^\circ,
\quad\frac4{20}\times360^\circ=72^\circ,
\quad\frac3{20}\times360^\circ=54^\circ.
$$

Check: $126+108+72+54=360$.

If a percentage is supplied as the number 35, the shortcut is:

$$
\boxed{\text{Angle}=\text{percentage number}\times3.6^\circ}.
$$

Do not multiply the decimal proportion 0.35 by 3.6; use $0.35\times360$.

**Another school example — Pass and Fail**

For 80 passes and 20 failures out of 100, the angles are $288^\circ$ and $72^\circ$.

**When does it help?** Few mutually exclusive categories that exhaust one meaningful whole. The largest slice shows the modal category. For many tiny slices, or comparing 24% with 26%, a bar chart is generally easier to read.

**Cross-question:** What if students choose several clubs? Counts of memberships are not non-overlapping shares of students. A pie could describe the share of all **selections**, if clearly labelled, but not falsely present each student as belonging to only one slice.

**Memory:** **Bar = compare categories. Pie = parts of a whole. $100\%=360^\circ$.**

**Try it yourself**

1. A category represents 25%. What is its angle?
2. A slice is 72°. How many students does it represent in a class of 20?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 25 × 3.6° = 90°.

2. 72/360 = 0.20 of the class. 0.20 × 20 = 4 students.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="categorical-mode"></a>
### 2.7 Mode for categorical data — The most common category

The principal asks:

> “Which club is the most popular?”

We cannot find a meaningful arithmetic average of Music and Sports. Nominal categories have no natural middle either. But they do have frequencies.

> **Mode is the value or category that occurs with the highest frequency in a dataset.**

For categorical data:

> **Mode = most common category.**

| Club | Frequency |
|---|---:|
| Music | 7 |
| Sports | 6 |
| Coding | 4 |
| Drama | 3 |

The maximum frequency is 7; the category with that frequency is Music.

$$
\boxed{\text{Mode}=\text{Music}}
$$

**Rule, rather than arithmetic on labels**

$$
\boxed{\text{Mode}=\text{category or categories corresponding to }\max(f_i)}
$$

$\max$ means maximum. The frequency is **7**; the mode is **Music**. Do not confuse the count with the category.

```text
Frequency table → highest count
Bar chart       → longest/tallest bar
Pie chart       → largest slice
```

**The school-uniform example**

| Size | Students |
|---|---:|
| S | 20 |
| M | 45 |
| L | 30 |
| XL | 5 |

Mode = M. That helps the school identify the most frequently needed uniform size. A numerical mean of the labels would not answer the question.

**Can there be several modes?**

`Music 6, Sports 6, Coding 4, Drama 2` gives two modes: Music and Sports (**bimodal**). Three highest-frequency ties are multimodal. If all categories have frequency 5, there is no unique mode; conventions may describe all as tied modes or say there is no single mode.

**Mode does not mean majority**

Music's 35% is the largest share, but a strict majority requires **more than 50%**. The modal category need not contain most students in the “more than half” sense.

**Other original examples**

Blood groups `A, O, B, A, AB, O, O, A, B, O` give A = 3, B = 2, AB = 1, O = 4. Mode = O. Ordered satisfaction categories also have a mode: ordering is not required, but it does not prevent frequency counting.

**Memory:** **Most common ≠ necessarily a majority.**

**Try it yourself**

1. Music has frequency 7 and share 35%. State the mode, modal frequency, and whether it has a majority.
2. What happens when Music and Sports both have the largest count?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Mode: Music. Modal frequency: 7. It does not have a majority because 35% is less than 50%.

2. Both are modes. Report the tie rather than choosing one arbitrarily.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="categorical-median"></a>
### 2.8 Median for categorical data — No order, no median

Now students give **ordered** ratings. The principal asks:

> “What is the middle satisfaction level of the students?”

Mode finds the most frequent category, not necessarily the category containing the middle student. So order gives us another useful summary.

> **The median category is the category containing the middle ordered observation, with an explicit convention when two central categories differ.**

This is meaningful for ordinal data, not ordinary nominal categories such as Music, Sports, Coding, Drama.

**Our 20-student rating example**

| Rating | Frequency | Cumulative frequency | Observation positions |
|---|---:|---:|---|
| Poor | 2 | 2 | 1–2 |
| Average | 5 | 7 | 3–7 |
| Good | 8 | 15 | 8–15 |
| Very Good | 4 | 19 | 16–19 |
| Excellent | 1 | 20 | 20 |

For $n=20$, the central observations are 10th and 11th. Both fall in Good.

$$
\boxed{\text{Median category}=\text{Good}}
$$

**What does it mean?** At least half the observations are at or below Good, and at least half are at or above Good. With ties, these proportions can be **more than half**: here 75% are at or below Good and 65% at or above Good. It is not a claim that exactly 50% are strictly below and 50% strictly above.

**Formula for positions**

For odd $n$:

$$
\boxed{\text{Middle position}=\frac{n+1}{2}}
$$

For even $n$:

$$
\boxed{\text{Central positions}=\frac n2\text{ and }\frac n2+1}
$$

$n$ is the number of observations. Use cumulative frequency to discover which category contains each position.

**A different example — Mode and Median disagree**

| Rating | Frequency | Cumulative frequency |
|---|---:|---:|
| Poor | 6 | 6 |
| Average | 4 | 10 |
| Good | 3 | 13 |
| Very Good | 2 | 15 |
| Excellent | 1 | 16 |

Mode = Poor, because its frequency is highest. For 16 observations, the 8th and 9th are both Average. Median = Average.

```text
Mode   → Which category repeats most?
Median → Which category occupies the middle position?
```

**What if the two middle categories differ?**

```text
Poor, Average, Good, Very Good, Excellent, Excellent
                  ↑       ↑
                  two middle observations
```

Do not calculate `(Good + Very Good)/2`, or average arbitrary codes into a supposedly measured 3.5. Report the two central categories or follow a stated lower/upper category-quantile convention. There is no justified equal-distance midpoint without extra assumptions.

For 9 ordered ratings `Poor, Poor, Average, Average, Good, Good, Very Good, Very Good, Excellent`, the 5th observation is Good.

**Memory:** **No order → no median. Order → use positions, not arithmetic on category labels.**

**Try it yourself**

1. In the 16-student example, why are Mode and Median different?
2. If the two middle ratings are Good and Very Good, can you automatically label the median “3.5”?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Poor has the largest single frequency, while the cumulative count places the 8th and 9th students in Average.

2. No. That assumes numerical distances between codes. Report the middle-category pair or use a specified ordinal-median convention.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="numerical-center"></a>
## 3. Numerical data — From many marks to a meaningful center

We return to Mathematics marks. The categorical chapter taught us to count and organize observations. Now we ask what numerical operations can add to that picture.

The learning order keeps related ideas together: organize the marks → understand central tendency → study the mean family → understand median and mode → choose the right summary.

[Back to the topic index](#clickable-topic-index)


<a id="numerical-frequency"></a>
### 3.1 Numerical frequency distributions — Values, intervals, and midpoints

The teacher has too many marks to list comfortably. We have already solved a similar problem for categories: count repetitions.

**Ungrouped frequency distribution**

> An ungrouped frequency distribution lists individual observed values and their frequencies.

| Mark $x_i$ | Students $f_i$ |
|---|---:|
| 60 | 2 |
| 70 | 5 |
| 80 | 3 |

This represents `60, 60, 70, 70, 70, 70, 70, 80, 80, 80` exactly.

**The next problem:** With many distinct marks, this table can still be long. We group neighboring scores into intervals.

> A grouped frequency distribution records how many observations fall into each specified numerical interval.

Our original 1,000-student example:

| Marks interval | Number of students | Midpoint |
|---|---:|---:|
| $40\le x<50$ | 80 | 45 |
| $50\le x<60$ | 180 | 55 |
| $60\le x<70$ | 300 | 65 |
| $70\le x<80$ | 250 | 75 |
| $80\le x<90$ | 140 | 85 |
| $90\le x\le100$ | 50 | 95 |
| **Total** | **1,000** | |

The endpoint convention is explicit so a score of 50 is not counted in two intervals. The final interval includes 100.

**The vocabulary we placed in the master tree**

A **class interval** is one range of values. **Class boundaries** are the actual cut-points separating adjacent intervals. **Class limits** are the stated lowest and highest class values; their relation to boundaries depends on how data are recorded. For integer scores reported as 40–49, boundaries may be 39.5 and 49.5 when rounding conventions justify them. Do not automatically apply a half-unit correction to already continuous intervals.

$$
\boxed{\text{Class width}=\text{upper boundary}-\text{lower boundary}}
$$

$$
\boxed{\text{Class midpoint}=\frac{\text{lower boundary}+\text{upper boundary}}{2}}
$$

For the interval $40\le x<50$, width is 10 and midpoint is 45.

**What is lost?** We no longer know each student's exact mark inside the interval. Treating all 80 students in the first class as having 45 marks gives a **grouped-data approximation**, not necessarily the exact raw-data mean.

This distinction will stay in all three mean-calculation methods. They give the same answer for the same representative values; they cannot recover information lost through grouping.

**Memory:** **Ungrouped preserves values. Grouped compresses into intervals. Midpoints represent, not reveal, hidden individual marks.**

**Try it yourself**

1. What are the width and midpoint of 60 ≤ x < 70?
2. Does a midpoint mean of 68.4 prove the exact raw mean is 68.4?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Width = 70 − 60 = 10. Midpoint = (60 + 70)/2 = 65.

2. No. It is the mean under the midpoint approximation unless actual within-class values or totals are known.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="central-tendency"></a>
### 3.2 Measures of central tendency — Why do we need one number?

Let’s continue our **school marks story**.

Suppose the Mathematics marks of 10 students are:

```text
55, 60, 65, 68, 70, 72, 75, 78, 82, 85
```

The principal looks at the list and asks:

> “Can you give me **one number** that roughly represents how this class performed?”

That question creates the need for **Measures of Central Tendency**.

> **A measure of central tendency is a value that represents the center or typical value of a dataset.**

It performs a kind of compression:

```text
Many values → One representative value
```

For this class, the total is 710 and the mean is 71. But a single number cannot preserve every feature of the class.

**The new problem: what exactly counts as the center?**

For `40, 60, 70, 70, 80`, we could ask three different questions:

> “If all marks were distributed equally, what would each student get?” → **Mean**

> “What mark is in the middle of the ordered students?” → **Median**

> “Which mark appears most often?” → **Mode**

```text
                 CENTRAL TENDENCY
                        │
          ┌─────────────┼─────────────┐
          ↓             ↓             ↓
        Mean          Median         Mode
     Equal share     Middle value   Most common
```

These are not three interchangeable calculation shortcuts. They define center differently.

**Formula?** Each measure has its own rule. There is no single formula called central tendency.

**Memory:** **Mean → equal share. Median → middle. Mode → most common.**

**Try it yourself**

1. Can two classes share a mean while having very different marks?
2. Why is reporting one center a compression rather than a complete description?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Yes. For example, 68,69,70,71,72 and 40,55,70,85,100 both average 70 but have very different spread.

2. Different datasets can produce the same center. The summary discards information about variation, shape, and individual observations.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="mean-family"></a>
### 3.3 The mean family — What exactly are we averaging?

When we initially said **Mean**, we were studying the **Arithmetic Mean**. Later the principal encounters weights, group totals, compound change, and travel rates.

> **Different real-world processes combine values differently, so one averaging method cannot correctly represent all of them.**

```text
Marks pooled into a total       → Arithmetic Mean
Unequal contributions           → Weighted Arithmetic Mean
Group averages + group sizes    → Combined Mean
Repeated multiplicative changes → Geometric Mean
Rates over equal distances      → Harmonic Mean
```

The choice is not made by spotting the word “average.” First identify the total, the process, and the quantity that must be preserved.

[Back to the topic index](#clickable-topic-index)


<a id="arithmetic-mean"></a>
#### 3.3.1 Arithmetic Mean — The equal-share and balance-point story

Suppose 5 students scored:

```text
A → 40
B → 50
C → 60
D → 70
E → 80
```

The principal asks:

> “If I want just one number to represent the overall performance of these 5 students, what should I use?”

We need a number that uses **all the marks**, not just one student.

**Pool the marks, then share equally**

$$
40+50+60+70+80=300\text{ marks}.
$$

Imagine redistributing the same 300 marks equally:

$$
300\div5=60.
$$

Everyone would then have `60, 60, 60, 60, 60`. That **60** is the mean.

> **Mean tells us what each value would be if the total were shared equally.**

```text
Before equal sharing             After equal sharing
A  ████      40                   A  ██████  60
B  █████     50                   B  ██████  60
C  ██████    60                   C  ██████  60
D  ███████   70                   D  ██████  60
E  ████████  80                   E  ██████  60
```

**The total did not change.** $5\times60=300$. The mean is the equal-share point that preserves the total.

**Formula and every symbol**

$$
\boxed{\bar{x}=\frac{\sum_{i=1}^{n}x_i}{n}}
$$

$\bar{x}$ is the arithmetic mean of these observations; $x_i$ is observation $i$; $n$ is the count; $\sum$ means add. For a whole population, use $\mu$ and $N$.

> **Mean = Total ÷ How many.**

The arithmetic mean is an additive average: it preserves the total through equal sharing. Geometric and harmonic means preserve different structures.

**Why is that useful?**

Compare two classes:

```text
Class A → 40, 50, 60, 70, 80
Class B → 55, 58, 60, 62, 65
```

Both total 300 and average 60. Their average marks are the same, but their consistency differs. This will later create the need for dispersion.

**One beautiful property — balance**

Deviations from 60 are:

```text
40 → −20
50 → −10
60 →   0
70 → +10
80 → +20
```

$$
-20-10+0+10+20=0.
$$

This always happens for deviations from the arithmetic mean:

$$
\boxed{\sum_{i=1}^{n}(x_i-\bar{x})=0}.
$$

The negative and positive deviations balance. The mean is therefore also a **balance point**.

**Cross-question:** Must someone actually score the mean? No. For `50, 60, 60, 60, 100`, the mean is 66, even though nobody scored 66. It is an equal-share summary, not a requirement that one observed score equal it.

**Memory:** **Pool everything → share equally → mean.**

**Try it yourself**

1. One more student scores 100. What is the new mean of 40,50,60,70,80,100?
2. If the five-student mean is 60, what is the total? Why?

<details>
<summary>Answers and explanations — open after trying</summary>

1. The total is 400, with 6 students. Mean = 400/6 ≈ 66.67 marks.

2. 5 × 60 = 300. Rearranging mean = total/count gives total = count × mean.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="direct-mean"></a>
##### 3.3.1.1 Direct / simple method — Use the values as they are

**The problem:** A frequency table lists repeated values only once. We need to count their full contribution to the total.

The **direct method** is the ordinary arithmetic-mean calculation. “Simple method” for raw observations is not a different kind of mean.

$$
\boxed{\bar{x}=\frac{\sum f_ix_i}{\sum f_i}}
$$

$x_i$ is the value, $f_i$ its frequency, $f_ix_i$ its contribution to the total, and $\sum f_i$ the total number of observations. For grouped classes, $x_i$ is the representative midpoint.

**Exact ungrouped example**

| Mark | Frequency | $f_ix_i$ |
|---|---:|---:|
| 60 | 2 | 120 |
| 70 | 5 | 350 |
| 80 | 3 | 240 |
| **Total** | **10** | **710** |

$$
\bar{x}=710/10=71.
$$

Frequency acts as a weight: 70 is counted five times, not just once.

**Our 1,000-student grouped example**

| Midpoint $x_i$ | Frequency $f_i$ | $f_ix_i$ |
|---:|---:|---:|
| 45 | 80 | 3,600 |
| 55 | 180 | 9,900 |
| 65 | 300 | 19,500 |
| 75 | 250 | 18,750 |
| 85 | 140 | 11,900 |
| 95 | 50 | 4,750 |
| **Total** | **1,000** | **68,400** |

$$
\boxed{\bar{x}_{\text{grouped}}=68,400/1,000=68.4}.
$$

**What new problem occurs?** Repeatedly multiplying large actual values can be inconvenient by hand. Can we calculate with smaller numbers and recover the same answer? That motivates the assumed mean method.

**Memory:** **Direct = multiply actual representative values by their frequencies, add, divide.**

**Try it yourself**

1. Why is (60 + 70 + 80)/3 not the frequency mean in the first table?
2. What is exact and what is approximate about 68.4 in the grouped table?

<details>
<summary>Answers and explanations — open after trying</summary>

1. It treats the three distinct marks as equally frequent. The observed students give weights 2,5,3, producing 71, not 70.

2. It is the exact weighted mean of the chosen midpoints. It is an approximation to the unknown raw-student mean.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="assumed-mean"></a>
##### 3.3.1.2 Assumed mean method — Use a nearby starting point

The teacher looks at values such as:

```text
525, 535, 545, 555, 565, 575
```

These are a separate large-value arithmetic illustration, not marks out of 100. They cluster near 550.

**The problem:** Why repeatedly calculate using all the large digits when the deviations are small?

Choose a convenient starting point, called the **assumed mean**, $A=550$.

```text
525 → −25
535 → −15
545 →  −5
555 →  +5
565 → +15
575 → +25
```

> **The assumed mean method calculates the arithmetic mean using deviations from a convenient reference value.**

“Assumed” does not mean we believe $A$ is the true mean. It is a calculation reference, and the average deviation supplies the correction.

$$
\boxed{d_i=x_i-A},\qquad
\boxed{\bar{x}=A+\frac{\sum f_id_i}{\sum f_i}}.
$$

$A$ is the chosen reference; $d_i$ is deviation from it; $f_i$ is frequency. For raw data, each frequency is 1.

> **Actual Mean = Assumed Mean + Correction.**

**Use the same grouped table as before**

Choose $A=65$.

| $x_i$ | $f_i$ | $d_i=x_i-65$ | $f_id_i$ |
|---:|---:|---:|---:|
| 45 | 80 | −20 | −1,600 |
| 55 | 180 | −10 | −1,800 |
| 65 | 300 | 0 | 0 |
| 75 | 250 | 10 | 2,500 |
| 85 | 140 | 20 | 2,800 |
| 95 | 50 | 30 | 1,500 |
| **Total** | **1,000** | | **3,400** |

$$
\bar{x}=65+3,400/1,000=65+3.4=68.4.
$$

Same answer, easier intermediate numbers.

**Why does the formula work?** Since $x_i=A+d_i$,

$$
\frac{\sum f_ix_i}{\sum f_i}
=\frac{A\sum f_i+\sum f_id_i}{\sum f_i}
=A+\frac{\sum f_id_i}{\sum f_i}.
$$

**Our programmer analogy:** Replacing `10020,10030,10040,10050,10060` by offsets `−20,−10,0,10,20` around 10040 changes the representation, not the information.

**Cross-question:** Must $A$ be an observed value? No. Any convenient finite reference works. A value near the center usually makes arithmetic easier.

**Memory:** **Start nearby, calculate the average correction, add it back.**

**Try it yourself**

1. For values 68,69,70,71,72, choose A = 60. What correction do you obtain?
2. Will choosing A = 70 instead of A = 65 change the grouped mean?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Deviations are 8,9,10,11,12; their mean is 10. Therefore mean = 60 + 10 = 70.

2. No. The average deviation becomes −1.6, so 70 − 1.6 = 68.4.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="step-deviation"></a>
##### 3.3.1.3 Step-deviation method — Shrink the offsets, then restore them

Our deviations from 65 are:

```text
−20, −10, 0, +10, +20, +30
```

**The next problem:** They share a common step of 10. Why not calculate with `−2,−1,0,1,2,3` instead?

> **The step-deviation method finds the same arithmetic mean after shifting by an assumed mean and scaling the deviations by a convenient nonzero factor.**

$$
\boxed{u_i=\frac{x_i-A}{h}},\qquad
\boxed{\bar{x}=A+h\frac{\sum f_iu_i}{\sum f_i}}.
$$

$u_i$ is the scaled deviation; $A$ is the assumed mean; $h$ is a nonzero common scale factor, often the common class width; $f_i$ is frequency.

Using the same grouped dataset, $A=65$, $h=10$:

| Midpoint | Frequency | $u_i$ | $f_iu_i$ |
|---:|---:|---:|---:|
| 45 | 80 | −2 | −160 |
| 55 | 180 | −1 | −180 |
| 65 | 300 | 0 | 0 |
| 75 | 250 | 1 | 250 |
| 85 | 140 | 2 | 280 |
| 95 | 50 | 3 | 150 |
| **Total** | **1,000** | | **340** |

$$
\bar{x}=65+10\left(\frac{340}{1,000}\right)=68.4.
$$

**Why multiply by $h$ again?** We divided deviations by $h$ to simplify them. The average scaled deviation, 0.34, represents 3.4 marks, not 0.34 marks. Multiply by 10 to restore the original unit.

```text
Original values      → 45,55,65,75,85,95
Subtract 65          → −20,−10,0,10,20,30
Divide deviations 10 → −2,−1,0,1,2,3
Average with weights → 0.34
Restore ×10          → 3.4
Restore +65          → 68.4
```

Equal class widths make integer step deviations convenient. The algebra itself works with any common nonzero $h$; do not claim it becomes mathematically invalid whenever intervals differ.

**Memory:** **Shift → shrink → average → unshrink → unshift.** All three routes give the same mean from the same input representation.

**Try it yourself**

1. The mean of u is 0.34, A = 65, h = 10. What is the original mean?
2. Why is 65 + 0.34 wrong?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 65 + 10 × 0.34 = 68.4.

2. 0.34 is measured in scaled steps. You must multiply by the step size 10 before adding the original reference value.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="weighted-mean"></a>
##### 3.3.1.4 Weighted Mean — Some values get more votes

So far, whenever we calculated an ordinary arithmetic mean, we assumed:

> **Every observation contributes equally.**

But the school calculates a final grade from unequal assessment weights:

| Assessment | Score out of 100 | Weight |
|---|---:|---:|
| Assignment | 80 | 20% |
| Midterm | 70 | 30% |
| Final Exam | 90 | 50% |

**The problem:** $(80+70+90)/3=80$ gives each assessment one-third of the influence. That does not match the stated grading rule.

> **Weighted Mean is an average where observations can have different amounts of influence, represented by weights.**

A weight can represent importance, frequency, credit load, amount, or group size; it is not always a subjective importance score.

$$
\boxed{\bar{x}_w=\frac{\sum w_ix_i}{\sum w_i}}.
$$

$x_i$ is each value; $w_i$ its weight; $\bar{x}_w$ the weighted arithmetic mean. Use nonnegative weights with a positive total for the ordinary averaging interpretation.

**Calculate the final grade**

$$
\bar{x}_w=\frac{80(20)+70(30)+90(50)}{20+30+50}
=\frac{1600+2100+4500}{100}=82.
$$

The weighted mean is higher than 80 because the highest score, 90, receives the greatest weight.

```text
Assignment → 20 votes for 80
Midterm    → 30 votes for 70
Final exam → 50 votes for 90
```

> **Arithmetic Mean: everyone gets one vote.**  
> **Weighted Mean: some values get more votes than others.**

**Do weights need to be percentages?** No. Weights `2,3,5`, `20,30,50`, and `0.2,0.3,0.5` have the same ratios. Multiplying all weights by the same positive number leaves the mean unchanged.

If the weights sum to 1:

$$
\bar{x}_w=\sum w_ix_i=80(0.2)+70(0.3)+90(0.5)=82.
$$

**The separate subject-weight example**

Maths = 80 with weight 50%, Science = 70 with weight 30%, English = 90 with weight 20% gives **79**, not 82. The score-weight pairings matter. This is a different setup from the assessment table above.

**More examples from our discussion**

- **Course credits:** Scores 90,80,70 with credits 4,2,1 give $(360+160+70)/7=84.29$. This is a credit-weighted percentage score, not automatically a GPA; GPA would use the institution's grade-point scale.
- **Frequency:** Scores 60,70,80 occurring 2,5,3 times give 71. Frequencies are weights.
- **Teacher evaluation:** Scores 90,70,80,100 weighted 30%,40%,20%,10% give $27+28+16+10=81$.
- **Hypothetical allocation arithmetic:** 80% of an unchanged portfolio earns 10% over one period and 20% earns 20%. With no intervening flows or fees, total return is $0.8(10\%)+0.2(20\%)=12\%$, not 15%.

**Cross-question:** What if assessments have different maximum scores? First put them on the intended comparable scale, such as percentages, unless the rule explicitly weights raw points. Do not average 8/10 and 80/100 as raw values 8 and 80 with equal importance.

**Memory:** **Unequal influence → attach weights. Equal weights → ordinary arithmetic mean.**

**Try it yourself**

1. Scores are 60 and 90, weighted 1 and 2. Find the weighted mean.
2. Will replacing weights 20,30,50 with 2,3,5 alter the final grade?

<details>
<summary>Answers and explanations — open after trying</summary>

1. (60 × 1 + 90 × 2)/(1 + 2) = 240/3 = 80.

2. No. All weights have been divided by the same positive constant, so their relative influence is unchanged.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="combined-mean"></a>
###### 3.3.1.4.1 Combined Mean — Group size becomes the weight

The principal receives two reports:

```text
Class A → 30 students → Mean = 70
Class B → 70 students → Mean = 80
```

He asks:

> “What is the average mark of all 100 students together?”

Someone calculates $(70+80)/2=75$. But that gives each **class** equal weight, not each **student**.

> **Combined Mean finds the mean of several groups when we know each group's size and mean.**

**The whole trick: recover totals**

Since mean = total/count:

$$
\boxed{\text{Group total}=n_i\bar{x}_i}.
$$

Class A total is $30\times70=2,100$. Class B total is $70\times80=5,600$.

$$
\bar{x}_c=\frac{2100+5600}{30+70}=\frac{7700}{100}=77.
$$

$$
\boxed{\bar{x}_c=\frac{\sum_{i=1}^{k}n_i\bar{x}_i}{\sum_{i=1}^{k}n_i}}.
$$

$\bar{x}_c$ is combined mean; $n_i$ is group $i$'s size; $\bar{x}_i$ is its mean; $k$ is the number of groups.

> **Combined Mean = Weighted Mean where group size is the weight.**

**Why was it needed?** The principal does not need every mark again. Exact group sizes and means contain enough information to recover the overall total. If the reported means are rounded, the reconstructed total and mean inherit that approximation. Groups must also not unintentionally double-count the same observations.

**Three-class example**

| Class | Students | Mean | Implied total |
|---|---:|---:|---:|
| A | 20 | 60 | 1,200 |
| B | 30 | 70 | 2,100 |
| C | 50 | 80 | 4,000 |

Combined mean = $7,300/100=73$, not $(60+70+80)/3=70$.

**Other examples from the discussion**

Campuses of 500 students averaging 72 and 1,500 averaging 78 combine to:

$$
\frac{500(72)+1500(78)}{2000}=76.5.
$$

Year groups of 120 averaging 74 and 180 averaging 79 combine to:

$$
\frac{120(74)+180(79)}{300}=77.
$$

These are averages across the recorded observations, not automatically a measure of year-to-year progress for the same students.

**Reverse question — a missing group mean**

Class A: 40 students, mean 70. Class B: 60 students, unknown mean. Combined mean: 76.

```text
Combined total = 100 × 76 = 7,600
Class A total  = 40 × 70  = 2,800
Class B total  = 7,600 − 2,800 = 4,800
Class B mean   = 4,800 / 60 = 80
```

**Can we ever average means directly?** Yes, equal group sizes make the simple average valid. With unequal sizes it may coincide accidentally, for example when group means are identical, but it is not a reliable general method.

**Memory:** **Mean × size → total; combine totals; divide by combined size.**

**Try it yourself**

1. Class A has 10 students averaging 50; B has 30 averaging 70. Find the combined mean.
2. Why does the combined mean lie closer to the larger group’s mean?

<details>
<summary>Answers and explanations — open after trying</summary>

1. (10 × 50 + 30 × 70)/40 = 2600/40 = 65.

2. Each student has equal weight, so the larger group contributes more observations and therefore more influence.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="geometric-mean"></a>
#### 3.3.2 Geometric Mean — Preserve the multiplied result

The school tracks the number of students using its online learning platform.

```text
Start → 100
       ↓ +10%
       110
       ↓ −10%
        99
```

**What problem occurred?** The arithmetic mean of percentage changes is $(10\%-10\%)/2=0\%$. But the platform ends with 99 users, not 100.

The arithmetic calculation is an average of the two listed percentages. It is not the constant **compound growth rate** producing the same endpoint, because the percentages act on different starting amounts.

$$
100\times1.10\times0.90=99.
$$

The process multiplies. So the principal asks:

> “What single multiplier, applied each period, would produce the same final result?”

> **The Geometric Mean of positive values is the equal repeated factor that preserves their product.**

$$
\boxed{GM=\left(\prod_{i=1}^{n}x_i\right)^{1/n}
=\sqrt[n]{x_1x_2\cdots x_n}}.
$$

$x_i$ are positive values; $n$ is their count; $\prod$ (capital Pi/product symbol) means multiply, just as $\sum$ means add; $\sqrt[n]{\ }$ means take the $n$th root.

**Calculate the growth example**

$$
GM=\sqrt{1.10\times0.90}=\sqrt{0.99}\approx0.994987.
$$

That is a **growth factor**, not a percentage. Subtract 1:

$$
\boxed{g=GM-1\approx-0.005013=-0.5013\%\text{ per year}}.
$$

Check:

$$
100(0.994987)^2\approx99.
$$

**General compound-growth formula**

If $g_i$ are rates written as decimals for equal-length periods:

$$
\boxed{g_{\mathrm{equiv}}=\left(\prod_{i=1}^{n}(1+g_i)\right)^{1/n}-1}.
$$

If the initial and final positive amounts are $V_0,V_n$ over $n$ equal periods:

$$
\boxed{g_{\mathrm{equiv}}=(V_n/V_0)^{1/n}-1}.
$$

**Why “geometric”?** For two positive lengths $a,b$, a rectangle has area $ab$. A square of the same area has side $\sqrt{ab}$, the geometric mean. This is the geometric interpretation discussed earlier, rather than a needed historical derivation.

**Cross-question:** Should we multiply raw percentages 10 and −10? No. For compound growth, use **factors** 1.10 and 0.90. A negative growth rate can be fine if its factor remains positive. The usual positive-data geometric-mean formulas and log interpretation do not apply indiscriminately to zero or negative observations.

The same multiplication idea applies to sequential discounts: 10%,20%,30% discounts retain factors 0.9,0.8,0.7. The retained total is 0.504; the total discount is 49.6%, not 60%. This is an application of the compounding idea, not a separate kind of mean.

**Memory:** **Arithmetic preserves the sum. Geometric preserves the product.**

**Try it yourself**

1. The platform doubles one year and halves the next. What is the equivalent annual growth rate?
2. Why can +10% followed by −10% produce a loss?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Factors are 2 and 0.5. Their product is 1. GM = √1 = 1, so equivalent growth is 0% per period.

2. The 10% decrease is taken from 110, not 100. The product 1.1 × 0.9 = 0.99 leaves 99% of the original amount.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="harmonic-mean"></a>
#### 3.3.3 Harmonic Mean — Equal-distance rate problems

The school bus travels **10 km at 60 km/h**, then **10 km at 40 km/h**.

The principal asks:

> “What was the average speed?”

A tempting answer is $(60+40)/2=50$ km/h. But average speed must preserve total distance divided by total time.

**What problem occurred?** The distances are equal, not the times. The slower segment takes longer.

$$
\text{Time}=\frac{\text{distance}}{\text{speed}}.
$$

```text
10 km at 60 km/h → 10/60 hour = 10 minutes
10 km at 40 km/h → 10/40 hour = 15 minutes
```

Total distance is 20 km. Total time is $1/6+1/4=5/12$ hour.

$$
\boxed{\text{Average speed}=\frac{20}{5/12}=48\text{ km/h}}.
$$

**Why does a reciprocal appear?** For fixed distance $d$, time is $d/v$. The rate sits in a denominator. We must average the corresponding time-per-distance quantities and invert back.

> **The Harmonic Mean is the reciprocal of the arithmetic mean of the reciprocals.**

For positive values:

$$
\boxed{HM=\frac{n}{\sum_{i=1}^{n}1/x_i}}.
$$

$n$ is the number of values; $x_i$ is each positive rate or value; $1/x_i$ is its reciprocal.

For our bus:

$$
HM=\frac2{1/60+1/40}=\frac2{5/120}=48.
$$

For two positive values $a,b$:

$$
\boxed{HM=\frac{2ab}{a+b}}.
$$

**Why equal distances lead to HM**

$$
\frac{nd}{d/x_1+\cdots+d/x_n}
=\frac{n}{1/x_1+\cdots+1/x_n}.
$$

The equal distance $d$ cancels.

**The vital cross-question: Do all rate problems use HM? No.**

If the bus spends **one hour** at 60 and **one hour** at 40, total distance is 100 km and total time 2 hours. Average speed is **50 km/h**, the arithmetic mean.

```text
Equal distances → harmonic mean of speeds
Equal times     → arithmetic mean of speeds
Unequal segments → total distance / total time first
```

For distances $d_i$ and speeds $v_i$:

$$
\boxed{\bar{v}=\frac{\sum d_i}{\sum d_i/v_i}}.
$$

This is a distance-weighted harmonic mean. Here $d_i/v_i$ is segment time. For time weights $t_i$, average speed is $\sum t_iv_i/\sum t_i$.

**More applications, with the condition made explicit**

Equal numbers of words typed at different words-per-minute rates; equal file sizes downloaded at different MB/s rates; equal quantities of work performed sequentially at different rates. Always check what is held equal. Parallel workers' combined rate is a different question, not automatically an average.

**Compare the three means using 40 and 60**

$$
AM=50,\qquad GM=\sqrt{2400}\approx48.99,\qquad HM=48.
$$

For positive values:

$$
\boxed{AM\ge GM\ge HM},
$$

with equality when every value is equal.

**Memory:** **Rates do not automatically mean HM. Ask: equal what?**

**Try it yourself**

1. The bus travels 10 km at 60 and 10 km at 40. What is its average speed?
2. It instead spends 30 minutes at each speed. What changes?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 48 km/h, because total time is 25 minutes and total distance is 20 km.

2. Distances are 30 km and 20 km. Total distance 50 km over 1 hour gives 50 km/h. Equal time makes the arithmetic mean appropriate.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="numerical-median"></a>
### 3.4 Median — Why mean is not always the typical student

We already learned that Mean answers:

> “If all marks were shared equally, what mark would every student have?”

That works beautifully in many situations. But then the principal encounters a problem.

**Chapter 1: Mean seems perfect**

```text
60, 65, 70, 75, 80
```

Mean = 70. The class is balanced around 70.

**Chapter 2: Something unusual happens**

```text
0, 65, 70, 75, 80
```

Suppose a student attended little of the exam and received zero under the grading rule. The mean becomes:

$$
\bar{x}=\frac{0+65+70+75+80}{5}=58.
$$

Four out of five students scored between 65 and 80. The principal thinks:

> “58 doesn't really look like a typical student in this group.”

The mean has not calculated the wrong total. It answers the equal-share question correctly. But it may not represent a **typical position** well.

**A different idea**

> “Instead of combining everybody's marks, can I simply find the student who stands in the middle?”

```text
0    65    [70]    75    80
             ↑
           middle
```

> **Median is the middle value when observations are arranged in order.**

Here the median is 70. There are two observations below and two above.

**Formula — sort first**

Let $x_{(1)}\le x_{(2)}\le\cdots\le x_{(n)}$ be the sorted observations; parentheses indicate **ordered position**, not the original student's ID.

$$
\boxed{M=x_{((n+1)/2)}\quad\text{for odd }n}
$$

$$
\boxed{M=\frac{x_{(n/2)}+x_{(n/2+1)}}2\quad\text{for even }n}
$$

$M$ is the usual numerical median and $n$ is the number of observations.

For `50,60,65,70,75,80`, the central values are 65 and 70:

$$
M=(65+70)/2=67.5.
$$

**Why is it resistant to extremes?**

```text
10,65,70,75,80 → Median 70
 1,65,70,75,80 → Median 70
 0,65,70,75,80 → Median 70
```

As long as changing the lowest value does not change the central positions, the median stays the same. Its resistance is not a claim that nothing can ever change it.

**Cross-question:** Should a real zero be removed because the mean changes? No. An unusual observation may be valid. Choose a summary matching the question; do not discard inconvenient values automatically.

**Memory:** **Mean cares about every magnitude. Median locates the middle after sorting.**

**Try it yourself**

1. Find the median of 80,50,70,60.
2. If 80 becomes 100 in 0,65,70,75,80, what happens to mean and median?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Sort to 50,60,70,80. Median = (60 + 70)/2 = 65.

2. Mean increases from 58 to 62. Median remains 70.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="numerical-mode"></a>
### 3.5 Mode — The most frequently observed score

The principal now asks:

> “Which mark did students score most often?”

For:

```text
55, 60, 60, 65, 70, 70, 70, 75, 80
```

counts are 55:1, 60:2, 65:1, 70:3, 75:1, 80:1.

> **Mode is the value or category that occurs with the highest frequency in a dataset.**

$$
\boxed{\text{Mode}=70}.
$$

**The problem it solves:** Neither total/count nor middle position directly identifies the most frequent actual outcome.

For `40,60,60,60,100`, the mean is 64 but the most common score is 60. Nobody scoring 64 does not invalidate the mean; it simply answers a different question.

For `10,20,30,40,50,50,50`, median = 40 while mode = 50. Most frequent and middle are not interchangeable.

**Rule**

$$
\boxed{\text{Mode}=\text{value(s) having maximum frequency}}.
$$

Tied highest frequencies can give two or more modes. If all values occur equally often, there is no unique mode. For continuous measurements, exact repetitions can depend on rounding, and a distribution's modal region is not the same as the most frequent rounded number in a tiny sample.

**Cross-question:** Must mode occur in the observed raw data? An observed-value mode does. A modal class in grouped data or an estimated density peak is a different kind of representation; do not silently swap them.

**Memory:** **Mode = most common, not necessarily middle.**

**Try it yourself**

1. Find mode and median of 10,20,30,40,50,50,50.
2. Does 50,60,70,80,90 have a uniquely most frequent score?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Mode = 50, because it occurs three times. Median = the 4th value = 40.

2. No. All appear once. In the usual school convention, it has no mode; more precisely, no unique mode.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="choose-center"></a>
### 3.6 Mean vs Median vs Mode — Choose the question before the formula

Knowing how to calculate the three centers is only half the job. The principal asks:

> “Which one actually represents my data properly?”

There is no universally best measure. The choice depends on the question, the measurement scale, and the data's shape.

**Our three questions**

```text
Mean   → What is the numerical balance / equal-share value?
Median → What is the middle ordered position?
Mode   → What occurs most frequently?
```

**Balanced marks**: `60,65,70,75,80` give mean = median = 70, with no unique mode. Mean is a useful overall numerical summary.

**A low extreme**: `0,65,70,75,80` give mean = 58, median = 70. If the question is typical position, the median is more resistant. If it is total marks per student, 58 is exactly the mean you want.

**A long high tail**: `20,25,30,35,40,45,90` give mean $285/7\approx40.71$ and median 35. The high score pulls the mean upward.

**The income analogy from our discussion**

Monthly incomes of ₹30k,₹35k,₹40k,₹45k,₹500k have mean ₹130k and median ₹40k. The mean remains the correct total-per-person value, but the median describes the middle person's position more directly.

**When all three differ**

```text
10,20,30,40,50,50,100
```

$$
\bar{x}=300/7\approx42.86,\qquad M=40,\qquad\text{Mode}=50.
$$

No contradiction: different questions produce different summaries.

| Question / property | Mean | Median | Mode |
|---|---|---|---|
| Preserves total through equal sharing | Yes | Not generally | Not generally |
| Uses order | Not needed | Essential | Not needed |
| Sensitive to extreme magnitudes | Yes | Resistant | Depends on frequencies |
| Nominal labels | Not as an arbitrary-code average | No | Yes |
| Ordinal categories | Requires more than order to interpret arithmetic | Yes, with convention | Yes |
| Must equal an observed value | No | Not always | For an observed-value mode, yes |

**Why not automatically replace the mean when there is an outlier?**

A real zero belongs in the total. A high expenditure may be precisely what the principal needs to budget for. Robust typical-value questions and total-based questions are different. Sometimes reporting both mean and median is better than forcing one to stand for everything.

**What about symmetric data?**

For `50,60,70,70,70,80,90`, all three equal 70. Symmetry gives mean = median when these are defined in the usual setting, but not necessarily a unique central mode. A symmetric two-peaked distribution is a counterexample to “symmetry always makes all three equal.”

**Memory:** **Mean = balance. Median = position. Mode = frequency. Choose the question first.**

**Try it yourself**

1. The principal needs total marks divided by students even when one scored zero. Which measure?
2. For nominal club labels, why is mode meaningful while a code mean is not?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Arithmetic mean. The extreme score is part of the quantity being summarized.

2. Mode depends only on frequencies. A code mean changes when arbitrary category labels are renumbered.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="spread-position"></a>
## 4. Numerical data — Spread, position, and the five-number picture

The principal now knows the center. But **same center does not mean same class**.

Our study order is deliberately:

```text
Need spread → Range → everyone’s deviations
                    ├── absolute deviations → Mean Deviation
                    └── squared deviations → Variance → SD
Need internal landmarks → Quartiles → Percentiles → IQR → Five-number summary
Need relative comparison → Coefficient of Variation
```

Quartiles come before IQR because IQR cannot be understood until its two endpoints are understood.

[Back to the topic index](#clickable-topic-index)


<a id="dispersion"></a>
### 4.1 Measures of dispersion — Why the center is not enough

The principal thinks:

> “Great. If I know the average marks of a class, I understand how the class performed.”

Then he sees two classes:

```text
Class A: 68,69,70,71,72
Class B: 40,55,70,85,100
```

Both total 350, so both average 70. But Class A is tightly packed around 70, while Class B has much larger differences between students.

**What problem occurred?** The same center can hide very different patterns of individual performance.

> **Measures of Dispersion tell us how much the values in a dataset differ or spread out.**

```text
Center → Where is the data centered?
Spread → How far apart are the observations?
```

The principal may need a different support plan for a class where everyone is close to 70 than for one where some students score 40 and others 100. The mean alone cannot show that difference.

**Start with actual distances**

```text
Class A distance from 70 → 2,1,0,1,2
Class B distance from 70 → 30,15,0,15,30
```

Different measures summarize these patterns differently. Some use the extreme endpoints; some use all observations; others focus on the middle half.

**Formula?** Dispersion is a family of questions. Range, MD, variance, SD, IQR, and CV have different formulas because they measure different aspects of spread.

**Memory:** **Central tendency tells us where the class is. Dispersion tells us how scattered the class is.**

**Try it yourself**

1. Do the two classes have the same average?
2. Would a mean of 70 reveal how many students are far from 70?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Yes. Each total is 350, and 350/5 = 70.

2. No. A measure of spread or the actual distribution is also needed.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="range"></a>
### 4.2 Range — The first attempt, and why two endpoints are not enough

The principal thinks:

> “This seems easy. I'll look at the highest and lowest marks.”

> **Range tells us the total width covered by the data.**

$$
\boxed{R=\max(x_i)-\min(x_i)}.
$$

$R$ is the range; $\max$ selects the largest observation; $\min$ selects the smallest. The unit is the original unit, here marks.

For Class A:

$$
R_A=72-68=4.
$$

For Class B:

$$
R_B=100-40=60.
$$

Excellent: the first solution distinguishes the tightly packed class from the widely spread class.

**But Range has a serious problem**

Consider two more classes from our discussion:

```text
Class C → 40,40,70,100,100
Class D → 40,69,70,71,100
```

| Class | Mean | Range |
|---|---:|---:|
| C | 70 | 60 |
| D | 70 | 60 |

In C, four students are 30 marks from the mean. In D, three are at or within 1 mark of the mean. The range cannot distinguish this.

> **Range uses only two observations. It completely ignores everyone in between.**

It did not calculate incorrectly; it answers the total-width question and no more.

The principal now asks:

> “Why am I measuring spread using only TWO students? Can't I include EVERY student's distance from the center?”

This leads to deviations.

**Cross-question:** Can one changed minimum alter the range a lot? Yes. Changing 40 to 0 changes a 60-mark range into a 100-mark range, even if every other score is unchanged.

**Memory:** **Range = edge to edge; not the internal arrangement.**

**Try it yourself**

1. Find the range of 55,60,70,75,90.
2. If the minimum and maximum stay fixed while all middle scores change, does the range change?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 90 − 55 = 35 marks.

2. No. That is why range cannot describe all aspects of spread.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="mean-deviation"></a>
### 4.3 Signed deviations and Mean Absolute Deviation — Keep distance, ignore direction

Before choosing a complicated formula, the principal asks a natural question:

> “Why can't I simply calculate how far each student is from the average, and then average those distances?”

For `68,69,70,71,72`, the mean is 70.

| Mark $x_i$ | Signed deviation $x_i-70$ | Absolute distance $\lvert x_i-70\rvert$ |
|---:|---:|---:|
| 68 | −2 | 2 |
| 69 | −1 | 1 |
| 70 | 0 | 0 |
| 71 | 1 | 1 |
| 72 | 2 | 2 |

**What goes wrong with signed deviations?**

$$
-2-1+0+1+2=0.
$$

This is always true around the arithmetic mean:

$$
\sum(x_i-\bar{x})=0.
$$

The mean signed deviation is zero because negative and positive directions balance. That does **not** mean the average distance is zero.

**The rescue: absolute values**

> “I don't care whether a student is below or above the mean. I only want to know how far away the student is.”

Absolute value measures magnitude without direction: $|-5|=5$ and $|5|=5$.

> **Mean Deviation measures the average absolute distance of observations from a chosen central value.**

$$
\boxed{MD_A=\frac1n\sum_{i=1}^{n}|x_i-A|}.
$$

$A$ is the chosen center, not necessarily an assumed-mean shortcut; $x_i$ is observation $i$; $n$ is the count; vertical bars mean absolute value.

About the mean:

$$
\boxed{MD_{\bar{x}}=\frac{\sum|x_i-\bar{x}|}{n}}.
$$

For our class:

$$
MD_{\bar{x}}=\frac{2+1+0+1+2}{5}=1.2\text{ marks}.
$$

**What does 1.2 actually mean?**

> Students are, on average, 1.2 marks away from the class mean of 70, ignoring direction.

**Compare two classes with the same mean**

```text
Class A: 68,69,70,71,72 → distances 2,1,0,1,2 → MD 1.2
Class B: 50,60,70,80,90 → distances 20,10,0,10,20 → MD 12
```

The second class has ten times the average absolute distance, despite the same center.

**About the median and with frequencies**

If $M$ is the median:

$$
MD_M=\frac{\sum|x_i-M|}{n}.
$$

With frequencies:

$$
\boxed{MD_A=\frac{\sum f_i|x_i-A|}{\sum f_i}}.
$$

For 60,70,80 with frequencies 2,5,3, the mean is 71:

$$
MD_{71}=\frac{2(11)+5(1)+3(9)}{10}=5.4.
$$

About the median 70, it is $(20+0+30)/10=5$. The median minimizes the sum of absolute deviations; the mean minimizes the sum of squared deviations. These are different optimization questions.

**Why also learn variance?** There are two responses to cancellation:

```text
Take absolute values → average ordinary distances → MD
Square deviations    → average squared distances → Variance
```

Variance gives larger deviations more emphasis and has useful algebraic properties. MD is intuitive, but not a universal replacement for it.

**Notation clarification:** Our chat used **MAD** for mean absolute deviation. Other books use MAD for **median absolute deviation**, namely $\operatorname{median}(|x_i-M|)$. They are different quantities. This notebook uses **MD** for the mean of absolute distances to avoid ambiguity. [See notation check: S1.](#reference-s1)

**Memory:** **Signed deviation tells direction. Absolute deviation tells distance.**

**Try it yourself**

1. Compute MD about the mean for 50,60,70,80,90.
2. Why is a zero sum of signed deviations not proof of zero spread?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Mean = 70. Absolute distances total 20+10+0+10+20 = 60. MD = 60/5 = 12 marks.

2. Positive and negative deviations cancel. Zero spread would require every distance to be zero, so every observation equals the center.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="variance"></a>
### 4.4 Variance — Average the squared distances

The principal now knows that averaging signed deviations gives zero even when students are spread out. Mean Deviation used absolute values. Another mathematical response is to **square** each deviation.

$$
(-30)^2=900,\qquad(+30)^2=900.
$$

Both sides now contribute positively. Large deviations also receive extra emphasis.

> **Variance measures the average squared distance of observations from their mean.**

This exact “average” definition applies to the population/empirical form. The sample estimator with $n-1$ is introduced separately below.

**Population formula**

$$
\boxed{\sigma^2=\frac{\sum_{i=1}^{N}(x_i-\mu)^2}{N}}.
$$

$\sigma^2$ is population variance; $\mu$ is population mean; $N$ is population size; $x_i$ is an individual observation; $\sum$ means add; the exponent 2 means square.

**Return to the two classes that defeated Range**

Both C and D have mean 70 and range 60.

| Class C marks | Deviation | Squared deviation |
|---:|---:|---:|
| 40 | −30 | 900 |
| 40 | −30 | 900 |
| 70 | 0 | 0 |
| 100 | 30 | 900 |
| 100 | 30 | 900 |
| **Total** | **0** | **3,600** |

Treating each five-student class as the complete population:

$$
\sigma_C^2=3600/5=720\text{ marks}^2.
$$

| Class D marks | Deviation | Squared deviation |
|---:|---:|---:|
| 40 | −30 | 900 |
| 69 | −1 | 1 |
| 70 | 0 | 0 |
| 71 | 1 | 1 |
| 100 | 30 | 900 |
| **Total** | **0** | **1,802** |

$$
\sigma_D^2=1802/5=360.4\text{ marks}^2.
$$

Finally we can distinguish them. C has more spread **as measured by average squared distance from the mean**.

**A smaller example for learning the calculation**

For `68,69,70,71,72`, deviations are `−2,−1,0,1,2`; squares are `4,1,0,1,4`.

$$
\sigma^2=10/5=2\text{ marks}^2.
$$

**Why square instead of merely dropping signs?** Squaring does more than prevent cancellation:

```text
Distance 2  → square 4
Distance 5  → square 25
Distance 20 → square 400
```

That is useful when large deviations should matter strongly, but it also makes variance sensitive to extreme values. It is an alternative measure, not proof that MD was wrong.

For a complete frequency distribution:

$$
\boxed{\sigma^2=\frac{\sum f_i(x_i-\mu)^2}{\sum f_i}}.
$$

Use class midpoints only as a grouped approximation when exact within-class values are unknown.

**The next problem:** Students score in marks, not square marks. How should the principal interpret $720\text{ marks}^2$? That creates the need for Standard Deviation.

**Memory:** **Deviation → square → average = variance.**

**Try it yourself**

1. What is population variance for 68,69,70,71,72?
2. Why can variance distinguish classes that share the same range?

<details>
<summary>Answers and explanations — open after trying</summary>

1. The mean is 70. Squared deviations total 10. Divide by 5 to get 2 marks².

2. It uses the distance of every observation from the mean, including the observations between the endpoints.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="standard-deviation"></a>
### 4.5 Standard Deviation — Bring spread back to the original unit

The principal asks:

> “What does 720 marks² mean to me? Students don't score in square marks.”

**The problem:** Variance is useful mathematically, but its squared unit is awkward to interpret directly.

> **Standard deviation is the square root of variance. It describes the scale of spread around the mean in the original unit.**

For a population:

$$
\boxed{\sigma=\sqrt{\frac{\sum_{i=1}^{N}(x_i-\mu)^2}{N}}=\sqrt{\sigma^2}}.
$$

$\sigma$ is lowercase sigma, population SD; $\mu$ is population mean; $N$ is size; $x_i$ is each observation; $\sqrt{\ }$ means square root. Do not confuse $\sigma$ with $\sum$.

For the tightly packed marks `68,69,70,71,72`:

$$
\sigma=\sqrt2\approx1.414\text{ marks}.
$$

For our comparison classes:

$$
\sigma_C=\sqrt{720}\approx26.83\text{ marks},
\qquad
\sigma_D=\sqrt{360.4}\approx18.98\text{ marks}.
$$

**What exactly does it tell us?**

> Standard deviation tells us the typical scale of distance between observations and the mean.

More precisely, population SD is the **root mean square** of deviations. It is **not** the arithmetic mean of absolute distances; that was MD. In the small example, MD = 1.2 but SD ≈ 1.414.

```text
Small SD → values tend to be close to the mean
Large SD → greater root-mean-square distance from the mean
```

It does not say every student is exactly one SD away. It does not, without distributional assumptions, say a fixed percentage must lie within one SD.

**Why keep variance too?** Variance has useful algebra. Later we will see that variances of independent sums add, whereas SDs do not simply add. SD is easier to report in marks, centimetres, or hours. The two serve related but different purposes.

**Unit-change example**

Multiplying all values by a positive factor $a$ multiplies SD by $a$ and variance by $a^2$. Adding a constant changes neither spread measure.

$$
\operatorname{Var}(aX+b)=a^2\operatorname{Var}(X),
\quad SD(aX+b)=|a|SD(X).
$$

$a$ is a scale multiplier and $b$ an added constant. This is a useful bridge to CV and correlation, not an assumption that all unit conversions are simple multiplication.

**Memory:** **Variance → square units. Square root → SD → original units.**

**Try it yourself**

1. Population variance is 36 marks². What is SD?
2. Every student receives 5 extra marks. What happens to SD?

<details>
<summary>Answers and explanations — open after trying</summary>

1. √36 = 6 marks.

2. Nothing, provided the marks are simply shifted without clipping at a maximum. Every deviation from the new mean is unchanged.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="sample-variance-sd"></a>
### 4.6 Sample variance and SD — Why two denominators appear

> **Coverage:** Introduced / preview; not a full advanced treatment.

So far we treated the five students as the complete class of interest. Now the principal wants to estimate variability in a much larger school from those five students.

**The problem:** A sample's own fitted mean is especially close to that sample. Squared distances from it tend to underestimate the population variance if we simply divide by $n$ and use the result as an unbiased variance estimator.

**The formulas introduced in our discussion**

$$
\boxed{s^2=\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}},
\qquad
\boxed{s=\sqrt{\frac{\sum_{i=1}^{n}(x_i-\bar{x})^2}{n-1}}}.
$$

$s^2$ is the usual sample variance estimator; $s$ is sample SD; $\bar{x}$ is sample mean; $n$ is sample size, at least 2.

For `68,69,70,71,72`, the squared deviations total 10:

```text
Empirical/population-form variance = 10/5 = 2
Usual sample variance estimator    = 10/4 = 2.5
Sample SD                         = √2.5 ≈ 1.581
```

**A brief intuition for $n-1$**

Once the sample mean is fixed, deviations must add to zero. Knowing $n-1$ deviations determines the last. This is the degrees-of-freedom intuition.

Under independent, identically distributed sampling with finite variance, dividing by $n-1$ makes $s^2$ unbiased for the population variance. Taking its square root does **not** automatically make $s$ unbiased for population SD.

**Important distinction:** Dividing by $n$ is not always “wrong because these are sample data.” It gives the empirical mean squared deviation of the observed sample. Dividing by $n-1$ is the standard correction when estimating the population variance under the stated sampling setup.

**Status:** We introduced these formulas and the motivation. A full derivation of bias, degrees of freedom, and sampling distributions remains pending, just as in our conversation.

**Memory:** **Describe the observed squared distances → divide by count. Usual unbiased population-variance estimate → use $n-1$.**

**Try it yourself**

1. The sum of squared deviations is 40 for n = 5. Find sample variance and sample SD.
2. Does dividing by n−1 guarantee that sample SD is unbiased?

<details>
<summary>Answers and explanations — open after trying</summary>

1. s² = 40/4 = 10. s = √10 ≈ 3.162, in the original unit.

2. No. The correction makes the variance estimator unbiased under its assumptions. Square roots do not preserve unbiasedness.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="quartiles"></a>
### 4.7 Quartiles — Why median alone is not enough

The principal knows the median but asks:

> “Where does the bottom quarter of the class end? At what score does the top quarter begin?”

**The problem:** The median supplies one middle landmark. We need more cut-points across the ordered observations.

> **Quartiles are positional cut-points associated with the 25%, 50%, and 75% levels of ordered data.**

```text
Lowest         25%           50%           75%        Highest
   |------------|-------------|-------------|------------|
               Q1            Q2            Q3
                             ↑
                           Median
```

This is a schematic of proportions, not a claim that the numerical gaps between quartiles are equal. With ties and small samples, equal quarters need not translate into exactly equal counts strictly between cut-points.

$$
\boxed{Q_1=P_{25},\qquad Q_2=P_{50}=M,\qquad Q_3=P_{75}}.
$$

$Q_1,Q_2,Q_3$ are the quartiles; $P_k$ is the $k$th percentile; $M$ is median.

**Use the same 20 students from our chat**

```text
35,40,44,48,50,54,58,60,62,65,
68,70,72,74,76,78,82,86,90,95
```

The 10th and 11th values are 65 and 68:

$$
Q_2=(65+68)/2=66.5.
$$

Lower half:

```text
35,40,44,48,50,54,58,60,62,65
```

Its middle two values are 50 and 54:

$$
Q_1=(50+54)/2=52.
$$

Upper half:

```text
68,70,72,74,76,78,82,86,90,95
```

Its middle two values are 76 and 78:

$$
Q_3=(76+78)/2=77.
$$

$$
\boxed{Q_1=52,\quad Q_2=66.5,\quad Q_3=77}.
$$

Now the principal can describe the lower-quarter boundary, the middle of the class, and the upper-quarter boundary rather than only reporting the median.

**Why might calculators disagree?** Sample quartiles have several accepted conventions. The calculations above retain our original median-of-halves result for these 20 observations. For a consistent rule that also computes other percentiles, the next section states a sample-quantile convention giving these same answers here. Other sample sizes and conventions can differ. [Convention check: S2.](#reference-s2)

**Cross-question:** Must a quartile be one student's exact score? No. Here 52,66.5,77 are interpolated midpoints between observations, not scores someone necessarily earned.

**Memory:** **Median gives one landmark. Quartiles give three.**

**Try it yourself**

1. For the 20-student list, what are Q1, Q2, and Q3?
2. Do the four quartile sections have equal mark widths?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Q1 = 52, Q2 = 66.5, Q3 = 77 using the stated calculation.

2. No. They target equal portions of the ordered observations, not equal intervals of marks.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="percentiles"></a>
### 4.8 Percentiles — Finer landmarks, not percentage marks

The principal now asks:

> “What if I want to know whether a student is in the top 10%?”

Quartiles give only 25%,50%,75% landmarks. We need a finer positional scale.

> **Percentiles are cut-points describing location in an ordered distribution on a percentage scale.**

A percentile **value** answers “What score is the 90th percentile?” A percentile **rank** answers “Where does this student's score stand relative to the group?” These are related but not identical questions in a finite dataset.

**What does “90th percentile” mean?**

Roughly, it is a score around which 90% of observations are at or below and 10% above, subject to ties and the percentile convention.

```text
Percentage → How much of the available score did I earn?
Percentile → Where does that score sit compared with others?
```

A score of 76 out of 100 is 76%. In a difficult exam it could correspond to a high percentile. A 90th-percentile result is **not** necessarily 90 marks.

**Percentile ranks — say how ties are handled**

Let $L$ be the number strictly below score $x$, $E$ the number equal to it, and $n$ the comparison-group size.

$$
PR_{<}(x)=100\frac{L}{n},\qquad
PR_{\le}(x)=100\frac{L+E}{n}.
$$

One also encounters the midrank convention $100(L+E/2)/n$. These conventions answer slightly different questions; do not switch silently.

If Rahul is one of 100 students, 89 scored below him, 1 scored his mark (Rahul himself), and 10 scored above:

```text
Strictly-below rank → 89%
At-or-below rank   → 90%
```

That explains why careless “better than 90%” and “90% at or below” wording can disagree.

**Finding a percentile value — a declared sample convention**

For this notebook's numerical examples, use this common rule, equivalent to a stepwise empirical-quantile method with averaging at an exact jump:

1. Sort values $x_{(1)}\le\cdots\le x_{(n)}$.
2. Set $h=nk/100$, where $k$ is the desired percentile number, $0<k<100$.
3. If $h$ is not an integer, take $x_{(\lceil h\rceil)}$.
4. If $h=j$ is an integer, take $(x_{(j)}+x_{(j+1)})/2$.

Here $\lceil h\rceil$ means round the position upward. The endpoint conventions are $P_0=\min$ and $P_{100}=\max$.

For our 20 marks, $P_{90}$ uses $h=18$. The 18th and 19th values are 86 and 90:

$$
P_{90}=(86+90)/2=88.
$$

This same rule gives $P_{25}=52$, $P_{50}=66.5$, $P_{75}=77$, matching the original quartile example. It need not match every software default or every median-of-halves rule for other sample sizes. Follow an exam's stated convention. [Convention check: S2.](#reference-s2)

**The ten-student example from our discussion**

```text
32,40,45,51,58,64,70,76,84,92
```

For score 84, the strictly-below rank is 80% and the at-or-below rank is 90%. Under the percentile-value convention above, $P_{90}=(84+92)/2=88$. That is not a contradiction: rank-of-a-score and selected quantile-value rules need not be exact inverses in a finite sample.

**Comparing different exams**

82 marks at the 70th percentile and 75 marks at the 95th percentile show different **relative positions within their respective groups**. This alone does not prove one student's absolute ability is higher: different exams and comparison groups may differ.

**Memory:** **Percentage = own score. Percentile = relative position. Check the convention.**

**Try it yourself**

1. Rahul earns 76/100 and 90% of students score at or below 76. State percentage and at-or-below percentile rank.
2. Find P90 of the original 20 marks using the convention in this section.

<details>
<summary>Answers and explanations — open after trying</summary>

1. Percentage score = 76%. At-or-below percentile rank = 90. They measure different things.

2. h = 20 × 90/100 = 18, an integer. Average the 18th and 19th values: (86 + 90)/2 = 88.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="deciles-preview"></a>
#### 4.8.1 Deciles — A named extension of percentile landmarks

> **Coverage:** Introduced / preview; not a full advanced treatment.

**Status:** Deciles were included in our master tree but did not receive a separate full lesson.

**The question they answer:** What if the principal wants ten broad positional groups rather than four?

> **Deciles are the nine cut-points at the 10th,20th,...,90th percentile levels.**

$$
\boxed{D_k=P_{10k},\quad k=1,2,\ldots,9}.
$$

$D_k$ is decile $k$. In particular, $D_5=P_{50}$ is the median. Use the same declared sample-quantile convention as for percentiles.

For our 20-score example, $D_9=P_{90}=88$ under this notebook's convention. There are nine dividing points for ten conceptual groups; ties prevent a promise of exactly equal distinct-score groups in every small sample.

**Memory:** **Quartiles → four groups. Deciles → ten. Percentiles → hundredth-position landmarks.**

**Try it yourself**

1. Which percentile is the third decile?
2. What is D5 under the same convention as the numerical median?

<details>
<summary>Answers and explanations — open after trying</summary>

1. D3 = P30.

2. D5 = P50 = the median.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="iqr"></a>
### 4.9 Interquartile Range — Focus on the middle half

The principal knows the total range but asks:

> “What if I want to know how spread out the middle group is without letting the extremes dominate?”

**The problem:** Range uses the minimum and maximum. Variance and SD use every numerical value, so extreme distances can have a strong influence. Sometimes our question is specifically about the middle half.

> **IQR measures the width of the middle 50% of the data, using the difference between the third and first quartiles.**

$$
\boxed{IQR=Q_3-Q_1=P_{75}-P_{25}}.
$$

$Q_1$ is the first quartile; $Q_3$ is the third; IQR has the original data unit.

For our 20 marks:

$$
IQR=77-52=25\text{ marks}.
$$

```text
Min 35      Q1 52        Median 66.5       Q3 77       Max 95
                <--------- IQR = 25 --------->
```

The middle-half interval extends from 52 to 77. These marks are not “normal students” in a diagnostic sense; they are simply the middle section by ordered position.

**The outlier-resistance example**

Change the lowest mark from 35 to 5, leaving all other marks unchanged. With our stated quartile convention:

```text
Before: Range = 95 − 35 = 60; IQR = 77 − 52 = 25
After:  Range = 95 − 5  = 90; IQR = 77 − 52 = 25
```

The range changes dramatically. The IQR stays the same because this endpoint change did not change the quartile positions or values.

**Why not always use IQR?** It deliberately leaves out how far the most extreme values lie. That can be a strength for resistant summaries and a limitation when total extremes matter. It can also be zero when many central values tie.

```text
CENTER                         SPREAD
Mean                           Standard Deviation
Uses all magnitudes            Uses all squared distances
Sensitive to extremes          Sensitive to extremes

Median                         IQR
Position-based                 Middle-half width
Resistant to extremes          Resistant to extremes
```

**Cross-question:** Does IQR = 25 mean SD = 25? No. They measure different things and have no fixed equality without additional assumptions.

**Memory:** **Range = outer edges. IQR = inner half.**

**Try it yourself**

1. Q1 = 50 and Q3 = 80. Find IQR.
2. Can the minimum change without changing IQR?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 80 − 50 = 30, in the same unit as the observations.

2. Yes. An extreme change that leaves the quartile values unchanged changes range but not IQR.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="five-number-summary"></a>
### 4.10 Five-number summary — Five checkpoints across the class

The principal asks:

> “Can you give me a very small set of numbers that tells me roughly where the class starts, where the middle is, where the middle half lies, and where the class ends?”

**The problem:** Mean alone gives one center. Range alone gives one width. Neither supplies landmarks inside the full span.

> **The Five-Number Summary is a set of five values that describes the position and spread of a numerical dataset using its minimum, first quartile, median, third quartile, and maximum.**

$$
\boxed{\left(\min,Q_1,M,Q_3,\max\right)}.
$$

Here $M=Q_2$ is the median. The minimum and maximum are the smallest and largest observed values.

**Calculate it using our original 20 marks**

```text
35,40,44,48,50,54,58,60,62,65,
68,70,72,74,76,78,82,86,90,95
```

| Landmark | Calculation | Value |
|---|---|---:|
| Minimum | First sorted value | 35 |
| $Q_1$ | $(50+54)/2$ | 52 |
| Median | $(65+68)/2$ | 66.5 |
| $Q_3$ | $(76+78)/2$ | 77 |
| Maximum | Last sorted value | 95 |

$$
\boxed{(35,52,66.5,77,95)}.
$$

**What does this tell the principal?**

The lowest mark is 35; the lower-quarter boundary is 52; the middle is 66.5; the upper-quarter boundary is 77; the highest mark is 95.

```text
START       lower-quarter       MIDDLE       upper-quarter       END
 Min             Q1              Median          Q3              Max
```

This is a positional sketch, not an equal-distance drawing. The gaps can differ even though the landmarks target equal proportions of observations.

**Two spread measures can be recovered immediately**

$$
\boxed{R=\max-\min=95-35=60},
\qquad
\boxed{IQR=Q_3-Q_1=77-52=25}.
$$

The summary does **not** generally determine the mean, variance, SD, or every detail of the distribution. For this actual dataset, the mean is 65.35; it is not part of the five-number summary.

**Why not include the mean?** This particular summary is built from ordered landmarks. The mean summarizes numerical balance rather than a chosen order position. The endpoints are still sensitive to extremes, so do not call the entire five-number summary outlier-proof.

**The next connection**

```text
Quartiles → Five-number summary → Basic box plot
```

A basic min–max box plot draws the five landmarks. A modified outlier-marking box plot has a different whisker rule; we preview that separately rather than confusing its whisker ends with the actual minimum and maximum.

**Memory:** **Start, quarter, middle, three-quarters, end.**

**Try it yourself**

1. From (35,52,66.5,77,95), recover range and IQR.
2. Can two different datasets share a five-number summary?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Range = 60; IQR = 25.

2. Yes. Values between the selected landmarks can differ. The summary is compact, not a reconstruction of all observations.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="coefficient-variation"></a>
### 4.11 Coefficient of Variation — Spread relative to what?

The principal thinks:

> “If one class has a larger SD, it must always be more inconsistent.”

Then he sees:

| Assessment | Mean | SD |
|---|---:|---:|
| Mathematics | 80 | 8 |
| Quiz | 20 | 5 |

**The problem:** Maths has larger absolute spread: 8 > 5. But 8 is only a tenth of 80, whereas 5 is a quarter of 20. The question of **relative** variation needs a reference size.

> **CV tells us how big the standard deviation is compared with the mean.**

Population percentage form:

$$
\boxed{CV=\frac{\sigma}{\mu}\times100\%}.
$$

Sample percentage form:

$$
\boxed{CV=\frac{s}{\bar{x}}\times100\%}.
$$

$\sigma$ or $s$ is SD; $\mu$ or $\bar{x}$ is the matching mean. CV can also be reported as a ratio without the percentage conversion.

**Calculate our comparison**

$$
CV_{\text{Maths}}=\frac8{80}\times100\%=10\%,
\qquad
CV_{\text{Quiz}}=\frac5{20}\times100\%=25\%.
$$

The quiz has greater spread **relative to its average points**. Maths still has the larger spread in raw points. Neither calculation overturns the other; they answer different questions.

**Why is CV unitless?**

$$
\frac{8\text{ marks}}{80\text{ marks}}=0.1.
$$

The units cancel. Multiplying all values by a positive scale factor multiplies both mean and SD by the same factor:

$$
\frac{a\sigma}{a\mu}=\frac{\sigma}{\mu}\quad(a>0).
$$

For generic scaled numerical values `8,10,12` versus `80,100,120`, population means are 10 and 100; population SDs are approximately 1.633 and 16.330. Both CVs are approximately 16.33%. The second list is a scaling illustration, not marks out of 100.

**Other comparisons from our discussion**

Class A: mean 70, SD 7 → CV 10%. Class B: mean 40, SD 6 → CV 15%. Class A has the lower relative spread, although its SD is larger.

A school workshop's two machines make parts averaging 100 mm and 10 mm, with SDs 2 mm and 1 mm. Their CVs are 2% and 10%. The smaller parts vary more in proportion to their average length. Relative variation is not the same as meeting a manufacturing tolerance.

**The important limitations**

The mean should be positive and meaningfully away from zero, and ratios to the mean should make sense for the measured quantity. If the mean is 0, CV is undefined. If the mean is 0.1 and SD 2, the CV is 2,000%, which may be unstable and unhelpful.

An arbitrary zero causes another problem: adding a constant changes the mean but not SD. Celsius and Fahrenheit therefore produce different CVs for the same temperatures. Use CV where the ratio-scale interpretation is justified; do not infer ratios of student ability from point-score CVs. [Scale and zero-point check: S3.](#reference-s3)

**Cross-question:** Does CV = 10% mean 10% of students are far from the mean? No. It means SD is one-tenth of the mean, not a proportion of students.

**Memory:** **SD → spread in units. CV → SD as a share of the mean.**

**Try it yourself**

1. Group A has mean 50, SD 5; B has mean 100, SD 20. Compare CVs.
2. What happens to CV if 10 is added to every value?

<details>
<summary>Answers and explanations — open after trying</summary>

1. A: 10%. B: 20%. B has greater relative variability under a meaningful ratio-scale comparison.

2. SD is unchanged but the mean increases by 10, so CV generally changes. This is why an arbitrary zero is a problem.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="other-dispersion"></a>
### 4.12 Other dispersion measures we mentioned briefly

> **Coverage:** Introduced / preview; not a full advanced treatment.

These appeared when we checked for missing concepts. They belong under dispersion, but we did not give them the same extended treatment as SD, IQR, and CV. Keep that distinction visible rather than silently marking every named measure complete.

[Back to the topic index](#clickable-topic-index)


<a id="quartile-deviation"></a>
#### 4.12.1 Quartile Deviation / Semi-IQR

> **Coverage:** Introduced / preview; not a full advanced treatment.

The principal already has the width of the middle half and asks for half that width as a compact scale measure.

> **Quartile Deviation, also called Semi-Interquartile Range, is half the interquartile range.**

$$
\boxed{QD=\frac{Q_3-Q_1}{2}=\frac{IQR}{2}}.
$$

$QD$ is quartile deviation; $Q_1,Q_3$ are quartiles. Its unit is the original data unit.

In the example introduced earlier, $Q_1=50$ and $Q_3=80$:

$$
IQR=30,\qquad QD=15.
$$

For the original 20 marks, QD = $25/2=12.5$ marks.

**What problem does it solve?** It supplies a conventional half-width version of the middle-half spread. It does not add new information beyond IQR and is not automatically an average distance from the median. The median need not lie halfway between $Q_1$ and $Q_3$.

**Memory:** **Semi-IQR = half the middle-half width.**

**Try it yourself**

1. IQR is 24 marks. What is quartile deviation?
2. Does QD = 12 imply the median is exactly 12 marks from both quartiles?

<details>
<summary>Answers and explanations — open after trying</summary>

1. QD = 24/2 = 12 marks.

2. No. QD is half the quartile gap. The median need not be the midpoint of that gap.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="coefficient-range"></a>
#### 4.12.2 Coefficient of Range

> **Coverage:** Introduced / preview; not a full advanced treatment.

**The question:** Can the endpoint gap be expressed relative to the size of the endpoints rather than only in marks?

> **The coefficient of range is the difference between the largest and smallest values divided by their sum.**

$$
\boxed{C_R=\frac{L-S}{L+S}}.
$$

$L$ is the largest value and $S$ the smallest. This version is most interpretable for appropriate nonnegative ratio-scale values with $L+S>0$.

For $L=100$ and $S=40$:

$$
C_R=\frac{60}{140}=\frac37\approx0.4286.
$$

It is unitless under positive multiplicative unit changes, but remains entirely dependent on the two extremes. An arbitrary added constant changes it.

**What problem remains?** It cannot distinguish our Class C and Class D because their endpoints are identical. A relative measure can still discard important internal information.

**Memory:** **Endpoint difference / endpoint sum.**

**Try it yourself**

1. Find the coefficient of range when L = 80 and S = 20.
2. Does this measure fix Range’s problem of ignoring middle observations?

<details>
<summary>Answers and explanations — open after trying</summary>

1. (80 − 20)/(80 + 20) = 60/100 = 0.6.

2. No. It rescales the endpoint comparison but still uses only the endpoints.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="coefficient-quartile"></a>
#### 4.12.3 Coefficient of Quartile Deviation

> **Coverage:** Introduced / preview; not a full advanced treatment.

**The question:** Can we express the quartile gap relative to the quartile level rather than only in original units?

> **The coefficient of quartile deviation is the difference between the third and first quartiles divided by their sum.**

$$
\boxed{C_Q=\frac{Q_3-Q_1}{Q_3+Q_1}}.
$$

$Q_1,Q_3$ are the first and third quartiles. A meaningful relative interpretation requires suitable measurement scale and a nonzero denominator.

For $Q_1=50,Q_3=80$:

$$
C_Q=\frac{30}{130}=\frac3{13}\approx0.2308.
$$

This is not the same as QD = 15 marks or IQR = 30 marks. It is a dimensionless relative version.

**Cross-question:** Can it be used indiscriminately on arbitrary-zero scales? No. Adding the same constant to all data changes the denominator without changing the quartile gap.

**Memory:** **Quartile difference / quartile sum.**

**Try it yourself**

1. Q1 = 30 and Q3 = 50. Find this coefficient.
2. What is the distinction between this coefficient and IQR?

<details>
<summary>Answers and explanations — open after trying</summary>

1. (50 − 30)/(50 + 30) = 20/80 = 0.25.

2. IQR is a width in the original unit. The coefficient divides that width by Q1 + Q3 and is a relative ratio.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="shape-previews"></a>
## 5. Distribution shape and outliers — Connections already introduced

> **Coverage:** Introduced / preview; not a full advanced treatment.

These ideas appeared while choosing a center and discussing the five-number summary. They are recorded here as **introductions**, not as a claim that we completed every topic on distribution shape or numerical graphics.

[Back to the topic index](#clickable-topic-index)


<a id="shape-skewness"></a>
### 5.1 Symmetry, skewness, and the mean–median–mode pattern

> **Coverage:** Introduced / preview; not a full advanced treatment.

The principal compares the center with the actual shape of the marks.

**The problem:** A mean and SD do not show whether marks are balanced, have a long tail, or form two groups.

A **symmetric distribution** has matching left and right structure about a center. **Skewness** describes asymmetry; a longer right tail suggests right skew, and a longer left tail suggests left skew.

```text
Balanced class → 50,60,70,70,70,80,90
High-side tail → 20,25,30,35,40,45,90
Low-side tail  → 0,65,70,75,80
```

The balanced example has mean = median = mode = 70. The high-tail example has mean ≈ 40.71 and median 35. The low-tail example has mean 58 and median 70.

**Why did this help our choice of center?** A distant value changes the total and hence the mean, while a median depends on central positions. Comparing both can reveal that a single balance-point summary misses the typical position.

**An important qualification to our early shortcut**

`Mode < Median < Mean` for right skew and the reverse for left skew are common illustrations, not universal mathematical laws. Symmetry does not guarantee a unique central mode: symmetric data can have two peaks. Do not infer an entire distribution's shape from three numbers alone.

**Formula?** Formal skewness coefficients were not taught in this thread. We retain the visual concept rather than adding an unexplained formula and calling the chapter complete. [Terminology check: S7.](#reference-s7)

**Memory:** **Look at the tail and the whole graph; do not use a mean–median ordering as a universal proof.**

**Try it yourself**

1. For 0,65,70,75,80, which center is pulled downward?
2. Does symmetry always imply exactly one mode at the center?

<details>
<summary>Answers and explanations — open after trying</summary>

1. The mean becomes 58; the median remains 70.

2. No. A symmetric two-peaked distribution can have two modes away from the center.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="outliers"></a>
### 5.2 Outliers — A rule for flagging, not automatic deletion

> **Coverage:** Introduced / preview; not a full advanced treatment.

The principal notices one very low mark while most of the class lies much higher.

**The problem:** “It looks unusual” can be vague. A consistent descriptive rule helps identify values worth investigating.

An **outlier** is an observation unusually separated from the relevant pattern or bulk of the data. Unusual does not automatically mean erroneous.

The IQR rule previewed in our discussion is:

$$
\boxed{L=Q_1-1.5\,IQR},\qquad
\boxed{U=Q_3+1.5\,IQR}.
$$

$L$ and $U$ are lower and upper fences; $Q_1,Q_3$ are quartiles; $IQR=Q_3-Q_1$. Values below $L$ or above $U$ are flagged as possible outliers by this rule.

For $Q_1=52,Q_3=77,IQR=25$:

$$
L=52-37.5=14.5,\qquad U=77+37.5=114.5.
$$

The original minimum 35 is not flagged. If it changes to 5 while these quartiles stay unchanged, 5 is below 14.5 and is flagged.

**Cross-question:** Is 114.5 an impossible observation on a 100-mark test, so the rule is invalid? No. A fence is a computed threshold, not a claim about the permitted score range. Here no permitted upper-end mark can exceed that upper fence.

Investigate recording mistakes, unusual circumstances, and the question being studied. Do not automatically remove a valid low score because it changes a mean or correlation.

**Memory:** **Outlier flag → investigate. It does not mean “delete.”**

**Try it yourself**

1. Q1 = 50 and Q3 = 70. Find the fences.
2. A valid observation lies below the lower fence. Must it be removed?

<details>
<summary>Answers and explanations — open after trying</summary>

1. IQR = 20. Lower fence = 50 − 30 = 20; upper fence = 70 + 30 = 100.

2. No. The fence is a descriptive flag; whether to exclude a value requires a justified reason, not merely its extremeness.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="box-plot"></a>
### 5.3 Box plot — Draw the five-number landmarks

> **Coverage:** Introduced / preview; not a full advanced treatment.

We have five useful numbers, but the principal wants to see them together.

> **A box plot is a graph summarizing a numerical distribution using a box between the quartiles, a median line, and whiskers whose endpoints depend on the stated convention.**

**What problem does it solve?** It makes center and middle-half spread easy to compare across classes without drawing every observation.

For our original summary `(35,52,66.5,77,95)`, a schematic basic plot is:

```text
35          52             66.5       77          95
|-----------[================|========]-----------|
Min         Q1            Median     Q3          Max
```

The drawing is schematic, not a precise numeric scale.

**Two conventions must not be confused**

A basic **min–max box plot** sends whiskers to the actual minimum and maximum. A common **modified box plot** sends whiskers to the most extreme observed values inside the $1.5\,IQR$ fences and displays more extreme observations separately. Fences are not themselves automatically whisker endpoints. [Convention check: S6.](#reference-s6)

After replacing 35 with 5, the lower fence is 14.5. The modified lower whisker reaches **40**, the smallest remaining observed value inside the fence; the score 5 appears separately. The five-number summary still has actual minimum **5**.

**Formula relationships**

$$
\text{Box span}=Q_3-Q_1=IQR;
\quad\text{median line}=M.
$$

Whisker endpoints are selected observations, not a new averaging formula.

**Memory:** **Box = middle half. Line = median. Whiskers = check the convention.**

**Try it yourself**

1. Are the ends of a modified box plot always the minimum and maximum?
2. After replacing the original minimum 35 by 5, where is the lower modified whisker?

<details>
<summary>Answers and explanations — open after trying</summary>

1. No. Points beyond the fences can be plotted separately; whiskers end at the most extreme non-flagged observations.

2. At 40, because the lower fence is 14.5 and 40 is the smallest observation still inside it.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="association"></a>
## 6. Week 4 — Association: What changes when we study two variables?

So far we mainly studied one variable at a time. The principal's new question is:

> “Are these two characteristics connected?”

```text
Categorical + Categorical
    → Contingency tables → Relative frequencies → Association / independence

Numerical + Numerical
    → Scatterplots → Covariance → Pearson correlation

Binary Categorical + Numerical
    → Point-biserial correlation
```

Paired observations are essential in every branch. A collection of marks and a separate collection of tutoring labels do not show association unless we retain which belong to the same student.

[Back to the topic index](#clickable-topic-index)


<a id="contingency-table"></a>
### 6.1 Contingency tables — Preserve how categories occur together

The school has 20 students. Separate frequency tables tell us:

| Exam result | Students |
|---|---:|
| Pass | 12 |
| Fail | 8 |

| Extra tutoring | Students |
|---|---:|
| Yes | 10 |
| No | 10 |

The principal asks:

> “Of the students who took tutoring, how many passed?”

**The problem:** The separate tables have lost the pairing. We know how many passed and how many took tutoring, but not how those categories overlap.

**Why the missing pairing matters**

Both of these arrangements match the separate totals:

```text
Arrangement A                 Arrangement B
Tutoring Yes: 8 Pass, 2 Fail   Tutoring Yes: 6 Pass, 4 Fail
Tutoring No:  4 Pass, 6 Fail   Tutoring No:  6 Pass, 4 Fail
```

The marginal totals are identical, but the association pattern differs. We need to cross-classify the same students by both variables.

> **A contingency table is a table that shows the frequency of observations for combinations of two or more categorical variables.**

For two variables it is also a **two-way table**, **cross-tabulation**, or **crosstab**.

| Extra tutoring | Pass | Fail | Total |
|---|---:|---:|---:|
| Yes | 8 | 2 | 10 |
| No | 4 | 6 | 10 |
| **Total** | **12** | **8** | **20** |

**Inside each cell: a joint frequency**

The cell 8 means **Tutoring = Yes AND Result = Pass**. It does not mean all tutoring students, and it does not mean all passing students.

```text
Joint = both conditions together
Marginal = one variable by itself, obtained at the table's margins
```

**Symbols and totals**

Let $f_{ij}$ be the count in row $i$, column $j$.

$$
\boxed{R_i=\sum_jf_{ij}},\qquad
\boxed{C_j=\sum_if_{ij}},\qquad
\boxed{N=\sum_i\sum_jf_{ij}}.
$$

$R_i$ is a row total; $C_j$ a column total; $N$ the grand total. A sum over $j$ moves across columns, while a sum over $i$ moves down rows.

Here tutoring row totals are 10 and 10, result column totals 12 and 8, and $N=20$. Row and column totals are **marginal frequencies** because they sit at the margins.

**Why the name?** “Contingent on” provides a useful reading question: does the result distribution differ depending on tutoring status? The table records combinations whether or not dependence is actually present; its name does not assert an association.

**Not only 2 × 2**

Our table has two row categories and two column categories, excluding totals. A Study Method × Performance table can be 3 × 3:

| Method | Low | Medium | High |
|---|---:|---:|---:|
| Self Study | 5 | 10 | 8 |
| Tutoring | 3 | 8 | 12 |
| Group Study | 4 | 9 | 11 |

It answers how categories occur together. We have not established that a study method caused any result.

**The next problem — unequal groups**

| Tutoring | Pass | Fail | Total |
|---|---:|---:|---:|
| Yes | 16 | 4 | 20 |
| No | 24 | 16 | 40 |
| **Total** | **40** | **20** | **60** |

There are more passes without tutoring, 24 versus 16. But there are twice as many students without tutoring. Comparing counts alone does not answer who has the higher pass rate.

**Memory:** **One categorical variable → frequency table. Two together → contingency table.**

**Try it yourself**

1. In the 20-student table, what does cell 8 represent?
2. Can separate tutoring and result totals determine the contingency table uniquely?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Eight students both took tutoring and passed: a joint frequency.

2. No. Different joint pairings can produce the same marginal totals, as the two arrangements demonstrate.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="contingency-relative"></a>
### 6.2 Relative frequencies in contingency tables — Always ask “out of what?”

Continue with the unequal groups:

| Extra tutoring | Pass | Fail | Total |
|---|---:|---:|---:|
| Yes | 16 | 4 | 20 |
| No | 24 | 16 | 40 |
| **Total** | **40** | **20** | **60** |

Someone says:

> “24 students without tutoring passed, while only 16 tutoring students passed. The non-tutoring students must have performed better.”

**The problem:** A raw count is being mistaken for a within-group rate.

> **Relative frequency is the proportion of observations belonging to a category or combination of categories relative to a specified total.**

$$
\boxed{\text{Relative frequency}=\frac{\text{frequency}}{\text{relevant total}}}.
$$

The important word is **relevant**. Different denominators answer different questions.

**1. Joint relative frequency — out of everyone**

The 16 tutoring students who passed are:

$$
\frac{16}{60}\approx0.2667=26.67\%
$$

of all students.

$$
\boxed{\text{Joint relative frequency}_{ij}=\frac{f_{ij}}N}.
$$

| Tutoring | Pass | Fail | Share of all students |
|---|---:|---:|---:|
| Yes | 26.67% | 6.67% | 33.33% |
| No | 40.00% | 26.67% | 66.67% |
| **Total** | **66.67%** | **33.33%** | **100%** |

All internal cells total 100% before rounding. Rounded displayed cells can total 100.01%.

**2. Marginal relative frequency — an edge total out of everyone**

$$
\boxed{\frac{R_i}{N}\text{ for row margins},\qquad\frac{C_j}{N}\text{ for column margins}}.
$$

Tutoring share = $20/60=33.33\%$. Overall pass share = $40/60=66.67\%$. A marginal proportion summarizes one variable without conditioning on the other.

**3. Row conditional relative frequency — within each tutoring group**

The principal asks:

> “Among students who took tutoring, what percentage passed?”

The relevant group has 20 students:

$$
16/20=80\%.
$$

Without tutoring:

$$
24/40=60\%.
$$

| Tutoring | Pass | Fail | Row total |
|---|---:|---:|---:|
| Yes | 80% | 20% | 100% |
| No | 60% | 40% | 100% |

$$
\boxed{\text{Row conditional relative frequency}_{ij}=\frac{f_{ij}}{R_i}}.
$$

Every row now represents one complete subgroup, so each row totals 100%.

**4. Column conditional relative frequency — within each result group**

Reverse the question:

> “Among students who passed, what percentage took tutoring?”

There are 40 passing students. Of these, 16 took tutoring:

$$
16/40=40\%.
$$

| Tutoring | Among Pass | Among Fail |
|---|---:|---:|
| Yes | 40% | 20% |
| No | 60% | 80% |
| **Column total** | **100%** | **100%** |

$$
\boxed{\text{Column conditional relative frequency}_{ij}=\frac{f_{ij}}{C_j}}.
$$

**Same cell, three useful denominators**

```text
16 / 60 → 26.67% of everyone took tutoring AND passed
16 / 20 → 80% of tutoring students passed
16 / 40 → 40% of passing students took tutoring
```

All are correct. They are not interchangeable.

**Probability notation — a bridge**

If we choose uniformly from these 60 observed students:

$$
P(\text{Pass}\mid\text{Tutoring Yes})=16/20=0.80,
$$

$$
P(\text{Tutoring Yes}\mid\text{Pass})=16/40=0.40.
$$

$P$ means probability under that selection; $\mid$ means “given that.” These are empirical proportions for the observed dataset, not automatically known probabilities in a wider population.

**Cross-question:** Which words tell me the denominator? Usually the group after **“among”** or **“given that.”**

**The next question:** The pass distributions differ, 80% versus 60%. What does that tell us about association, and what would no association look like?

**Memory:** **The denominator tells you the meaning.**

**Try it yourself**

1. What percentage of all 60 students did not take tutoring and failed?
2. Among students who failed, what percentage did not take tutoring?

<details>
<summary>Answers and explanations — open after trying</summary>

1. 16/60 × 100% ≈ 26.67%: a joint relative frequency.

2. 16/20 × 100% = 80%: a column conditional percentage. The denominator is all failures, not all non-tutoring students.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="categorical-association"></a>
### 6.3 Association and independence between categorical variables

The principal compares the conditional distributions:

| Extra tutoring | Pass | Fail |
|---|---:|---:|
| Yes | 80% | 20% |
| No | 60% | 40% |

He asks:

> “Does exam result seem to depend on whether a student took tutoring?”

**What problem does the concept solve?** Separate summaries cannot describe whether knowing one variable changes what we expect about the other. Conditional distributions can.

> **Two categorical variables are associated when the distribution of one variable changes depending on the category of the other variable.**

In these observed data, the pass proportion differs by tutoring status.

```text
Tutoring Yes → PASS ████████ 80% / FAIL ██   20%
Tutoring No  → PASS ██████   60% / FAIL ████ 40%
```

**What would no association look like?**

Consider a separate illustrative table:

| Tutoring | Pass | Fail | Total |
|---|---:|---:|---:|
| Yes | 16 | 4 | 20 |
| No | 32 | 8 | 40 |
| **Total** | **48** | **12** | **60** |

Each row has 80% Pass and 20% Fail. Knowing tutoring status does not change the observed result distribution.

> **Two variables are independent when knowing the value of one variable does not change the distribution of the other.**

At the population/model level, this is an exact property. In a sample, differences can occur even under population independence, and identical sample percentages do not prove population independence.

**Formal rules and symbols**

For every relevant pair of categories $x,y$ with $P(X=x)>0$:

$$
\boxed{P(Y=y\mid X=x)=P(Y=y)}.
$$

Equivalently, for all category pairs:

$$
\boxed{P(X=x,Y=y)=P(X=x)P(Y=y)}.
$$

$X,Y$ are variables; $x,y$ their particular categories; $P$ is probability; $\mid$ means given. For events $A,B$, the second rule is $P(A\cap B)=P(A)P(B)$, where $\cap$ means AND.

The equality must hold across the distributions, not just one selected cell in a many-category table.

**Quantify our observed difference**

Let $p_1=0.80$ be the tutoring pass proportion and $p_0=0.60$ the non-tutoring pass proportion.

$$
\boxed{p_1-p_0=0.20=20\text{ percentage points}}.
$$

It is **not** the same as “20% higher.” Relative to 60%, the increase is $0.20/0.60\approx33.33\%$. Keep percentage points and relative percentage changes distinct.

**What would independence predict with the original margins?**

In the original table, $N=60$, tutoring total = 20, pass total = 40. The expected Tutoring-Yes/Pass count under an independence model is:

$$
\boxed{E_{ij}=\frac{R_iC_j}{N}}.
$$

$E_{ij}$ is expected count, $R_i,C_j$ the row and column totals.

$$
E_{\text{Yes,Pass}}=20(40)/60\approx13.33.
$$

The observed count is 16. An expected count can be fractional because it is a model-based average, not a literal partially counted student. A later chi-square test asks how unusual the whole pattern of differences is under a sampling model; we have not completed that test here.

**A three-category example from our discussion**

| Method | Low | Medium | High | Total |
|---|---:|---:|---:|---:|
| Self Study | 8 | 12 | 10 | 30 |
| Tutoring | 3 | 7 | 20 | 30 |

Row percentages are `26.67%,40%,33.33%` versus `10%,23.33%,66.67%`. The conditional distributions differ, showing descriptive association in the recorded data.

**Association is not causation**

Tutoring students may also differ in motivation, attendance, prior preparation, or resources. An observed difference alone does not prove that tutoring caused it. Nor does the word association automatically imply statistical significance.

**Direction and symmetry**

Association is symmetric: if $X$ is associated with $Y$, $Y$ is associated with $X$. But $P(Y\mid X)$ and $P(X\mid Y)$ have different denominators. Positive/negative language is not generally meaningful for unordered labels; when binary codes are used, the sign depends on which categories are coded high.

**Memory:** **Split into groups → compare conditional distributions → distinguish description from inference and causation.**

**Try it yourself**

1. Pass rates are 80% in both tutoring groups. What does this say about the observed table?
2. Pass rates are 80% versus 60%. State the difference correctly and whether it proves causation.

<details>
<summary>Answers and explanations — open after trying</summary>

1. The observed result distributions are identical by tutoring status. It shows no association in that empirical table, but does not prove population independence from a finite sample.

2. The difference is 20 percentage points. It is an observed association, not by itself a causal conclusion or a significance test.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="scatterplots"></a>
### 6.4 Scatterplots — See how two numerical variables behave together

The principal changes the question:

> “Do students who study more hours tend to score higher marks?”

Now both variables are numerical. A contingency table of raw labels is no longer the natural first representation.

| Student | Study hours $x$ | Marks $y$ |
|---|---:|---:|
| A | 1 | 45 |
| B | 2 | 52 |
| C | 3 | 60 |
| D | 4 | 68 |
| E | 5 | 75 |
| F | 6 | 82 |

**The problem:** Six pairs are readable, but 100 pairs in a table can be difficult to inspect. Two separate histograms would lose which hours belong to which marks.

> **A scatterplot is a graph that displays pairs of numerical observations as points to show the relationship or association between two quantitative variables.**

Each student contributes one paired point:

$$
\boxed{(x_i,y_i)}.
$$

$x_i$ is that student's study time; $y_i$ is that same student's mark; $i$ identifies the student.

```text
Marks
 85 |                 ●
 75 |              ●
 65 |           ●
 60 |        ●
 50 |     ●
 45 |  ●
    +----------------------
       1  2  3  4  5  6     Study hours
```

This is a schematic, not a precision plot. The points rise overall from left to right.

**What should we inspect? D-S-F-O**

**Direction:** As $x$ increases, does $y$ generally rise, fall, or show no clear trend? The study-time example is positive. Absences `1,2,3,5,7` paired with marks `88,83,78,68,57` give a negative pattern.

**Strength:** How closely do the points follow the visible pattern? A tight trend and a widely scattered trend can have the same direction but different strength. This is not the same as the slope's steepness.

**Form:** Is the pattern approximately straight, curved, flat, clustered, or something else? Marks might improve with study time and then level off. A nonlinear association can still be strong.

**Outliers:** Is a point unusually separated from the pattern? A student studying 6 hours and scoring 30 when the rest follow an upward trend needs attention. It may be valid; it may substantially affect a later correlation.

**Axes**

Conventionally put the explanatory/predictor variable on $x$ and response/outcome on $y$ when those roles make sense. Merely choosing $x$ does not establish causation or independence.

**The no-obvious-pattern example**

Shoe sizes `7,8,9,10,11` paired with marks `65,82,61,77,69` have no obvious smooth upward/downward pattern in this small illustration. A small visual example is not proof that these variables are independent in every population.

**Cross-question:** Why not connect the points like a time series? A scatterplot treats each pair as an observation, not necessarily a sequence in time. Connecting in arbitrary student order can suggest a path that was never observed.

**Association is not causation:** Study time, motivation, attendance, and prior knowledge may be related. The graph reveals a pattern, not its cause.

**The next problem:** We can see joint movement, but can we put a number on whether deviations tend to go together? That motivates covariance.

**Memory:** **Scatterplot first. Direction, Strength, Form, Outliers.**

**Try it yourself**

1. What is lost by drawing separate distributions of hours and marks?
2. A clear curved pattern has no single upward straight trend. Is association necessarily absent?

<details>
<summary>Answers and explanations — open after trying</summary>

1. The student-by-student pairings. Separate distributions do not show which score goes with which study time.

2. No. It may be a strong nonlinear association that a linear summary captures poorly.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="covariance"></a>
### 6.5 Covariance — Turn paired deviations into a number

The scatterplot suggests that study hours and marks rise together. The principal asks:

> “Can we measure this joint movement with a number instead of only looking at the graph?”

**The problem:** A picture shows a pattern, but we want an algebraic measure of whether both variables tend to be above their means together, below together, or on opposite sides.

> **Covariance measures whether two numerical variables tend to vary together in the same direction or in opposite directions.**

More precisely, the population/empirical form averages products of paired deviations from the two means.

**Why multiply the deviations?**

| Position of $X$ | Position of $Y$ | Product sign |
|---|---|---|
| Above mean | Above mean | $(+)(+)=+$ |
| Below mean | Below mean | $(-)(-)=+$ |
| Above mean | Below mean | $(+)(-)=-$ |
| Below mean | Above mean | $(-)(+)=-$ |

Same-side deviations give positive products; opposite-side deviations give negative products. Their sizes also matter, not just how many products have each sign.

**Population covariance formula**

$$
\boxed{\operatorname{Cov}(X,Y)=\frac1N\sum_{i=1}^{N}(x_i-\mu_X)(y_i-\mu_Y)}.
$$

$X,Y$ are the variables; $(x_i,y_i)$ is one matched pair; $\mu_X,\mu_Y$ are population means; $N$ is the number of population pairs.

**Sample covariance formula**

$$
\boxed{s_{XY}=\frac{\sum_{i=1}^{n}(x_i-\bar{x})(y_i-\bar{y})}{n-1}}.
$$

$s_{XY}$ is sample covariance; $\bar{x},\bar{y}$ are sample means; $n$ is sample size. As with variance, the $n-1$ form has an estimation role.

**Our simplified five-student calculation**

| Student | Hours $x$ | Marks $y$ | $x-3$ | $y-70$ | Product |
|---|---:|---:|---:|---:|---:|
| A | 1 | 50 | −2 | −20 | 40 |
| B | 2 | 60 | −1 | −10 | 10 |
| C | 3 | 70 | 0 | 0 | 0 |
| D | 4 | 80 | 1 | 10 | 10 |
| E | 5 | 90 | 2 | 20 | 40 |
| **Total** | **15** | **350** | **0** | **0** | **100** |

The means are 3 hours and 70 marks. If these are the complete five students of interest:

$$
\boxed{\operatorname{Cov}(X,Y)=100/5=20\text{ hour·marks}}.
$$

If computing the usual sample covariance estimate:

$$
s_{XY}=100/4=25\text{ hour·marks}.
$$

**What does positive 20 mean?** Students below average in hours are also below average in marks, and those above average tend to be above in both. Covariance is positive. It is not a slope of 20 marks per hour.

**Negative covariance**

For absences `1,2,3,4,5` paired with marks `90,80,70,60,50`, the products total −100. Population-form covariance = −20. Larger absences accompany lower marks.

**Zero covariance does not mean no relationship**

A curved illustrative pattern can cancel:

```text
Hours → 1, 2, 3, 4, 5
Marks → 90,60,50,60,90
```

The means are 3 and 70. Products are `−40,+10,0,−10,+40`, summing to zero. A U-shaped pattern exists, but net linear co-movement is zero.

**The unit problem — why covariance is not the final answer**

Hours × marks is an awkward unit. If hours become minutes, the first variable is multiplied by 60:

$$
\operatorname{Cov}(60X,Y)=60\operatorname{Cov}(X,Y).
$$

The covariance changes from 20 to 1,200 minute·marks. The actual association has not become 60 times stronger. Therefore covariance magnitude is not a standardized strength score.

**Connection with variance**

$$
\boxed{\operatorname{Cov}(X,X)=\operatorname{Var}(X)}
$$

because multiplying a deviation by itself squares it. Covariance is also symmetric: $\operatorname{Cov}(X,Y)=\operatorname{Cov}(Y,X)$.

**Cross-question:** Why not just average $x_iy_i$? Large positive baselines can make that large even without co-movement. Centering at the means isolates departures from each variable's typical level.

**Memory:** **Paired deviations → multiply → average. Same direction +, opposite direction −.**

**Try it yourself**

1. The paired deviation products total 100 across five pairs. Give population-form and sample covariance.
2. Hours become minutes. What happens to covariance and the actual pattern?

<details>
<summary>Answers and explanations — open after trying</summary>

1. Population-form: 100/5 = 20. Usual sample covariance: 100/4 = 25.

2. Covariance multiplies by 60. The underlying pattern is unchanged, which reveals covariance’s scale dependence.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="pearson"></a>
### 6.6 Pearson correlation — Standardise covariance

Covariance answered whether the variables tend to move together. But the principal asks:

> “Is a covariance of 20 weak or strong? Why does it become 1,200 when I use minutes instead of hours?”

**The problem:** Covariance depends on units and on how spread out each variable is. We need a unitless linear-association measure on a fixed scale.

> **Pearson correlation measures the direction and strength of the linear relationship between two numerical variables.**

For a sample:

$$
\boxed{r=\frac{s_{XY}}{s_Xs_Y}}.
$$

$r$ is Pearson correlation; $s_{XY}$ is sample covariance; $s_X,s_Y$ are the sample standard deviations of the corresponding variables. Use consistent covariance/SD conventions.

For a population:

$$
\boxed{\rho=\frac{\operatorname{Cov}(X,Y)}{\sigma_X\sigma_Y}}.
$$

$\rho$ (rho) is population correlation. Both spreads must be positive and finite for these ordinary formulas to be defined.

**Why divide by the SDs?**

Changing hours to minutes multiplies covariance by 60 and $SD_X$ by 60. The factors cancel. Adding a constant changes neither the centered products nor SD.

```text
Covariance
    ↓
Divide by SD of X × SD of Y
    ↓
Unitless standardised covariance
    ↓
Pearson correlation
```

**Range and interpretation**

$$
\boxed{-1\le r\le1}.
$$

$r=+1$: all points lie exactly on a positively sloped line. $r=-1$: all lie on a negatively sloped line. $r=0$: zero linear correlation, not necessarily no relationship.

The sign gives direction. $|r|$ (absolute value of $r$) gives linear strength: closer to 1 is stronger, closer to 0 weaker. Labels such as weak/moderate/strong depend on context.

**The perfect examples**

Hours `1,2,3,4,5` with marks `50,60,70,80,90` have $r=1$. Absences `1,2,3,4,5` with marks `90,80,70,60,50` have $r=-1$.

Perfect positive correlation does **not** require $Y=X$. It can follow $Y=10X+40$, as in the first example.

**Calculate the non-perfect example from our chat**

| Student | Hours $x$ | Marks $y$ | $x-3$ | $y-64$ | Product | $(x-3)^2$ | $(y-64)^2$ |
|---|---:|---:|---:|---:|---:|---:|---:|
| A | 1 | 50 | −2 | −14 | 28 | 4 | 196 |
| B | 2 | 55 | −1 | −9 | 9 | 1 | 81 |
| C | 3 | 65 | 0 | 1 | 0 | 0 | 1 |
| D | 4 | 70 | 1 | 6 | 6 | 1 | 36 |
| E | 5 | 80 | 2 | 16 | 32 | 4 | 256 |
| **Total** | **15** | **320** | **0** | **0** | **75** | **10** | **570** |

The means are $\bar{x}=3$ and $\bar{y}=64$.

$$
s_{XY}=75/4=18.75,
\quad s_X=\sqrt{10/4}=\sqrt{2.5},
\quad s_Y=\sqrt{570/4}=\sqrt{142.5}.
$$

$$
r=\frac{18.75}{\sqrt{2.5}\sqrt{142.5}}
\approx0.993399.
$$

$$
\boxed{r\approx0.9934}.
$$

Study time and marks show very strong positive linear association in this illustrative sample. Keep full precision until the final rounding.

**Equivalent direct formula**

$$
\boxed{r=\frac{\sum(x_i-\bar{x})(y_i-\bar{y})}
{\sqrt{\left[\sum(x_i-\bar{x})^2\right]\left[\sum(y_i-\bar{y})^2\right]}}}.
$$

The common $n-1$ factors cancel. Here this is $75/\sqrt{10\times570}$, giving the same answer.

**What it does not tell us**

A curved relationship can have $r=0$. Outliers can strongly alter $r$. A large sample correlation is not automatically a causal conclusion or a significance result. It does not mean “99.34% of students improve” or give marks gained per hour.

If one variable is constant, its SD is zero and correlation is **undefined**, not zero. Pearson correlation does not require normality merely to compute the descriptive coefficient; inferential procedures can have additional assumptions. [Formula and edge-case check: S4.](#reference-s4)

**Scale and symmetry**

Swapping $X$ and $Y$ leaves $r$ unchanged. Positive unit changes leave it unchanged. Multiplying only one variable by a negative number reverses its sign. Thus “unitless” does not mean the sign survives reversing the meaning of a scale.

**Memory:** **Correlation = standardised covariance. Scatterplot first; number second.**

**Try it yourself**

1. For the worked example, compute r using sums 75,10,570.
2. If all students studied exactly 3 hours, is the correlation with marks zero?

<details>
<summary>Answers and explanations — open after trying</summary>

1. r = 75/√(10 × 570) ≈ 0.9934.

2. No. The study-time SD is zero, so the Pearson formula divides by zero and the correlation is undefined.

</details>

[Back to the topic index](#clickable-topic-index)


<a id="point-biserial"></a>
### 6.7 Point-biserial correlation — Two groups, numerical outcomes

The principal returns to tutoring, but keeps marks numerical:

```text
Tutoring → Yes / No
Marks    → Numerical scores
```

He asks:

> “Do students who take tutoring tend to score differently from students who do not?”

**What problem occurred?** We know how to study categorical pairs and numerical pairs. This is the mixed case: a two-category group variable and a numerical outcome. Comparing means is useful, but we also want a standardised association measure.

> **Point-biserial correlation is Pearson correlation between a binary-coded variable and a numerical variable.**

The conventional setting is a dichotomous variable with a quantitative, often continuous, outcome. The numerical outcome can also be a score recorded in discrete increments.

**Keep the actual eight-student example from our conversation**

| Student | Tutoring | Binary code $B$ | Marks $Y$ |
|---|---|---:|---:|
| A | Yes | 1 | 85 |
| B | Yes | 1 | 90 |
| C | Yes | 1 | 80 |
| D | Yes | 1 | 88 |
| E | No | 0 | 70 |
| F | No | 0 | 68 |
| G | No | 0 | 75 |
| H | No | 0 | 72 |

**Step 1 — The two means**

$$
M_1=(85+90+80+88)/4=85.75,
$$

$$
M_0=(70+68+75+72)/4=71.25.
$$

$$
\Delta=M_1-M_0=14.5\text{ marks}.
$$

$M_1$ is the mean for code 1; $M_0$ for code 0; $\Delta$ is their difference. The difference alone does not yet account for total spread or group proportions.

**Step 2 — Group proportions**

$$
n_1=4,\quad n_0=4,\quad n=8,
\qquad p=n_1/n=0.5,\quad q=n_0/n=0.5.
$$

$p$ and $q$ are the observed proportions in the two groups, so $p+q=1$.

**Important formula clarification**

The earlier chat wrote $(M_1-M_0)\sqrt{pq}/s_Y$ without specifying the SD divisor. That compact form needs the overall SD calculated with divisor **$n$**, not the usual sample SD with divisor **$n-1$**.

Define the descriptive, divisor-$n$ spread:

$$
s_{Y,n}=\sqrt{\frac{\sum_{i=1}^{n}(y_i-\bar{y})^2}{n}}.
$$

Then:

$$
\boxed{r_{pb}=\frac{M_1-M_0}{s_{Y,n}}\sqrt{pq}}.
$$

If instead $s_Y=\sqrt{\sum(y_i-\bar{y})^2/(n-1)}$ is the usual sample SD, the equivalent formula is:

$$
\boxed{r_{pb}=\frac{M_1-M_0}{s_Y}
\sqrt{\frac{n_1n_0}{n(n-1)}}}.
$$

These are the **same correlation**, not competing estimates. The SD convention and size factor must match. [Formula check: S5.](#reference-s5)

**Step 3 — Compute the overall spread**

All eight marks total 628, so $\bar{y}=78.5$.

| Mark | Deviation from 78.5 | Squared deviation |
|---:|---:|---:|
| 85 | 6.5 | 42.25 |
| 90 | 11.5 | 132.25 |
| 80 | 1.5 | 2.25 |
| 88 | 9.5 | 90.25 |
| 70 | −8.5 | 72.25 |
| 68 | −10.5 | 110.25 |
| 75 | −3.5 | 12.25 |
| 72 | −6.5 | 42.25 |
| **Total** | **0** | **504** |

$$
s_{Y,n}=\sqrt{504/8}=\sqrt{63}\approx7.937254.
$$

**Step 4 — Calculate correlation**

$$
r_{pb}=\frac{14.5}{\sqrt{63}}\sqrt{0.5\times0.5}
=\frac{7.25}{\sqrt{63}}
\approx0.913414.
$$

$$
\boxed{r_{pb}\approx0.9134}.
$$

Check with the sample-SD form:

$$
s_Y=\sqrt{504/7}=\sqrt{72},
\quad r_{pb}=\frac{14.5}{\sqrt{72}}\sqrt{\frac{4\times4}{8\times7}}
\approx0.9134.
$$

**What does it mean?** With Yes coded 1, the positive sign means that group has higher mean marks. The magnitude indicates a strong observed binary–numerical correlation in these eight students. It is not proof that tutoring caused the difference.

**Why does $\sqrt{pq}$ appear?**

It is not an arbitrary fairness adjustment. A 0/1 variable has divisor-$n$ variance $pq$. Its covariance with $Y$ is $pq(M_1-M_0)$. Standardising that covariance gives:

$$
\frac{pq(M_1-M_0)}{\sqrt{pq}\,s_{Y,n}}
=\frac{M_1-M_0}{s_{Y,n}}\sqrt{pq}.
$$

So point-biserial is exactly the Pearson calculation for a binary indicator.

**Cross-questions that matter**

**Reverse the codes?** Yes = 0 and No = 1 gives $-0.9134$. The direction relative to the label coding reverses; the magnitude does not.

**Does zero point-biserial mean identical distributions?** No. Groups can have equal means but different spreads. For example, `[60,80]` and `[50,90]` both average 70, giving zero point-biserial despite different dispersion.

**Does $r_{pb}=1$ merely require all Yes marks to exceed all No marks?** No. For exact perfect correlation with a binary predictor and positive spreads, every outcome within each group must be constant at its group's distinct value. The earlier toy “means 86 and 72, balanced groups, overall SD 7” only permits $r=1$ when there is no within-group variation. Mere non-overlap is not enough.

**Must the binary variable be naturally binary?** It can be calculated for an observed 0/1 split, including an artificial cutoff. But dichotomising an underlying numerical variable loses information and changes the question. Biserial correlation is a different, assumption-dependent latent-variable idea, not an automatic replacement for every artificial split.

**When is it undefined?** If one group is absent, the binary variable has no variation. If all marks are identical, the outcome has no variation. Either causes a zero denominator.

**Memory:** **Binary + Numerical → Pearson on a 0/1 indicator → Point-biserial. Code the groups, compare means, match the SD formula.**

**Try it yourself**

1. Using M1 = 85.75, M0 = 71.25, p = q = 0.5 and divisor-n SD = √63, find rpb.
2. If the coding is reversed, and if the two groups instead have equal means, what happens respectively?

<details>
<summary>Answers and explanations — open after trying</summary>

1. rpb = (14.5/√63) × 0.5 = 7.25/√63 ≈ 0.9134.

2. Reversing codes reverses the sign only. Equal means give rpb = 0 when both groups and a nonconstant outcome are present; different group variances may still exist.

</details>

[Back to the topic index](#clickable-topic-index)


---
<a id="roadmap"></a>
## 7. Named but unfinished branches — Do not confuse a roadmap with a completed lesson

> **Coverage:** Named in the roadmap; the full lesson is still pending.

The following concepts appeared in our discussion or master tree. Some were only named as future topics. This section preserves them without replacing the requested notebook with an invented syllabus.

Our **user-supplied Week 3 list** is represented in the main lessons: Mean, Median, Mode, Quartiles, Percentiles, Range, Variance, Standard Deviation, IQR, and Five-Number Summary.

Our **user-supplied Week 4 list** is also represented: Contingency Tables, Relative Frequencies, Categorical Association, Scatterplots, Covariance, Pearson Correlation, and Point-Biserial Correlation.

This does not mean all of Statistics, or every branch ever named in the tree, is finished.

[Back to the topic index](#clickable-topic-index)


<a id="numerical-graphics-roadmap"></a>
### 7.1 Numerical graphs — Histogram, polygon, ogive, stem-and-leaf

> **Coverage:** Named in the roadmap; the full lesson is still pending.

**The remaining problem:** Numerical frequency tables organize marks, but how do we visualize the distribution's shape, cumulative pattern, and individual detail?

| Named concept | What it will help answer | Where we stopped |
|---|---|---|
| Histogram | How are numerical values distributed across intervals? | Contrasted with categorical bar charts; no full lesson yet |
| Frequency polygon | How does grouped frequency change across neighboring intervals? | Named in the master tree |
| Ogive | How many observations fall below or above a numerical threshold? | Named as a cumulative-frequency graph |
| Stem-and-leaf plot | How can we show a numerical distribution while retaining individual values? | Named in the master tree |
| Less-than / more-than cumulative frequency | How do cumulative totals depend on threshold direction? | The categorical ordered version was worked; the full numerical treatment is pending |

**One important histogram caution to carry forward:** With unequal bin widths, bar area should represent frequency (or proportion), so a frequency-density height is $f_i/h_i$, where $h_i$ is bin width. Equal-width histograms allow heights proportional to frequencies. Do not learn “all histogram heights always equal frequency” as a universal rule.

The natural school question for the full lesson is: “What pattern is hidden inside the marks table?”

[Back to the topic index](#clickable-topic-index)


<a id="index-dispersion-roadmap"></a>
### 7.2 Index of dispersion — Named, not yet developed

> **Coverage:** Named in the roadmap; the full lesson is still pending.

This term was present in the proposed master tree, but we did not work through a dedicated example or its intended model.

**The future question:** For count data such as daily absence counts, how large is the variance relative to the mean count?

One common count-data definition is:

$$
D=\frac{\operatorname{Var}(X)}{\operatorname{E}[X]},
\qquad\text{with sample analogue }\frac{s^2}{\bar{x}}.
$$

$\operatorname{E}[X]$ denotes the expected/mean count. This is **variance divided by mean**, not CV, which uses **SD divided by mean**. The term is used in more than one context, so the course's definition and reference model must be stated before interpreting thresholds.

A full lesson and the probabilistic reason for using this ratio remain pending. This is a vocabulary and formula preview, not a completed inference method.

[Back to the topic index](#clickable-topic-index)


<a id="inference-roadmap"></a>
### 7.3 Probability, sampling, estimation, and tests — The later branch

> **Coverage:** Named in the roadmap; the full lesson is still pending.

Our principal has described the observed school data. The next kinds of questions go beyond description:

> “How representative is this sample? How uncertain is the estimate? Is an observed difference larger than sampling variation would readily explain?”

```text
Probability foundations
├── Events, joint and conditional probability
├── Independence
└── Probability distributions

Sampling and inference
├── Population, sample, parameter, statistic       → introduced
├── Sampling methods and selection bias           → full lesson pending
├── Degrees of freedom and the n−1 derivation      → motivation introduced
├── Sampling distributions and standard error     → pending
├── Point estimation                              → named
├── Interval estimation / confidence intervals    → named
└── Hypothesis testing                            → named
    └── Chi-square association test               → expected-count preview only

Modelling extensions
├── Regression                                    → named, not taught fully
├── ANOVA                                         → mentioned as a later variance application
└── Biserial correlation                          → distinguished briefly from point-biserial
```

A **point estimate** supplies one sample-based estimate of a population quantity. An **interval estimate** supplies a range through a procedure whose uncertainty properties need explanation. A **hypothesis test** evaluates evidence relative to a stated model and assumptions. These descriptions are orientation, not a replacement for the future worked lessons.

We already used empirical conditional probabilities to read tables, but have not completed a full probability course. We saw expected counts $E_{ij}=R_iC_j/N$ under independence, but did not complete the chi-square statistic, degrees of freedom, or inference assumptions.

**Important:** A descriptive association, a significant test result, and a causal conclusion are three different claims. Later chapters should preserve that distinction.

[Back to the topic index](#clickable-topic-index)


---
<a id="rapid-revision"></a>
## 8. Rapid revision — Rebuild the story without rereading every paragraph

### 8.1 The question-to-tool map

| The principal's question | Tool / concept | Remember |
|---|---|---|
| What do these observations tell us? | Statistics | Data → understanding |
| What happened in this observed group? | Descriptive statistics | Describe what we have |
| What might be true beyond this group? | Inferential statistics | Sampling and uncertainty |
| Which operations have meaning? | Measurement scale | Name → order → equal gap → true zero |
| How many chose each category? | Frequency distribution | Count occurrences |
| What share chose each category? | Relative frequency | Count / relevant total |
| How many have we reached in order? | Cumulative frequency | Running total |
| Which category is larger? | Bar chart | Compare separate bars |
| How is one whole divided? | Pie chart | Shares of 360° |
| If all marks were shared equally? | Arithmetic mean | Preserve the total |
| Can calculation be simplified? | Assumed / step-deviation methods | Same mean, smaller numbers |
| What if contributions differ? | Weighted mean | More weight → more influence |
| How do I combine class averages? | Combined mean | Group sizes are weights |
| What constant factor gives the same endpoint? | Geometric mean | Preserve the product |
| What is average speed over equal distances? | Harmonic mean | Average reciprocals |
| What is the middle ordered value? | Median | Sort, then locate |
| What occurs most often? | Mode | Highest frequency |
| How wide is the whole span? | Range | Max − Min |
| How far away on average, ignoring direction? | Mean deviation | Average absolute distances |
| How large are squared distances? | Variance | Square, then average |
| Can spread return to original units? | SD | Square root of variance |
| Where are positional cut-points? | Quartiles / percentiles | Landmarks, not marks percentages |
| How wide is the middle half? | IQR | Q3 − Q1 |
| Can I see five checkpoints? | Five-number summary | Min, Q1, Median, Q3, Max |
| Is spread large relative to the mean? | CV | SD / Mean |
| Which two categories occur together? | Contingency table | Preserve the pairing |
| Within which group is this percentage? | Conditional relative frequency | “Among” chooses denominator |
| Does the distribution change across groups? | Categorical association | Compare conditional patterns |
| How do paired numerical values look? | Scatterplot | Direction, strength, form, outliers |
| Do deviations move together? | Covariance | Multiply paired deviations |
| Can joint movement be standardised? | Pearson correlation | Covariance / product of SDs |
| How does a binary group relate to marks? | Point-biserial correlation | Pearson with a 0/1 indicator |

### 8.2 Formula index

The notation and conditions are explained in the individual lessons. These formulas are reminders, not a substitute for choosing the correct question and denominator.

**Counts and categorical graphs**

$$
\sum f_i=n,\qquad RF_i=\frac{f_i}{n},\qquad \%_i=\frac{f_i}{n}\times100\%.
$$

$$
F_i=\sum_{j=1}^{i}f_j,\qquad \theta_i=\frac{f_i}{n}\times360^\circ.
$$

**Arithmetic mean and shortcuts**

$$
\bar{x}=\frac{\sum x_i}{n},\qquad\mu=\frac{\sum x_i}{N},\qquad
\bar{x}=\frac{\sum f_ix_i}{\sum f_i}.
$$

$$
d_i=x_i-A,\quad \bar{x}=A+\frac{\sum f_id_i}{\sum f_i}.
$$

$$
u_i=\frac{x_i-A}{h},\quad\bar{x}=A+h\frac{\sum f_iu_i}{\sum f_i}.
$$

$$
\bar{x}_w=\frac{\sum w_ix_i}{\sum w_i},\qquad
\bar{x}_c=\frac{\sum n_i\bar{x}_i}{\sum n_i}.
$$

**Multiplicative and rate means**

$$
GM=\left(\prod x_i\right)^{1/n},\qquad
g_{\mathrm{equiv}}=\left(\prod(1+g_i)\right)^{1/n}-1.
$$

$$
HM=\frac{n}{\sum(1/x_i)},\qquad HM(a,b)=\frac{2ab}{a+b},\qquad
\bar{v}=\frac{\sum d_i}{\sum d_i/v_i}.
$$

For positive inputs: $AM\ge GM\ge HM$, with equality when all values are equal. Equal-time average speed uses time-weighted AM, not automatically HM.

**Numerical median and position**

$$
M=x_{((n+1)/2)}\quad(n\text{ odd}),\qquad
M=\frac{x_{(n/2)}+x_{(n/2+1)}}2\quad(n\text{ even}).
$$

$$
Q_1=P_{25},\quad Q_2=P_{50}=M,\quad Q_3=P_{75},\quad D_k=P_{10k}.
$$

$$
PR_{<}(x)=100L/n,\qquad PR_{\le}(x)=100(L+E)/n.
$$

For percentile **values**, use the convention specified in [the percentile lesson](#percentiles), not the percentile-rank formulas above.

**Dispersion**

$$
R=\max-\min,\qquad MD_A=\frac{\sum|x_i-A|}{n},\qquad
MD_A=\frac{\sum f_i|x_i-A|}{\sum f_i}\text{ with frequencies}.
$$

$$
\sigma^2=\frac{\sum(x_i-\mu)^2}{N},\qquad
\sigma=\sqrt{\frac{\sum(x_i-\mu)^2}{N}}.
$$

$$
s^2=\frac{\sum(x_i-\bar{x})^2}{n-1},\qquad
s=\sqrt{\frac{\sum(x_i-\bar{x})^2}{n-1}}.
$$

$$
IQR=Q_3-Q_1,\quad QD=\frac{Q_3-Q_1}{2},\quad
CV=\frac{\sigma}{\mu}\times100\%\text{ or }\frac{s}{\bar{x}}\times100\%.
$$

$$
C_R=\frac{\max-\min}{\max+\min},\qquad
C_Q=\frac{Q_3-Q_1}{Q_3+Q_1}.
$$

The relative measures need an appropriate zero point and valid nonzero denominator.

**Five-number summary and outlier preview**

$$
(\min,Q_1,M,Q_3,\max),\qquad L=Q_1-1.5\,IQR,\quad U=Q_3+1.5\,IQR.
$$

**Contingency tables**

$$
R_i=\sum_jf_{ij},\quad C_j=\sum_if_{ij},\quad N=\sum_i\sum_jf_{ij}.
$$

$$
\text{Joint}=\frac{f_{ij}}{N},\quad
\text{Marginal}=\frac{R_i}{N}\text{ or }\frac{C_j}{N},\quad
\text{Row conditional}=\frac{f_{ij}}{R_i},\quad
\text{Column conditional}=\frac{f_{ij}}{C_j}.
$$

Under independence, for all relevant category pairs:

$$
P(Y=y\mid X=x)=P(Y=y),\quad
P(X=x,Y=y)=P(X=x)P(Y=y).
$$

$$
E_{ij}=\frac{R_iC_j}{N},\qquad\text{difference in proportions}=p_1-p_0.
$$

**Covariance and correlation**

$$
\operatorname{Cov}(X,Y)=\frac{\sum(x_i-\mu_X)(y_i-\mu_Y)}N,
\qquad
s_{XY}=\frac{\sum(x_i-\bar{x})(y_i-\bar{y})}{n-1}.
$$

$$
r=\frac{s_{XY}}{s_Xs_Y}
=\frac{\sum(x_i-\bar{x})(y_i-\bar{y})}
{\sqrt{[\sum(x_i-\bar{x})^2][\sum(y_i-\bar{y})^2]}}.
$$

$$
\rho=\frac{\operatorname{Cov}(X,Y)}{\sigma_X\sigma_Y},\qquad -1\le r,\rho\le1
$$

when the required variances are positive and finite.

**Point-biserial — match the SD denominator**

$$
p=\frac{n_1}{n},\quad q=\frac{n_0}{n},\quad
s_{Y,n}=\sqrt{\frac{\sum(y_i-\bar{y})^2}{n}}.
$$

$$
\boxed{r_{pb}=\frac{M_1-M_0}{s_{Y,n}}\sqrt{pq}}
$$

or, with the usual sample SD $s_Y$ computed with $n-1$:

$$
\boxed{r_{pb}=\frac{M_1-M_0}{s_Y}\sqrt{\frac{n_1n_0}{n(n-1)}}}.
$$

### 8.3 Symbols — Read the mathematics without guessing

| Symbol | Read it as | Meaning in this notebook |
|---|---|---|
| $x_i,y_i$ | x-i, y-i | Values for the same observation i |
| $x_{(i)}$ | i-th ordered x | The i-th value after sorting |
| $n,N$ | n, capital N | Sample/observed size; population or grand total as locally specified |
| $\bar{x},\bar{y}$ | x-bar, y-bar | Means of observed samples |
| $\mu,\mu_X,\mu_Y$ | mu | Population mean(s) |
| $\sum$ | sum / capital Sigma | Add the indicated terms |
| $\prod$ | product / capital Pi | Multiply the indicated terms |
| $\sigma,\sigma^2$ | sigma, sigma-squared | Population SD and variance |
| $s,s^2$ | s, s-squared | Usual sample SD and variance |
| $\lvert a\rvert$ | absolute value of a | Magnitude without sign |
| $\sqrt{a}$ | square root | Nonnegative square root for a ≥ 0 |
| $\sqrt[n]{a}$ | n-th root | A factor whose n-th power is a |
| $f_i$ | frequency i | Count of category/value i |
| $F_i$ | cumulative frequency i | Running total through ordered category i |
| $w_i$ | weight i | Influence / frequency / amount associated with value i |
| $A,d_i,u_i,h$ | reference, deviation, step deviation, step | Mean-shortcut notation; A is also a chosen center in MD when specified |
| $M,Q_1,Q_2,Q_3$ | median, quartiles | Positional landmarks |
| $P_k,D_k$ | kth percentile, kth decile | Position cut-points under a stated convention |
| $\lceil h\rceil$ | ceiling of h | Smallest integer at least h |
| $\theta_i$ | theta i | Pie-chart sector angle |
| $f_{ij}$ | frequency i-j | Count at row i, column j |
| $R_i,C_j,E_{ij}$ | row total, column total, expected count | Contingency-table notation |
| $P(A)$ | probability of A | Probability under the stated model or empirical selection |
| $A\cap B$ | A and B | Joint occurrence of events |
| $P(A\mid B)$ | probability of A given B | Conditional probability |
| $s_{XY}$ | sample covariance | Sample average-product estimate with n−1 divisor |
| $r,\rho$ | r, rho | Sample and population Pearson correlation |
| $r_{pb}$ | r point-biserial | Correlation for a binary-coded variable and numerical outcome |
| $M_1,M_0$ | mean one, mean zero | Outcome means of the two binary groups |
| $p,q$ | group proportions | n1/n and n0/n in the point-biserial lesson |
| $s_{Y,n}$ | Y SD using divisor n | Overall empirical SD needed in the compact point-biserial formula |

Symbols such as $R$ (range), $R_i$ (row total), $L$ (largest value in one coefficient), and $L$ (lower fence elsewhere) are context-dependent. Each lesson defines its local use. **Σ/∑ means add; σ means population SD.**

### 8.4 Memory map

```text
DATA
  → Which group? categorical
  → How much? numerical

SCALE
  → N-O-I-R: Name, Order, equal Intervals, Real zero

CENTER
  → Mean: equal share / balance
  → Median: middle position
  → Mode: most frequent

MEAN FAMILY
  → Direct: use the values
  → Assumed: shift and correct
  → Step deviation: shift, shrink, restore
  → Weighted: unequal influence
  → Combined: group sizes become weights
  → Geometric: multiply / compound
  → Harmonic: reciprocals; check equal distances vs equal times

SPREAD
  → Range: outer edges
  → MD: absolute distances
  → Variance: squared distances
  → SD: back to original unit
  → IQR: middle half
  → CV: spread relative to mean

POSITION
  → Q1, Median, Q3: three landmarks
  → Percentile: position, not percentage marks
  → Five-number summary: start, quarter, middle, three-quarters, end

ASSOCIATION
  → Cat + Cat: contingency table
  → Denominator: everyone, row, or column?
  → Same conditional distribution: independence pattern
  → Num + Num: scatterplot, covariance, Pearson
  → Binary + Num: point-biserial
  → Correlation ≠ causation
```

---
<a id="accuracy-notes"></a>
## 9. Clarifications to keep the notebook mathematically consistent

These are small corrections to earlier conversational shortcuts, not a change in the learning story.

1. **Marks above 100:** Earlier dispersion sketches used 104 or 110 without a different scoring scale. The worked comparisons use our later corrected `40,55,70,85,100` and C/D datasets. Generic values like 525 or 120 are explicitly labelled scale illustrations, not out-of-100 marks.
2. **Mean is not “wrong” when an extreme value changes it:** It still preserves the total. It may answer a different question from the intended “typical student” question.
3. **Grouped means:** Direct, assumed mean, and step-deviation agree for the same representative values. Midpoint-based means can still be approximations to raw data.
4. **Weighted examples must keep score-weight pairings:** The assignment/midterm/final example gives 82. Maths 80, Science 70, English 90 weighted 50%,30%,20% gives 79. They are different examples.
5. **Harmonic mean is not the answer to every rate question:** Equal distances give HM of speeds; equal times give AM. Total quantity divided by total time is the first principle.
6. **Median with ties:** At least half the observations are at or below a median, and at least half at or above. Exactly half strictly on either side is not guaranteed.
7. **Ordinal median:** Do not average arbitrary category codes when the central labels differ without stating additional assumptions or a convention.
8. **Quartiles and percentiles:** The calculation convention is explicit. Percentile rank and percentile value are not interchangeable formulas; ties matter.
9. **MAD ambiguity:** Mean absolute deviation and median absolute deviation are different. MD denotes the former here.
10. **SD interpretation:** SD is a root-mean-square scale, not the arithmetic mean of absolute distances and not a guaranteed fixed-percentage interval.
11. **Sample denominators:** Dividing by n describes an empirical mean squared deviation; n−1 is the usual variance-estimation correction under its sampling assumptions. Unbiased variance does not imply unbiased SD.
12. **CV:** Unitless does not mean meaningful for arbitrary scales. Zero must have the appropriate meaning, and means near zero are problematic.
13. **Five-number summary:** The actual 20-student mean is 65.35, not an exact 65. A five-number summary does not generally recover the mean or SD.
14. **Skewness shortcuts:** The usual mean–median–mode orderings are not universal identities.
15. **Box-plot whiskers:** A modified outlier-marking box plot need not extend to the actual minimum and maximum; it also need not end exactly at a fence.
16. **Sample association:** Different empirical percentages describe a pattern. They do not by themselves prove a population association, statistical significance, or causation.
17. **Pearson correlation:** It is undefined with zero variation in either variable. A zero coefficient does not exclude a nonlinear relationship; positive unit scaling and negative recoding affect signs differently.
18. **Point-biserial denominator:** The compact mean-difference formula with √(pq) uses divisor-n SD. The usual sample-SD formula needs √[n1n0/(n(n−1))]. The original tutoring example gives approximately **0.9134** using either matched form.
19. **Point-biserial scope:** It can be calculated for a defined 0/1 variable; artificial dichotomisation changes the question and loses information. Equal group means can give zero correlation even when the group distributions differ in spread.
20. **Point-biserial perfection:** Exact |r| = 1 with a binary variable requires constant outcomes within each group at two distinct levels, not merely a large mean difference or non-overlapping groups.

---
<a id="technical-references"></a>
## 10. Technical checks and source notes

The narrative, running examples, and educational questions come from our discussion. The sources below were used to check formula conventions and qualifications rather than replace the school storyline with textbook prose. Calculations in the worked examples were recomputed directly.

<a id="reference-s1"></a>
**S1 — NIST/SEMATECH, Measures of Scale.** Distinguishes variance, SD, average absolute deviation, median absolute deviation, range, and IQR; useful for the MAD naming clarification.

[Read the NIST reference](https://www.itl.nist.gov/div898/handbook/eda/section3/eda356.htm)

<a id="reference-s2"></a>
**S2 — R documentation, Sample Quantiles.** Documents multiple sample-quantile algorithms, including a stepwise method with averaging at discontinuities. Supports declaring a convention rather than treating different software answers as automatically wrong.

[Read the R reference](https://stat.ethz.ch/R-manual/R-devel/library/stats/html/quantile.html)

<a id="reference-s3"></a>
**S3 — NIST Dataplot, Coefficient of Variation.** Explains SD relative to mean, ratio-scale interpretation, and problems near zero or with arbitrary-zero scales.

[Read the NIST reference](https://www.itl.nist.gov/div898/software/dataplot/refman2/auxillar/coefvari.htm)

<a id="reference-s4"></a>
**S4 — SciPy, pearsonr.** Gives the centered-sums formula and describes constant-input undefinedness and the distinction between zero correlation and independence.

[Read the SciPy reference](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.pearsonr.html)

<a id="reference-s5"></a>
**S5 — SciPy, pointbiserialr.** States equivalence with Pearson correlation and gives the sample-SD formula containing √[n0n1/(n(n−1))]. This is the source check for the denominator correction; no inference-test formulas from that page are needed here.

[Read the SciPy reference](https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.pointbiserialr.html)

<a id="reference-s6"></a>
**S6 — NIST/SEMATECH, Box Plot.** Describes both basic min–max and fence-based outlier-marking forms, supporting the distinction between actual extremes, fences, and whisker endpoints.

[Read the NIST reference](https://www.itl.nist.gov/div898/handbook/eda/section3/boxplot.htm)

<a id="reference-s7"></a>
**S7 — NIST/SEMATECH, Measures of Skewness and Kurtosis.** Supports the terminology of symmetry, asymmetry, and long tails. Formal skewness and kurtosis calculations were not added as completed lessons.

[Read the NIST reference](https://www.itl.nist.gov/div898/handbook/eda/section3/eda35b.htm)

---

**Notebook continuity:** Add a new concept under its correct parent, preserve the school storyline, and record what new question makes it necessary. Do not mark a roadmap item completed until its explanation, example, formula where applicable, interpretation, and practice have actually been developed.
