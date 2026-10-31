# Method library contract

A library is an external, evolving knowledge source consumed by this skill. It can be a repository, supplied files, or an accessible knowledge base. Keep project-specific data outside the generic skill so a growing library does not require rewriting the procedure.

## Index

Maintain an index connecting a stable method ID and version to its record, the decision it helps make, applicability, exclusions, and review state. Focus categories help find relevant evidence; they are many-to-many with methods. Several papers may support one method, and one paper may inform several methods. Do not generate one skill per paper or make the number of papers a maturity score.

Prefer stable source IDs such as DOI/arXiv identifiers, with resolvable note links or a registry. Follow the registry's current note path when sources move. Preserve paper versions and the library revision used for a decision. New or unmapped categories remain research leads until their evidence supports a conditional method.

## Minimum useful method record

Adapt this shape to the project's existing format:

- **Identity:** stable ID, version, title, date, and links to revisions it replaces.
- **Decision:** the specific choice or uncertainty the method addresses.
- **Applicability:** required task structure, data, feedback, resources, and assumptions; explicit exclusions or missing prerequisites.
- **Rule and mechanism:** if these conditions hold, compare or do this, because of this proposed mechanism. Include what remains an inference.
- **Evidence:** source/work ID and version; exact claim and locator; access level; study setting and comparison; what it supports and what it does not. Experimental records additionally identify data/code/config versions, measurements, and uncertainty.
- **Alternatives and limits:** credible competing explanations or designs, contradictory observations, failure cases, and transfer gaps.
- **Test:** a discriminating comparison, important controls, practical success/failure criteria, and observations that would revise the method.
- **Status:** lifecycle (`proposed`, `active`, `rejected`, `superseded`); independent review (`pending`, `reviewed`, `changes-requested`, with evidence and reviewed version); and local adoption (`unassessed`, `trial`, `adopted`, `declined`, scoped to a project/decision).
- **History:** what changed, why, confidence rationale, reviewer if actually reviewed, and supersession links.

An `active` method must have a recorded independent or human review of the stated version and scope. A proposed method can still inform an explicitly provisional decision. Adoption records reflect actual user/project choices, not the author's hope. An abstract, a full paper, and a reproduced experiment describe different access/evidence states; none is an automatic quality grade. Older personal-principle statuses such as `human-confirmed` do not substitute for scientific review.

## Decision and outcome records

Keep enough context to revisit a decision: problem and constraints; method IDs/versions and library revision; alternatives considered; evidence and transfer assumptions; recommendation; proposed test; what would change it; decision/adoption status. Later append the actual outcome, deviations from the plan, and resulting method revision. Label planned experiments separately from executed ones.

Store sensitive data and human reflections according to the destination's existing privacy policy. Public records should be independently understandable without copying private transcripts or account routing information.
