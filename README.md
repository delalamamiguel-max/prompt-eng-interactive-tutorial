# Welcome to Anthropic's Prompt Engineering Interactive Tutorial

## Course introduction and goals

This course is intended to provide you with a comprehensive step-by-step understanding of how to engineer optimal prompts within Claude.

**After completing this course, you will be able to**:
- Master the basic structure of a good prompt 
- Recognize common failure modes and learn the '80/20' techniques to address them
- Understand Claude's strengths and weaknesses
- Build strong prompts from scratch for common use cases

## Course structure and content

This course is structured to allow you many chances to practice writing and troubleshooting prompts yourself. The course is broken up into **9 chapters with accompanying exercises**, as well as an appendix of even more advanced methods. It is intended for you to **work through the course in chapter order**. 

**Each lesson has an "Example Playground" area** at the bottom where you are free to experiment with the examples in the lesson and see for yourself how changing prompts can change Claude's responses. There is also an [answer key](https://docs.google.com/spreadsheets/d/1jIxjzUWG-6xBVIa2ay6yDpLyeuOh_hR_ZB75a47KX_E/edit?usp=sharing).

Note: This tutorial uses our smallest, fastest, and cheapest model, Claude 3 Haiku. Anthropic has [two other models](https://docs.anthropic.com/claude/docs/models-overview), Claude 3 Sonnet and Claude 3 Opus, which are more intelligent than Haiku, with Opus being the most intelligent.

*This tutorial also exists on [Google Sheets using Anthropic's Claude for Sheets extension](https://docs.google.com/spreadsheets/d/19jzLgRruG9kjUQNKtCg1ZjdD6l6weA6qRXG5zLIAhC8/edit?usp=sharing). We recommend using that version as it is more user friendly.*

When you are ready to begin, go to `01_Basic Prompt Structure` to proceed.

## Table of Contents

Each chapter consists of a lesson and a set of exercises.

### Beginner
- **Chapter 1:** Basic Prompt Structure

- **Chapter 2:** Being Clear and Direct  

- **Chapter 3:** Assigning Roles

### Intermediate 
- **Chapter 4:** Separating Data from Instructions

- **Chapter 5:** Formatting Output & Speaking for Claude

- **Chapter 6:** Precognition (Thinking Step by Step)

- **Chapter 7:** Using Examples

### Advanced
- **Chapter 8:** Avoiding Hallucinations

- **Chapter 9:** Building Complex Prompts (Industry Use Cases)
  - Complex Prompts from Scratch - Chatbot
  - Complex Prompts for Legal Services
  - **Exercise:** Complex Prompts for Financial Services
  - **Exercise:** Complex Prompts for Coding
  - Congratulations & Next Steps

- **Appendix:** Beyond Standard Prompting
  - Chaining Prompts
  - Tool Use
  - Search & Retrieval

---

# Owned checkout guide

## Purpose and status

This owned learning-reference fork preserves Anthropic’s prompt-engineering course above. It provides notebooks and exercises, not a production application. Model comparisons, pricing language and availability statements in the retained course introduction are historical course context, not verified current recommendations.

## Repository map

[`Anthropic 1P/`](Anthropic%201P/) contains direct Anthropic API lessons and exercise helpers. [`AmazonBedrock/`](AmazonBedrock/) contains its own README, requirements, license and contribution guidance, plus anthropic-SDK and boto3 notebook tracks, utilities and a CloudFormation workshop template. There is no root application manifest or standalone root license.

## Architecture and integrations

Direct-API lessons construct an Anthropic client and issue messages requests. Bedrock tracks use AnthropicBedrock or boto3 bedrock-runtime invocation. Exercise evaluation and playground cells can send prompts to providers; reading notebooks as files does not require execution. The optional workshop template defines IAM, KMS and a SageMaker notebook instance.

## Setup and environments

Choose the intended provider track before any future setup. Direct API lessons require Anthropic credentials; Bedrock lessons require appropriate AWS access, region and model permissions. The [Bedrock requirements](AmazonBedrock/requirements.txt) pin older SDK versions; compatibility is unverified. No packages were installed, notebooks opened in an executing kernel, credentials supplied or accounts configured during this review.

## Safe commands

For this documentation review, use only local inspection such as `git status --short`, `git ls-files`, `git diff -- README.md` and `git diff --check`. Read referenced scripts as text; do not install dependencies, execute examples, authenticate, run tests or publish. Do not use Run All, notebook install cells, provider calls or the CloudFormation template as documentation validation.

## Testing and validation

Only README structure, newly added local links, whitespace and preservation were checked. No exercise grading, notebook execution, model availability or external answer-key/Sheets links were tested. Existing output cells demonstrate prior examples and do not establish reproducibility today.

## Deployment and rollback

The course can be studied locally; the Bedrock workshop includes optional cloud provisioning, not an owner deployment record. CloudFormation can create billable resources and IAM permissions. Reverting notebooks does not tear down cloud resources or undo provider charges. No deployment or resource cleanup was attempted here.

## Risks and guardrails

Preserve course attribution, links and the [AmazonBedrock license](AmazonBedrock/LICENSE), which states MIT No Attribution. Do not assume that subdirectory license establishes terms for every file in the repository. Keep API keys, AWS credentials and private exercise inputs/outputs out of shared notebooks; example execution can incur usage.

## Related documentation

Use the course sequence above, [Bedrock README](AmazonBedrock/README.md), [Bedrock contributing guide](AmazonBedrock/CONTRIBUTING.md), [requirements](AmazonBedrock/requirements.txt) and [license](AmazonBedrock/LICENSE).
