# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarization.

## Scenario:
You are part of a content curation team for an educational platform that delivers quick summaries of research papers to undergraduate students. Your task is to summarize a 500-word technical article on "The Basics of Blockchain Technology" using multiple AI platforms and prompting strategies.

Your goal is to determine which combination of prompting technique + platform provides the best summary in terms of:

Accuracy

Coherence

Simplicity

Speed

User experience

## Algorithm
### ChatGPT:
#### Prompting Techniques
##### 1.Zero-Shot Prompting
The model receives only the instruction without examples.

Example Prompt:

Summarize the following article on blockchain technology in 100 words for undergraduate students.

Advantages
Fastest method
Minimal effort
Good for straightforward tasks
Disadvantages
Output style may vary
May omit important details
##### 2.Few-Shot Prompting
The model is given sample summaries before the task.

Example Prompt:

Here are two examples of simple technical summaries. Use the same style to summarize this blockchain article in 100 words.

Advantages
More consistent structure
Improved clarity and simplicity
Disadvantages
Requires preparation of examples
Slightly slower than zero-shot

##### 3.Chain-of-Thought Prompting

The model is asked to reason step-by-step before summarizing.

Example Prompt:

Identify the main concepts, explain their relationships, and then write a concise summary for undergraduate students.

Advantages
Excellent accuracy
Captures deeper understanding
Disadvantages
Longer response time
May produce overly detailed outputs

##### 4.Role-Based Prompting

The model is assigned a specific role.

Example Prompt:

You are a university professor explaining blockchain technology to first-year engineering students. Summarize the article in 100 words.

Advantages
Highly readable and educational
Tailored to audience needs
Disadvantages
Slightly more verbose
Depends on how well the role is defined

#### Evaluation Criteria
Criterion	Description
Accuracy	Correct representation of technical concepts
Coherence	Logical flow and readability
Simplicity	Ease of understanding for students
Speed	Time taken to generate summary
User Experience	Overall usefulness and satisfaction

### Gemini:
#### 1. Zero-Shot Prompting
The Strategy: Asking the AI to summarize the 500-word blockchain article with no prior examples or detailed instructions.

Best Platform: Claude 4.6 Opus

Performance:

Accuracy: High; Claude is excellent at staying true to the source text without adding "fluff."

Coherence: Superior; it produces the most fluid, "human-sounding" paragraphs.

Simplicity: Good, though it can sometimes lean toward more sophisticated vocabulary.

Speed: Moderate.

User Experience: Best for quick, one-off summaries where you don't have time to build a complex prompt.

#### 2. Few-Shot Prompting
The Strategy: Providing the AI with 2 or 3 examples of what a "perfect" undergraduate summary looks like before asking it to summarize the blockchain article.

Best Platform: GPT-5.4

Performance:

Accuracy: Extremely High; the model follows the structural patterns of your examples (e.g., specific headings or bullet points).

Coherence: Very High; it mirrors the tone you provide in the examples perfectly.

Simplicity: Excellent; since you can provide a "simple" example, the AI will match that level of complexity.

Speed: Fast, though the longer prompt (examples) takes slightly more time to process.

User Experience: Best for consistency across a large volume of research papers.

#### 3. Chain-of-Thought (CoT) Prompting
The Strategy: Instructing the AI to "think step-by-step" by first identifying key technical concepts (like hashing or decentralization) before writing the final summary.

Best Platform: Gemini 3.1 Pro

Performance:

Accuracy: The Winner; by breaking down the logic, the AI rarely misses technical nuances or confuses different blockchain protocols.

Coherence: High; the summary follows a logical progression from "what it is" to "how it works."

Simplicity: Moderate; sometimes the "steps" can make the final output feel a bit technical.

Speed: Very Fast; Gemini's 2026 architecture handles multi-step reasoning rapidly.

User Experience: Best for educational depth, ensuring students understand the mechanics behind the concepts.

#### 4. Role-Based Prompting
The Strategy: Assigning the AI a persona, such as "You are a Senior Research Fellow who specializes in explaining complex tech to first-year college students."

Best Platform: Microsoft Copilot

Performance:

Accuracy: High; the "expert" persona tends to prioritize factual correctness.

Coherence: Good; it maintains a consistent "teacher" voice throughout.

Simplicity: The Winner; the persona naturally uses analogies (like comparing blockchain to a public ledger or a shared digital notebook).

Speed: Moderate; influenced by real-time web-referencing.

User Experience: Best for engagement. The summary feels like a lecture note or a guided explanation rather than a dry document.

### Copilot:
#### 1. Zero-Shot Prompting
Strategy: Asking the AI to summarize the blockchain article with no prior examples or detailed instructions.

Best Platform: Claude 4.6 Opus

Performance:

Accuracy: High — Claude stays true to the source text without unnecessary additions.

Coherence: Superior — produces fluid, natural-sounding paragraphs.

Simplicity: Good — sometimes leans toward advanced vocabulary.

Speed: Moderate.

User Experience: Best for quick, one-off summaries when time is limited.

#### 2. Few-Shot Prompting
Strategy: Providing 2–3 examples of ideal undergraduate summaries before asking for the blockchain summary.

Best Platform: GPT‑5.4

Performance:

Accuracy: Extremely High — follows structural patterns of examples (e.g., headings, bullet points).

Coherence: Very High — mirrors tone and style consistently.

Simplicity: Excellent — matches the simplicity of provided examples.

Speed: Fast — though longer prompts take slightly more time to process.

User Experience: Best for consistency across large volumes of research papers.

#### 3. Chain-of-Thought Prompting
Strategy: Instructing the AI to reason step-by-step, identifying key concepts (hashing, decentralization) before summarizing.

Best Platform: Gemini 3.1 Pro

Performance:

Accuracy: The Winner — rarely misses technical nuances or confuses protocols.

Coherence: High — logical progression from “what it is” to “how it works.”

Simplicity: Moderate — stepwise reasoning can feel technical.

Speed: Very Fast — Gemini’s architecture handles multi-step reasoning efficiently.

User Experience: Best for educational depth, ensuring students grasp mechanics.

#### 4. Role-Based Prompting
Strategy: Assigning the AI a persona, e.g., “You are a Senior Research Fellow explaining blockchain to first-year students.”

Best Platform: Microsoft Copilot

Performance:

Accuracy: High — persona prioritizes factual correctness.

Coherence: Good — maintains consistent “teacher” voice.

Simplicity: The Winner — naturally uses analogies (e.g., blockchain as a public ledger).

Speed: Moderate — influenced by real-time web referencing.

User Experience: Best for engagement — feels like lecture notes or guided explanation.

### Claude:
#### Zero-Shot Output
Blockchain is a decentralized ledger that records transactions in blocks linked by cryptographic hashes, ensuring transparency, security, and data integrity.

#### Few-Shot Output

Blockchain stores transactions in connected blocks protected by hashing techniques. Consensus mechanisms validate the information, enabling applications such as cryptocurrencies, smart contracts, and supply chain tracking.

#### Chain-of-Thought Output

Step 1: Define blockchain as a distributed and decentralized ledger.
Step 2: Explain how transactions are grouped into blocks and linked using cryptographic hashes.
Step 3: Describe consensus mechanisms that verify and secure the data.
Step 4: Mention practical applications such as cryptocurrencies, healthcare, and supply chain management.

#### Final Summary: 
Blockchain is a secure distributed ledger technology that records and verifies transactions across multiple systems without a central authority.

#### Role-Based Output
As a university professor explaining to undergraduate students, blockchain can be described as a decentralized digital ledger that ensures trust, transparency, and immutability by combining cryptographic hashing with distributed consensus mechanisms.

## Performance Evaluation Table:
<img width="1691" height="930" alt="image" src="https://github.com/user-attachments/assets/8daf9df7-b112-463a-88f6-08486cc2c292" />

## Summary Insight
Best Accuracy & Technical Depth: Gemini with Chain-of-Thought Prompting
Best Coherence & Simplicity: Microsoft Copilot with Role-Based Prompting
Best Balanced Performance: ChatGPT with Few-Shot Prompting
Best Quick Summaries: Claude with Zero-Shot Prompting
Best Overall Combination: Role-Based Prompting + Microsoft Copilot

## Conclusion
The evaluation shows that both prompting technique and AI platform selection strongly influence the quality of summaries. Role-Based Prompting consistently produced the most effective results because it adapts explanations to undergraduate students, making the summaries clearer, more engaging, and easier to understand. ChatGPT provided the most balanced performance, Gemini excelled in technical reasoning, Claude generated highly coherent summaries with simple prompts, and Copilot delivered the most beginner-friendly outputs.

## Result
The experiment confirms that prompting technique and model choice together have a significant impact on summary quality. Among all techniques, Role-Based Prompting achieved the best overall performance, especially when used with Microsoft Copilot. For educational content generation, this combination is the most effective for producing accurate, coherent, and student-friendly summaries.


