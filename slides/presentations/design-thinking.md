<!-- .slide: class="title-slide" -->

# Design Thinking in Teaching

Jessica Perrigan

University of Nebraska at Omaha

Notes:
Your first year is not too early to think about promotion—but that doesn’t mean trying to manufacture an impressive CV immediately. It means making choices now that will produce evidence, expertise, and a coherent professional story later. In industry, we would not say, “I worked very hard on this process and people seemed to like it.” We would identify a problem, develop a product or intervention, test it, collect evidence, and improve it. Instructional design can work the same way. The goal here is for you to walk out with a plan for detecting, investigating, and documenting one potential student-learning problem during their first year.

---

## What is design thinking?
### And how can we use it to improve student learning?

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

<ul>
<li class="fragment">1. Identify the problem</li>
<li class="fragment">2. Understand how the students experience it</li>
<li class="fragment">3. Design a strategy</li>
<li class="fragment">4. Measure progress</li>
<li class="fragment">5. Iterate</li>
<li class="fragment">6. Document the results</li>
</ul>
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
