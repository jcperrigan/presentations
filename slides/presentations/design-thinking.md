<!-- .slide: class="title-slide" -->

# Design Thinking in Teaching

Jessica Perrigan

University of Nebraska at Omaha

Notes:
Welcome everyone and briefly introduce my background.

---

## What is design thinking?
### And how can we use it to

A structured process for:

<ul>
<li class="fragment">Identifying a meaningful problem</li>
<li class="fragment">Designing an intervention</li>
<li class="fragment">Evaluating its effects</li>
<li class="fragment">Improving it through iteration</li>

</ul>
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
