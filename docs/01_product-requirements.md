# Product Requirements Document


## Problem

[Who has the problem? What is difficult for them today? Alternatively, what need do you see this fulfilling in which user group?]

Individuals looking for a private, quick, low stress way to check in on their mental health and depressive symptoms using standarized clinical questions (PHQ-9) directly from their terminal without accounts or cloud tracking.
Existing wellness trackers are bloated, cloud-connect, or require sign-ups, and when someone is stressed, they need a fast, private, distraction-free tool.

## Desired outcome

[What should be better or more interesting for users when this is done?]

Users can run a terminal script, complete a streamlined PHQ-9 questionnaire with 0-3 scoring, see their evaluated severity tier, and receive immediate support ranging from randomized grounding/coping prompts to crisis resources readily available.

## Scope

[Which users, use cases, and features will this app cover?]

Users: Command-line users, students, and solo operators
Use Cases:
- Answering the PHQ-9 questionnaire items via terminal prompts with 0-3 integer validation
- Calculating total scores and severity tiers automatically
- Receiving randomized coping mechanisms using Python's random module.
Features: 
- PHQ-9 questionnaire bank and 0-3 input validation
- Score summation and severity classification
- Conditional routing to crisis hotlines or randomized coping prompts (random.choice()).
- Command-line argument handling (sys.argv) for quick launch options.

## Out of Scope

[What features is this app specifically avoiding?]

- Medical diagnosis, clinical therapy replacement, or external database storage

## Requirements


### The product must

- Administer the PHQ-9 questions and validate 0-3 integer inputs.
- Calculate the total score and map it to a severity category.
- Display immediate support or crisis resources based on score tier.
- Utilize standard Python libraries (statistics, random, and sys) with a main() guard (if _name_ == "_main_":).

### The product should

- Handle bad user inputs flawlessly without crashing
- Support optional command-line arguments via sys.argv.

### The product could

- Provide crisis information if prompted
- Direct user to nearest crisis facility that's local
