# The Bitter Lesson

- Author: Richard S. Sutton (essay signed Rich Sutton)
- Date: 2019-03-13
- Type: research-methodology essay
- Canonical source: http://www.incompleteideas.net/IncIdeas/BitterLesson.html
- Accessible copy inspected: https://www.cs.utexas.edu/~eunsol/courses/data/bitter_lesson.pdf
- Selection: explicitly chosen by the human on 2026-10-30 as a key methodology
- Status: foundational reference selected; the operational checklist below is a proposal

## Source argument

Sutton argues that general methods able to exploit increasing computation have repeatedly outperformed approaches built around extensive human domain knowledge. He highlights search and learning, drawing examples from games, speech, and vision. The methodological implication is to favor approaches whose capabilities can grow as resources grow, rather than assuming today’s compute budget is permanent. This is a historical argument and research heuristic, not a theorem guaranteeing that scale wins every comparison.

## Proposed use in this reading club

For each major research proposal, ask:

1. What improves when compute, data, interaction, or search budget increases? What evidence demonstrates the trend?
2. Which components are learned, searched, or fixed by a human? Which fixed choices may become bottlenecks?
3. What is the simplest scalable baseline, and is the comparison fair at matched budgets?
4. Does a specialized component improve the practical resource frontier, or only a narrow benchmark?
5. Can the system acquire knowledge through feedback, and what observation could falsify the proposal?

## Scope and limits of our application

Treat latency, data quality, feedback availability, energy, and deployment constraints as explicit experimental conditions. A hand-designed prior may be useful at a particular budget; test its benefit rather than rejecting it by slogan. Scaling predictive accuracy does not establish causal validity, and a fluent generated explanation does not establish understanding.

This checklist is our proposed interpretation for research decisions. The human selected the source; they have not yet confirmed every checklist item as a personal principle.
