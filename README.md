# EX-02-Cross-Platform-Prompting-Evaluating-Diverse-Techniques-in-AI-Powered-Text-Summarization

## AIM
To evaluate and compare the effectiveness of prompting techniques (zero-shot, few-shot, chain-of-thought, role-based) across different AI platforms (e.g., ChatGPT, Gemini, Claude, Copilot) in a specific task: text summarisation.

## Scenario:

### Step 1:

Summarise the following 500-word article on “The Basics of Blockchain Technology” in 120–150 words for undergraduate students. Keep it clear and beginner-friendly.


### Step 2 (Feedback):

Please revise the summary to simplify it and include at least two real-world examples of blockchain applications.

## Algorithm
1.	Input Preparation:
o	A ~500-word article was written on “The Basics of Blockchain Technology.”
o	This served as the common input for all AI models.
2.	Prompt Design (Step 1):
o	Each AI model was given the same instruction:
“Summarise this article on ‘The Basics of Blockchain Technology’ in 120–150 words for undergraduate students. Keep it clear and beginner-friendly.”
o	This tested zero-shot / direct prompting performance.
3.	Feedback Refinement (Step 2):
o	Each AI was then instructed:
“Make this summary even simpler and include at least two real-world examples of blockchain applications.”
o	This tested iterative / feedback-based prompting.
4.	Prompting Techniques Applied:
o	Zero-Shot Prompting: Asking directly without examples (used for Step 1).
o	Role-Based Prompting: Instructing the model to act like a teacher/lecturer (Gemini).
o	Chain-of-Thought Prompting: Asking the model to break down key points before summarising (Claude).
o	Feedback Refinement: Give further instructions on simplifying and adding examples (all models in Step 2).
5.	Output Collection:
o	Summaries from each platform (ChatGPT, Gemini, Claude, Copilot) were recorded in Step 1 and Step 2 formats.
6.	Comparison & Analysis:
o	Outputs were compared across AI models for clarity, depth, simplicity, and inclusion of real-world examples.
o	Results were presented in a comparison table(Google Drive).

## Result
| Platform / Model | Step 1 Summary | Step 2 Revised Summary | Remarks |
|------------------|----------------|-------------------------|---------|
| **ChatGPT (OpenAI)** | Blockchain is a digital system that records transactions securely and transparently across many computers, without needing a central authority. Information is grouped into blocks, linked to form a chain that is nearly impossible to alter. Originally used in Bitcoin, it is now applied in supply chain tracking, healthcare, voting, and smart contracts. Despite challenges like scalability and energy use, blockchain remains a promising technology. (Word Count: 141) | Blockchain is a special way of storing information that is shared across many computers. Once data is added, it cannot be changed, making it trustworthy. First famous for Bitcoin, it is now used by Walmart for food tracking and Estonia for healthcare records. Despite slow speed and energy use, it is expanding in finance, supply chains, and healthcare. (Word Count: 145) | Balanced, beginner-friendly, with real-world context |
| **Gemini (Google)** | Blockchain is a shared digital record distributed across many computers (decentralization). Data is grouped into “blocks” linked in a secure “chain.” Each block has a cryptographic fingerprint, making it nearly impossible to alter. Famous for Bitcoin, blockchain’s trust-building ability is now being explored in many industries. (Word Count: 142) | Blockchain is like a digital notebook copied across computers so no one can secretly change data. It is highly secure and trustworthy. Examples: Walmart tracks mangoes in its supply chain, and NFTs provide ownership for digital art/music. Blockchain builds trust across industries. | Clear, uses analogies, good for absolute beginners |
| **Claude (Anthropic)** | Blockchain is a digital ledger across multiple computers, making it almost impossible to hack or change. Each block of transactions is verified by the network before being added permanently. It removes the need for central authorities and offers transparency, security, and immutability. (Word Count: 147) | Blockchain is like a digital record book shared among many computers. Everyone keeps an identical copy, so it’s secure. Examples: Bitcoin transactions verified without banks, and Walmart’s supply chain tracking to trace food contamination. This builds trust without middlemen. (Word Count: 165) | Very explanatory, emphasizes analogy + security |
| **Copilot (Microsoft)** | Blockchain is a decentralized ledger recording transactions across many computers. It ensures transparency, security, and immutability. First used in Bitcoin, it now applies to finance, healthcare, supply chain, and voting. Challenges include scalability, energy use, and regulation. (~140 words) | Blockchain is like a digital notebook everyone can see but no one can erase. Examples: Banking for cross-border transfers, healthcare for patient records, supply chains for tracking goods, and voting for secure elections. Uses cryptography, consensus, and smart contracts but faces speed and energy challenges. | Covers more technical detail, broader applications |
