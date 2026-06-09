# Project 1 Planning: The Unofficial Guide

> Write this document before you write any pipeline code.
> Your spec and architecture diagram are what you'll use to direct AI tools (Claude, Copilot, etc.) to generate your implementation — the more specific they are, the more useful the generated code will be.
> Update the Retrieval Approach and Chunking Strategy sections if you change your approach during implementation.
> Update this file before starting any stretch features.

---

## Domain

The domain is reviews for budget smartphones that are $300 or less

This guide will make it easier for users to find a perfect smartphone in their budget. It will be based on public user reviews and coments, as well as professional reviews and tests. Typically, anyone who wanted to access this information would need to browse multiple websites and blindly trust random opinions in the internet, which makes it harder to make an informed decision on their smartphone. The guide gives them the information needed to make their next purchase.

---

## Documents

<!-- List your specific sources: URLs, subreddit names, forum threads, or file descriptions.
     Aim for at least 10 sources that together cover different subtopics or perspectives within your domain. -->
| # | Source | Type | URL or file path |
|---|--------|------|-----------------|
| 1 | Best entry-level smartphones guide | Buyer's guide | https://www.gsmarena.com/best_entry_level_smartphones_buyers_guide-review-2034.php |
| 2 | Nothing CMF Phone 2 review | Pro review | https://www.gsmarena.com/nothing_cmf_phone_2_pro-review-2827.php |
| 3 | Nothing CMF Phone 2 review user comments | User reviews | https://www.gsmarena.com/nothing_cmf_phone_2_pro_5g-reviews-13821.php |
| 4 | Pixel 9a review | Pro review | https://www.gsmarena.com/google_pixel_9a-review-2825.php |
| 5 | Pixel 9a user comments | User reviews | https://www.gsmarena.com/google_pixel_9a-reviews-13478.php |
| 6 | Nothing CMF Phone 2 review from PhoneArena | Pro review | https://www.phonearena.com/reviews/cmf-phone-2-pro-review_id7240 |
| 7 | Budget and affordable phones | Buyer's guide | https://www.phonearena.com/news/Budget-affordable-cheap-low-cost-smartphones-android-this-year_id58696 |
| 8 | Best cheap phones | Buyer's guide | https://www.tomsguide.com/best-picks/best-cheap-phones |
| 9 | Best phones under $300 | Buyer's guide | https://www.androidcentral.com/best-android-phones-under-300 |
| 10 | Best phones under $300 in 2026 | Buyer's guide | https://www.techtimes.com/articles/313609/20251225/best-smartphones-buy-under-300-2026.htm |


Questions:
1. What phones under $300 have the best storage?
2. What phones under $300 have the best camera?
3. Does the CMF Phone 2/Pixel 9a have overheating issues?
4. What downsides do reviewers report about the CMF Phone 2/Pixel 9a?
5. What phones under $300 have the best battery capacity? 
---

## Chunking Strategy

<!-- How will you split documents into chunks?
     State your chunk size (in tokens or characters), overlap size, and explain why those
     numbers fit the structure of your documents.
     A review-heavy corpus warrants different chunking than a long FAQ. -->

**Chunk size:**

**Overlap:**

**Reasoning:**

---

## Retrieval Approach

<!-- Which embedding model are you using (e.g., all-MiniLM-L6-v2 via sentence-transformers)?
     How many chunks will you retrieve per query (top-k)?
     If you were deploying this for real users and cost wasn't a constraint, what tradeoffs
     would you weigh in choosing a different embedding model — context length, multilingual
     support, accuracy on domain-specific text, latency? -->

**Embedding model:**

**Top-k:**

**Production tradeoff reflection:**

---

## Evaluation Plan

<!-- List your 5 test questions with their expected correct answers.
     Questions should be specific enough that you can judge whether the system's response
     is right or wrong. "What are good dining halls?" is too vague.
     "What do students say about wait times at [dining hall name] during lunch?" is testable. -->

| # | Question | Expected answer |
|---|----------|-----------------|
| 1 | | |
| 2 | | |
| 3 | | |
| 4 | | |
| 5 | | |

---

## Anticipated Challenges

<!-- What could go wrong? Name at least two specific risks with reasoning.
     Consider: noisy or inconsistent documents, missing source attribution, off-topic
     retrieval, chunks that split key information across boundaries. -->

1.

2.

---

## Architecture

<!-- Draw a diagram of your pipeline showing the five stages:
     Document Ingestion → Chunking → Embedding + Vector Store → Retrieval → Generation
     Label each stage with the tool or library you're using.
     You can use ASCII art, a Mermaid diagram, or embed a sketch as an image.
     You'll use this diagram as context when prompting AI tools to implement each stage. -->

---

## AI Tool Plan

<!-- For each part of the pipeline below, describe:
     - Which AI tool you plan to use (Claude, Copilot, ChatGPT, etc.)
     - What you'll give it as input (which sections of this planning.md, which requirements)
     - What you expect it to produce
     - How you'll verify the output matches your spec

     "I'll use AI to help me code" is not a plan.
     "I'll give Claude my Chunking Strategy section and ask it to implement chunk_text()
     with my specified chunk size and overlap" is a plan. -->

**Milestone 3 — Ingestion and chunking:**

**Milestone 4 — Embedding and retrieval:**

**Milestone 5 — Generation and interface:**
