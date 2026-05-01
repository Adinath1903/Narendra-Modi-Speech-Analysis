You can copy and paste the following content directly into a file named **README.md** in your GitHub repository.

---

# Thematic & Temporal Analysis of “Mann Ki Baat” Speeches

## Project Overview
This project presents a comprehensive statistical and linguistic study of Prime Minister Narendra Modi’s "Mann Ki Baat" radio program[cite: 1]. By analyzing 126 episodes spanning from June 2014 to the present, the study aims to uncover recurring themes and understand the mathematical predictability of the PM’s communication patterns.

## Key Objectives
*   Identify the main themes (topics) appearing in the speeches using NLP techniques.
*   Track how these themes evolve and change over time.
*   Analyze the temporal structure and predictability of these themes using Markov Chain theory.

## Methodology

### 1. Data Preprocessing & Chunking
*   **Cleaning**: Raw text was cleaned by removing punctuation, numbers, and stopwords, followed by lemmatization to extract root words.
*   **Chunking**: To improve the accuracy of topic modeling, long speeches were split into smaller, focused "mini-documents," resulting in approximately 320 text chunks.

### 2. Topic Modeling (LDA)
Using **Latent Dirichlet Allocation (LDA)**, the study identified six optimal latent topics based on Coherence Scores ($K=6$):
*   **Topic 0**: Sports / Youth / Education
*   **Topic 1**: Patriotism / Unity / Social Service
*   **Topic 2**: Leadership / Health / Communication
*   **Topic 3**: Education / Farmers / Citizen Issues
*   **Topic 4**: Healthcare / Organ Donation / Awareness
*   **Topic 5**: Women Empowerment / Culture

### 3. Markov Chain Analysis
The project treats the sequence of topics as a Markov Process, where the next topic depends on the current state.
*   **Transition Matrix**: Captured the probability of moving from one theme to another.
*   **Stationary Distribution ($\pi$)**: Found that the system spends ~99% of its time in Topic 3 (Education & Civic issues) in the long run.
*   **Mean First Passage Time (MFPT)**: Calculated the expected number of steps to reach or return to a specific topic.
*   **Entropy Rate**: Measured at 0.09 bits per step, indicating a highly structured and predictable communication sequence.

## Results & Conclusions
*   **Dominant Theme**: "Education and Citizen Issues" serves as the central hub and a "practically absorbing state" of the program.
*   **Predictability**: The very low entropy rate confirms that the speeches follow a stable, consistent narrative with limited thematic drift.
*   **Structure**: Regardless of the starting point, the conversation typically returns to core civic themes within 1–2 speech segments.
  
**Author**: Adinath Nare
