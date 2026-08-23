# ARWG Agent Adoption, Accuracy & Reliability Survey

This is the platform-neutral review source for the AAIF/Agentic AI Foundation Accuracy & Reliability Working Group survey. It records the current 16-question survey and the behavior a fielded survey must preserve, independent of implementation platform.

## Review status

- The question stems, answer choices, factor rows, and ordered scales below incorporate the current review decisions.
- Reviewers should flag unclear wording, missing response paths, analytical problems, or implementation risks in line comments. Proposed content changes should be discussed explicitly rather than silently incorporated.
- Survey-platform selection, privacy and aggregation language, analysis procedures, and deployment configuration are outside this document's current scope.

## Reading the response specifications

- **Single select:** exactly one listed answer may be selected.
- **Multi-select:** one or more listed answers may be selected unless an exclusive choice is specified.
- **Single-response matrix:** exactly one scale answer is selected for each factor row.
- **Inline text:** a short text field appears beside the answer choice and is required only when that choice is selected.
- **Display order:** fixed as listed in this survey. Any later randomization must preserve ordered scales and the placement of terminal choices such as “None,” “Something else,” and “Not sure.”

## Entry and anchor

### Q1. Eligibility and real-world use

- **Response:** Single select
- **Required:** Yes
- **Behavior:** The first five choices continue to the survey. The final three choices end the survey and record the response as screened out.

**During the past six months, which best describes your firsthand experience with AI agent systems?**

If more than one system reached real-world use, answer about the one you worked with most. If two qualify equally, choose the one you worked with most recently.

- Serious pilot: Being tried with real data or intended users for real work, but not yet part of normal work
- Limited deployment: Part of normal work for some intended users or workflows
- Broad deployment: Part of normal work for most intended users or workflows
- Paused or retired: Previously reached a serious pilot or deployment
- Real-world use, stage not sure: Used for real work, but I am not sure which stage fits
- Demo, prototype, or generic research only: No system reached real-world use
- Secondhand knowledge only: Knew about a system used for real work but did not personally work with it
- No relevant system experience

**Focal-system instruction**

For the rest of this survey, answer about the same system you had in mind for Q1 and your experience with it during the past six months. When a question asks about the system or organization at a particular point, answer based on the last time you worked with it.

### Q2. Direct activities

- **Response:** Multi-select
- **Required:** Yes

**Which activities have you personally performed with this system during the past six months? Select all that apply.**

- Designed, built, configured, or integrated it
- Tested or evaluated its quality
- Deployed, operated, monitored, or investigated it
- Reviewed, corrected, or approved its outputs or actions
- Used its outputs or relied on its actions in my work
- Made product or operational decisions using firsthand evidence about it

### Q3. Primary area of work

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**Which area of work was this system’s primary use? Choose the closest answer.**

- Customer or employee service
- Research and knowledge work
- Content and creative work
- Software engineering or IT operations
- Data, document, or administrative processing
- Analysis, planning, or decision support
- Risk, compliance, quality, or evaluation
- Business operations or transactions
- Something else (describe briefly)
- Not sure

### Q4. System structure

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**Which best describes how this system completed a typical task? Choose the closest answer.**

- A single AI response: Produced an answer, draft, or label from information supplied to it without choosing subsequent steps, calling other software, or taking actions
- One AI agent: Chose the steps needed to complete the task and could search, run code, call other software, or update records without handing work to another AI agent
- Multiple AI agents: Two or more AI agents coordinated, delegated, handed off, or checked one another’s work
- A preset automated workflow with AI steps: AI performed one or more steps in a preprogrammed sequence, while software or fixed rules determined what happened next
- Something else (describe briefly)
- Not sure

### Q5. Organization size

- **Response:** Single select
- **Required:** Yes

**Approximately how many employees or regular staff worked at the organization where this system was primarily used for real work? If you worked with it for a client or customer, answer about that organization rather than your own.**

- 1 to 99
- 100 to 999
- 1,000 or more
- The system was used across several organizations or customers (no single organization applies)
- Not sure
- Prefer not to answer

## Adoption and general concerns

### Q6. Constraints

- **Response:** Single-response matrix
- **Required:** Yes; one response for every factor row
- **Row order:** Fixed as listed
- **Scale order:** Fixed as listed

**During the past six months, how much did each factor limit progress or expansion of this system?**

Factors:

- Unclear value or fit with the intended work
- Financial or computing cost of building and running the system
- Response time or ability to handle the required volume
- Access to or integration with required data, tools, or systems
- Security, privacy, legal, or compliance requirements
- Gaps in staffing, skills, or operational ownership
- Low user trust or willingness to adopt
- The system’s results or actions were not accurate or useful enough
- The system did not behave reliably across repeated use or changing conditions
- Insufficient evidence to determine or demonstrate whether the system worked well enough

Scale:

1. Not a limitation
2. Present, but did not slow progress
3. Slowed progress somewhat
4. Slowed progress substantially
5. Stopped or reversed progress
6. Not enough visibility

### Q7. Human checking

- **Response:** Single select
- **Required:** Yes
- **Display order:** Fixed as listed

**During the past six months, which best describes how meaningful human checking was applied to this system’s outputs or actions before they were relied on or allowed to stand?**

- No routine human checking
- Occasional spot checks
- Checking mainly when the system flags uncertainty
- Checking mainly for high-risk cases
- Most or all outputs received a substantive review
- Practices varied too much to identify one pattern
- Not enough visibility

### Q8. Most significant benefit

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**During the past six months, what was the most significant benefit this system delivered in real work?**

- Completed roughly the same work faster or with less effort
- Handled more work, cases, or users
- Improved the quality or consistency of work
- Enabled work that was previously impractical or impossible
- Improved responsiveness or availability
- Produced no meaningful additional benefit
- Too early to tell
- Something else (describe briefly)
- Not enough visibility

## Accuracy and reliability

### Q9. Frequency of unacceptable results

- **Response:** Single select
- **Required:** Yes
- **Scale order:** Fixed as listed

**During the past six months, when this system was used for real work, roughly how often did it produce a result or action that was unacceptable for its intended use?**

- Never or almost never
- Rarely (a small minority of uses)
- Sometimes, but not in most uses
- Often (a substantial share of uses)
- In most or almost all uses
- Varied too much across tasks to answer
- Not enough visibility or use to answer

### Q10. Accuracy and reliability factors

- **Response:** Single-response matrix
- **Required:** Yes; one response for every factor row
- **Row order:** Fixed as listed
- **Scale order:** Fixed as listed

**During the past six months, how much did each of the following accuracy or reliability problems affect the system’s usefulness or continued use?**

Factors:

- Incorrect, misleading, or unusable results or actions
- Different results or actions under materially similar conditions
- Failure to follow an instruction, requirement, or limit
- Failure when inputs, context, or operating conditions changed
- Failure when a tool, data source, or dependency changed or broke
- Failure to flag uncertainty or involve a person when needed

Scale:

1. Did not encounter this
2. Encountered it, but with little or no effect
3. Reduced usefulness somewhat
4. Reduced usefulness substantially
5. Caused use to be restricted, paused, or stopped
6. Not enough visibility

### Q11. Recognition before impact

- **Response:** Single select
- **Required:** Yes
- **Scale order:** Fixed as listed

**During the past six months, among the unacceptable results or actions you know about, how often was the problem recognized before it affected real work?**

- Every or almost every time
- Most of the time
- About half the time
- Some of the time, but fewer than half
- Few or none of the time
- No unacceptable results or actions were known
- Not enough visibility

### Q12. Most serious consequence

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**During the past six months, what was the most serious consequence you know occurred because of an accuracy or reliability problem with this system?**

- No accuracy or reliability problem was known
- The problem was corrected before affecting real work
- Work was delayed, repeated, or abandoned
- A customer, employee, or other user received an inadequate outcome
- A decision, record, or system action had to be corrected or reversed
- Substantial additional cost or direct financial loss occurred
- A security, privacy, legal, compliance, or safety issue occurred
- Use of the system was restricted, paused, or stopped
- Something else (describe briefly)
- Not enough visibility

### Q13. Primary quality evidence

- **Response:** Single select
- **Required:** Yes

**During the past six months, which source of evidence had the greatest influence on decisions about whether this system’s quality was acceptable?**

- Informal human judgment or spot checks
- A repeatable collection of examples or test cases
- Defined measures or acceptance thresholds
- Production monitoring or incident evidence
- Real-world user, task, or business outcomes
- No consistent approach
- Not enough visibility

## Priorities and close

### Q14. Shared-industry priority

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**Based on your experience with this system, which accuracy or reliability problem most needs shared industry work?**

- Defining what “acceptable quality” means for a particular use
- Evaluating representative end-to-end tasks and workflows
- Measuring consistency across repeated or similar situations
- Detecting regressions after systems change
- Handling failures in tools, data, or dependencies
- Managing uncertainty and involving people at the right time
- Detecting and learning from production failures
- Something else (describe briefly)
- No shared industry work is needed
- Not sure

### Q15. Preferred ARWG output

- **Response:** Single select
- **Required:** Yes
- **Inline text:** Required when “Something else (describe briefly)” is selected.

**Which one vendor-neutral ARWG output would most help people working with systems like this one?**

- Shared, plain-language terminology for failures
- Practical guidance on metrics and evaluation design
- Reusable tests, evaluation tools, or test cases
- Reliability design and human-handoff patterns
- Monitoring and incident-learning guidance
- Worked examples and case studies
- A quality or conformance framework
- Something else (describe briefly)
- None of these
- Not sure

### Q16. Optional close

- **Response:** One short text response
- **Required:** No

**Optional: What important accuracy or reliability problem or experience did this survey miss?**
