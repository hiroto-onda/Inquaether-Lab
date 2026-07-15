# BlueDot Impact Rapid Grant 2026
## Authoritative Submission Record

Submission status:
Submitted

Submission date:
2026-07-15

Applicant name:
Hiroto Onda

Applicant email:
inquaetherlab@gmail.com

Where can we learn more about you?
https://github.com/hiroto-onda

Grant type:
Compute & research tools

What are you working on?
A small-scale HAI safety study using Prototype Exogram to observe how people attribute agency, intent, and capability to AI responses.

Link to your work:
https://github.com/hiroto-onda/lumenia-exogram

Public sharing:
Can share publicly with my name

Public URL:
https://github.com/hiroto-onda

How are you connected to the BlueDot community?
Other

How much funding are you requesting?
$400

Tell us more about your project:
This project will run a small-scale human–AI interaction safety study examining how people attribute agency, intent, and capability to AI responses.

The study will compare observable features of AI outputs with the interpretations assigned to them by human evaluators. Prototype Exogram will be used as a structured observation and logging tool, rather than as an automated judge.

I plan to evaluate approximately 20–50 dialogue samples and develop a preliminary observation model, evaluation rubric, and short public report. The goal is to identify recurring patterns in how AI response structures may encourage over-attribution or misattribution, and to produce a practical foundation for further research on safer human–AI interaction.

What have you already done?
I have already developed Prototype Exogram as a working, open-source research prototype for structured observation and logging of human–AI interactions.

The current system includes sample input handling, an ExogramCore processing layer, JSONL storage, SC-log conversion, a CLI viewer, and human-readable observation output. The implementation has been migrated to a clean virtual environment, runs without PYTHONPATH workarounds, and currently passes 370 regression tests.

Unsafe or authority-related functions are intentionally not connected, and output boundaries have been preserved. The prototype is therefore ready to support a small-scale evaluation study without requiring major new development.

What specifically would this grant fund?
$250 in API credits for generating and evaluating 20–50 human–AI dialogue samples across multiple model conditions.

$100 for participant or evaluator compensation, subject to recruitment needs, for structured annotation of agency, intent, and capability attributions.

$50 for cloud storage, documentation, and publication of the evaluation rubric, observation model, and public report.

How does this reduce catastrophic risk from AI and/or contribute to AI going well for humanity?
As AI systems become more fluent and socially persuasive, people may infer more agency, intent, understanding, or capability than the system actually has. These misattributions can contribute to over-trust, inappropriate delegation, reduced human oversight, and poor decisions in higher-stakes settings.

This project will develop a small, practical method for comparing observable AI output features with the interpretations assigned by human evaluators. By identifying recurring patterns that encourage over-attribution or misattribution, the study can support safer interface design, clearer communication of system limitations, and better human oversight.

The project does not claim to directly reduce catastrophic risk on its own. Its contribution is to build an empirical foundation for understanding a human–AI interaction failure mode that may become more important as AI systems become more capable and widely deployed.

What would you do without this grant?
Without this grant, I would continue the project at a much smaller and slower scale using free or self-funded resources. I would likely reduce the number of dialogue samples, rely on fewer model conditions, and limit or postpone external evaluator participation.

The project would not necessarily be abandoned, but the resulting evidence would be narrower and less reliable. The grant would allow me to run a more complete pilot now, compare multiple conditions, include structured human evaluation, and publish a clearer and more reusable set of methods and findings.

What makes you think this project will be successful? Why you? Why now?
The project is deliberately small, concrete, and technically ready to begin. Prototype Exogram is already implemented as an open-source observation and logging system, with 370 regression tests passing and key safety boundaries preserved. This means the grant would support evaluation work rather than speculative development.

I am an independent researcher focused on human–AI interaction, interpretation, agency attribution, and cognitive support. My work has centered on separating observable system structure from the meanings and intentions that people assign to AI responses, which is the core question of this pilot.

Now is a useful time to run the study because increasingly fluent and socially persuasive AI systems are being adopted faster than our understanding of how users interpret them. A small empirical pilot can produce an evaluation rubric, initial evidence, and reusable methods quickly, while the research prototype is stable and the scope remains manageable.

Feedback:
Not provided

Can we share your application with other funders and/or grantmakers?
Yes

## Record Authority

This document records the application content submitted on 2026-07-15.

It is the authoritative internal record for this submission.

Any future proposal, public summary, retrospective, or derivative document should remain distinguishable from the text recorded here.

Do not silently revise this file to reflect later changes in the project.
