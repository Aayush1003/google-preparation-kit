# 🏢 The 5 Rounds of Google Interviews

To successfully navigate the Google interview process, you need to understand the focus and expectations for each of the five primary evaluation stages. This guide provides a detailed breakdown of what to expect, how you are evaluated, and tips for success.

---

## 🛰️ Round 1: Technical Phone Screen
**Duration:** 45 - 60 Minutes
**Platform:** Google Meet + Google Docs (collaborative coding)

### 🎯 Focus
This is the "gatekeeper" round. The goal is to verify your core CS fundamentals and problem-solving speed.

- **Coding:** You'll solve 1-2 medium-difficulty LeetCode-style problems.
- **Complexity:** Focus on Big O analysis (Time & Space).
- **Communication:** Can you explain your logic before typing?

> [!TIP]
> Use a headset and ensure a stable connection. Since you're coding in a Google Doc (no syntax highlighting or auto-complete), practice writing clean code in a plain text editor.

---

## 💻 Round 2: Coding Round I (Algorithms & Data Structures)
**Duration:** 45 Minutes
**Platform:** Virtual Onsite

### 🎯 Focus
This round deep-dives into your ability to apply complex data structures to ambiguous problems.

- **Problem Types:** Often involves Trees, Graphs, or Dynamic Programming.
- **Evaluation:**
  - **Logic:** Accuracy of the algorithm.
  - **Edge Cases:** Handling nulls, empty inputs, or extremely large datasets.
  - **Speed:** Coming up with the optimal solution within 15-20 minutes.

---

## 🧠 Round 3: Coding Round II (Advanced Problem Solving)
**Duration:** 45 Minutes
**Platform:** Virtual Onsite

### 🎯 Focus
Expect "Follow-up" questions here. The interviewer will likely start with a basic problem and then add constraints that make it much harder.

- **Dynamic Constraints:** "What if the data is too large for memory?" or "What if the input stream is continuous?"
- **Refactoring:** Your ability to adapt your code to changing requirements.

---

## 🏗️ Round 4: System Design / Architecture
**Duration:** 45 Minutes
**Platform:** Virtual Onsite
**Level:** Primarily for L4 (Mid) and L5+ (Senior) roles.

### 🎯 Focus
Testing your ability to design scalable, reliable, and maintainable systems.

- **Components:** Load Balancers, Databases (SQL vs NoSQL), Caching, Messaging Queues (Kafka/RabbitMQ).
- **Trade-offs:** Every design decision has a pro and a con. You must justify *why* you chose one over the other.
- **Scalability:** How do you handle 100M+ DAU (Daily Active Users)?

> [!IMPORTANT]
> For L3 (Entry-level), this might be replaced by an additional Coding round or a "General Computing" round.

---

## 🤝 Round 5: Googliness & Leadership (Behavioral)
**Duration:** 45 Minutes
**Platform:** Virtual Onsite

### 🎯 Focus
This is arguably the most important round. Google cares deeply about *how* you work, not just *what* you can build.

- **Googliness:** Ambiguity handling, taking feedback, supporting others, and ethical decision-making.
- **Leadership:** Leading without authority and ownership of projects.
- **STAR Method:** All answers should follow the **Situation, Task, Action, Result** framework.

---

## 📊 Summary Table

| Round | Primary Skill | Key Expectation |
| :--- | :--- | :--- |
| **Phone Screen** | Fundamentals | Speed and Cleanliness |
| **Coding I** | DSA Application | Optimal Complexity |
| **Coding II** | Adaptability | Handling Constraints |
| **System Design** | Architecture | Scalability Trade-offs |
| **Googliness** | Soft Skills | Cultural Alignment & STAR |

## 📚 Expanded Guidance for Each Round

### 🛰️ Round 1: Technical Phone Screen
#### 📖 Preparation Tips
- Practice **plain‑text coding** in a simple editor (no syntax highlighting) to mimic the Google Docs environment.
- Time yourself: aim to write a correct solution in **≤ 8 minutes** and then discuss the approach for the remaining time.
- Master **edge‑case enumeration** before you start coding – interviewers love thoroughness.

#### 🧩 Core Topics
- Arrays & Strings (two‑pointer, sliding window)
- Basic Recursion/Backtracking
- Simple Hash‑map usage
- Big‑O analysis and space‑time trade‑offs

#### 🗂 Sample Questions
- *Two Sum* – variations with sorted input, duplicate handling.
- *Longest Substring Without Repeating Characters* – discuss sliding‑window.
- *Reverse a Linked List* – explain iterative vs recursive approach.

---

### 💻 Round 2: Coding Round I (Algorithms & Data Structures)
#### 📖 Preparation Tips
- Focus on **optimizing** an initial brute‑force solution; interviewers often ask you to improve it.
- Write **clean, modular code** – helper functions are allowed and can be discussed.
- Practice explaining **time/space** trade‑offs while coding.

#### 🧩 Core Topics
- Trees (BST, traversal, LCA)
- Graphs (BFS/DFS, shortest path basics)
- Dynamic Programming (memoization, tabulation)
- Heaps & Priority Queues

#### 🗂 Sample Questions
- *Lowest Common Ancestor in a Binary Tree*
- *Number of Islands* (DFS/BFS grid traversal)
- *Maximum Subarray* (Kadane’s algorithm) – discuss alternative O(N log N) solution.

---

### 🧠 Round 3: Coding Round II (Advanced Problem Solving)
#### 📖 Preparation Tips
- Be ready for **follow‑up constraints** that change the problem space.
- Practice **refactoring** on the fly – keep the original solution intact while you iterate.
- Strengthen your ability to discuss **complexity implications** of each new constraint.

#### 🧩 Core Topics
- Advanced DP (interval DP, bitmask DP)
- Sliding‑window with variable size
- In‑place algorithms & space‑optimizations
- Multi‑threading concepts (if asked)

#### 🗂 Sample Questions
- *Word Ladder* – discuss bidirectional BFS.
- *Median of Two Sorted Arrays* – explore O(log min(m,n)) solution.
- *Serialize and Deserialize a Binary Tree* – optimize for space.

---

### 🏗️ Round 4: System Design / Architecture
#### 📖 Preparation Tips
- Start with **high‑level requirements** (throughput, latency, consistency) before diving into components.
- Use the **C.A.D. (Compute, Store, Distribute)** framework to structure your answer.
- Prepare a **few go‑to designs** (e.g., URL shortener, Twitter feed, chat system) and adapt them.

#### 🧩 Core Topics
- Load Balancers, CDN, Caching (Redis, Memcached)
- Data storage choices (SQL vs NoSQL, sharding, replication)
- Messaging systems (Kafka, RabbitMQ) and eventual consistency
- CAP theorem, latency vs throughput trade‑offs
- Monitoring & alerting (metrics, logs, tracing)

#### 🗂 Sample Prompts
- Design a **global file‑storage service** like Google Drive.
- Architect a **real‑time collaborative editor** (Google Docs style).
- Build a **notification system** handling millions of users.

---

### 🤝 Round 5: Googliness & Leadership (Behavioral)
#### 📖 Preparation Tips
- Prepare **5‑7 STAR stories** covering: ownership, conflict resolution, mentorship, failure, and impact.
- Practice **concise storytelling** – keep each story under 2‑3 minutes.
- Emphasize **Google’s core values**: humility, learning, and collaborative mindset.

#### 🧩 Focus Areas
- Ambiguity handling – give examples where you defined requirements.
- Feedback loops – describe a time you gave and received constructive feedback.
- Leadership without authority – showcase project ownership.

#### 🗂 Sample Behavioral Prompts
- “Tell me about a time you failed and what you learned.”
- “Describe a situation where you had to convince a team to adopt a new approach.”
- “How do you prioritize tasks when you have multiple competing deadlines?”

---

## 📎 Additional Resources
- **LeetCode Top Interview Questions** – filter by “Google” tag.
- **System Design Primer** (GitHub repo by donnfelker) – read the “Design Patterns” chapter.
- **Google’s Career Site** – official interview guide and Googliness videos.
- **“Cracking the Coding Interview”** – focus on chapters 8‑11 for DS&A.
- **Mock interview platforms**: Pramp, Interviewing.io, Exponent.

Feel free to customize these notes, add personal anecdotes, and link to any external resources you find helpful. Good luck! 🎉
