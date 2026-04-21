# Cheat Sheets

Quick reference materials for last-minute revisions before your interview.

## 1. Time & Space Complexity (Big O)

| Data Structure | Access | Search | Insertion | Deletion | Space |
| :--- | :---: | :---: | :---: | :---: | :---: |
| Array | O(1) | O(n) | O(n) | O(n) | O(n) |
| Stack | O(n) | O(n) | O(1) | O(1) | O(n) |
| Queue | O(n) | O(n) | O(1) | O(1) | O(n) |
| Singly Linked List | O(n) | O(n) | O(1)* | O(1)* | O(n) |
| Hash Table | - | O(1) | O(1) | O(1) | O(n) |
| Binary Search Tree | O(log n) | O(log n) | O(log n) | O(log n) | O(n) |
| B-Tree | O(log n) | O(log n) | O(log n) | O(log n) | O(n) |

*\*If pointer to node is given.*

## 2. System Design - Numbers Every Engineer Should Know

| Operation | Time |
| :--- | :--- |
| L1 cache reference | 0.5 ns |
| Branch mispredict | 5 ns |
| L2 cache reference | 7 ns |
| Mutex lock/unlock | 100 ns |
| Main memory reference | 100 ns |
| Compress 1K bytes with Zippy | 10,000 ns (10 µs) |
| Send 2K bytes over 1 Gbps network | 20,000 ns (20 µs) |
| Read 1 MB sequentially from memory | 250,000 ns (250 µs) |
| Round trip within same datacenter | 500,000 ns (500 µs) |
| Disk seek | 10,000,000 ns (10 ms) |
| Read 1 MB sequentially from network | 10,000,000 ns (10 ms) |
| Read 1 MB sequentially from disk | 30,000,000 ns (30 ms) |
| Send packet CA->Netherlands->CA | 150,000,000 ns (150 ms) |

## 3. Quick System Design Checklist
- [ ] Ask clarifying questions (Scope, Traffic, Data size).
- [ ] Define system boundaries.
- [ ] Outline Core Entities / Data Models.
- [ ] Draw High-Level Architecture (Client -> LB -> App/Web -> Cache/DB).
- [ ] Discuss trade-offs (Consistency vs. Availability).
- [ ] Identify bottlenecks and scaling solutions.
