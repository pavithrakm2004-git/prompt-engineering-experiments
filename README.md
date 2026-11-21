# Prompt Engineering Experiments

## Overview

This repository contains practical experiments exploring different prompt engineering techniques using **Google Gemini 3.8 Flash** through Google AI Studio.

The main goal of this milestone was to understand how the design of a prompt influences the quality, accuracy, consistency, and structure of AI-generated responses.

All experiments were performed without writing code, using different prompts and comparing the model's actual outputs.

## Tools and Configuration

- **Platform:** Google AI Studio
- **Model:** Gemini 3.8 Flash
- **Model ID:** `gemini-3.8-flash`
- **Temperature:** 0.2
- **Approach:** No-code experimentation

## Experiments

### 1. Zero-shot vs Few-shot Prompting

Compared sentiment classification with and without examples.

- **Task:** Classify a customer review as Positive, Negative, or Neutral.
- **Zero-shot:** The model identified mixed sentiments but did not return a single category.
- **Few-shot:** After receiving three examples, the model returned `Positive` in the required format.

**Key finding:** Providing examples helped the model follow the expected output format in this test.

### 2. Direct Prompting vs Step-by-Step Prompting

Compared two approaches to solving a mathematical problem involving a discount and GST.

- **Direct prompting:** Asked the model to return only the final amount.
- **Step-by-step prompting:** Asked the model to show the intermediate calculations.

**Result:** Both approaches produced the correct final amount of ₹53,100.

**Key finding:** Step-by-step prompting made the calculation easier to understand and verify, although it did not improve accuracy in this particular test.

### 3. Structured Output Prompting

Tested information extraction using a predefined JSON structure.

The model was asked to extract:

- Name
- Date
- Amount

Five different text inputs were tested.

**Result:** All five outputs contained valid JSON and correctly extracted the required information.

**Success Rate: 100% (5/5 tests)**

## Key Learnings

Through these experiments, I learned that:

- Examples can help guide a model toward the expected response format.
- Clear and specific instructions are important for reliable outputs.
- Step-by-step prompting can make multi-step solutions easier to verify.
- Defining a JSON structure helps maintain consistency in information extraction.
- AI-generated responses should always be evaluated rather than accepted without checking.

## Project Files

- `Prompt_Engineering_Report.docx` – Detailed experiment report, prompts, actual model outputs, and analysis.
- `Prompt_Engineering_Report.pdf` – Final report in PDF format (if included).

## Conclusion

These experiments provided practical experience in designing, testing, and evaluating prompts for a Large Language Model. They also helped me understand that effective prompt engineering is not just about asking questions, but about giving clear instructions and evaluating whether the model follows them correctly.

---

**Experimented using Google AI Studio and Gemini 3.8 Flash.**
