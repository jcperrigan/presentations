<!-- .slide: class="title-slide" -->

# Design Thinking in Teaching

Jessica Perrigan

University of Nebraska at Omaha

Notes:
Welcome everyone and briefly introduce my background.

---

## What is design thinking?

A structured process for:

- Identifying a meaningful problem
- Designing an intervention
- Evaluating its effects
- Improving it through iteration

Notes:
Emphasize that the process begins with the problem rather than with a favored instructional tool.

---

## The basic process

1. Identify the problem
2. Understand the people experiencing it
3. Design a strategy
4. Measure progress
5. Iterate
6. Document the results

---

## An empirical claim

An instructional intervention implicitly claims:

$$
E[Y_i \mid D_i = 1] > E[Y_i \mid D_i = 0]
$$

where $D_i$ indicates exposure to the intervention.

Notes:
This is not necessarily a literal causal-estimation exercise. The point is that adopting an intervention implies an expected improvement.

---

## Two kinds of evidence

<div class="columns top">
<div>

### Direct evidence

- Student work
- Assessment results
- Error patterns
- Completion behavior

</div>

<div>

### Indirect evidence

- Student surveys
- Confidence
- Perceived usefulness
- Instructor observations

</div>
</div>

---

## Example code

```r
model <- lm(
  exam_score ~ intervention + prior_gpa,
  data = students
)

summary(model)
