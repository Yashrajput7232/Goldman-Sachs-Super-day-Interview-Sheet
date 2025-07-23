# 📘 Goldman Sachs Superday Full Checklist (Grouped by Topic)

Track your progress for DSA, System Design, Puzzles, and Behavioral rounds. Each table includes difficulty, topic, hints, edge cases, and answering strategy.

---

## ✅ Data Structures and Algorithms (DSA)

### Arrays

| ✅    | Problem                                                                                                | Difficulty | Hint                               | Edge Cases               |
| ---- | ------------------------------------------------------------------------------------------------------ | ---------- | ---------------------------------- | ------------------------ |
| \[ ] | [Arithmetic Progression](https://leetcode.com/problems/can-make-arithmetic-progression-from-sequence/) | Easy       | Sort and check difference          | Duplicates, zero         |
| \[ ] | [Wave Array](https://www.geeksforgeeks.org/problems/wave-array-1587115621/1)                           | Easy       | Swap alternate elements            | Odd-sized array          |
| \[ ] | [Rectangle Overlap](https://leetcode.com/problems/rectangle-overlap/)                                  | Easy       | Check overlap on both axes         | Touching edges           |
| \[ ] | [Trapping Rain Water](https://leetcode.com/problems/trapping-rain-water/)                              | Hard       | Use leftMax/rightMax or 2 pointers | Flat/ascending array     |
| \[ ] | [Median of Sorted Arrays](https://leetcode.com/problems/median-of-two-sorted-arrays/)                  | Hard       | Binary search on smaller array     | One empty, unequal sizes |

### Strings

| ✅    | Problem                                                                                           | Difficulty | Hint                            | Edge Cases                     |
| ---- | ------------------------------------------------------------------------------------------------- | ---------- | ------------------------------- | ------------------------------ |
| \[ ] | [Remove k Duplicates](https://leetcode.com/problems/remove-all-adjacent-duplicates-in-string-ii/) | Medium     | Stack with count                | Entire string removed          |
| \[ ] | [Reverse Words](https://leetcode.com/problems/reverse-words-in-a-string/)                         | Medium     | Split → reverse → join          | Multiple spaces                |
| \[ ] | [Decode Message](https://leetcode.com/problems/decode-the-message/)                               | Medium     | Track mappings uniquely         | Duplicates, mismatched pattern |
| \[ ] | [Remove Anagrams](https://leetcode.com/problems/find-resultant-array-after-removing-anagrams/)    | Medium     | Sort/frequency to check anagram | Reordered same strings         |

### Trees

| ✅    | Problem                                                                                                      | Difficulty | Hint                               | Edge Cases           |
| ---- | ------------------------------------------------------------------------------------------------------------ | ---------- | ---------------------------------- | -------------------- |
| \[ ] | [Balanced Binary Tree](https://leetcode.com/problems/balanced-binary-tree/)                                  | Medium     | Use post-order to calculate height | Empty or 1-node tree |
| \[ ] | [Sum Tree](https://www.geeksforgeeks.org/dsa/check-if-a-binary-tree-is-sum-tree/)                            | Medium     | Post-order, sum of subtrees = node | Leafs, zero values   |
| \[ ] | [Binary Tree to DLL](https://leetcode.com/problems/convert-binary-search-tree-to-sorted-doubly-linked-list/) | Medium     | In-order traversal to link nodes   | Single node          |

### Linked Lists

| ✅    | Problem                                                                                             | Difficulty | Hint                              | Edge Cases                     |
| ---- | --------------------------------------------------------------------------------------------------- | ---------- | --------------------------------- | ------------------------------ |
| \[ ] | [Palindrome Linked List](https://leetcode.com/problems/palindrome-linked-list/)                     | Medium     | Reverse second half and compare   | Odd length, one node           |
| \[ ] | [Intersection of Two Linked Lists](https://leetcode.com/problems/intersection-of-two-linked-lists/) | Easy       | Traverse both, then switch heads  | No intersection                |
| \[ ] | [Flatten Multilevel DLL](https://leetcode.com/problems/flatten-a-multilevel-doubly-linked-list/)    | Medium     | DFS with stack to flatten         | Multi-level nesting            |
| \[ ] | [Delete Node](https://leetcode.com/problems/delete-node-in-a-linked-list/)                          | Easy       | Copy next node’s data and skip it | Last node (undefined behavior) |

### Graphs

| ✅    | Problem                                                                  | Difficulty | Hint                            | Edge Cases            |
| ---- | ------------------------------------------------------------------------ | ---------- | ------------------------------- | --------------------- |
| \[ ] | [Number of Islands](https://leetcode.com/problems/number-of-islands/)    | Medium     | DFS/BFS to mark visited islands | All water or all land |
| \[ ] | [Knight Moves](https://leetcode.com/problems/minimum-knight-moves/)      | Medium     | BFS from source to destination  | Start equals end      |
| \[ ] | [Celebrity Problem](https://leetcode.com/problems/possible-bipartition/) | Medium     | Use 2 pointers to find & verify | No one knows anyone   |

### Stack/Queue

| ✅    | Problem                                                                         | Difficulty | Hint                                | Edge Cases             |
| ---- | ------------------------------------------------------------------------------- | ---------- | ----------------------------------- | ---------------------- |
| \[ ] | [Min Stack](https://leetcode.com/problems/min-stack/)                           | Medium     | Use auxiliary stack or min tracking | Duplicates in min      |
| \[ ] | [Queue via Stacks](https://leetcode.com/problems/implement-queue-using-stacks/) | Easy       | Two stacks (push/pop trick)         | Consecutive operations |

### Dynamic Programming

| ✅    | Problem                                                                                             | Difficulty | Hint                       | Edge Cases               |
| ---- | --------------------------------------------------------------------------------------------------- | ---------- | -------------------------- | ------------------------ |
| \[ ] | [Climbing Stairs](https://leetcode.com/problems/climbing-stairs/)                                   | Easy       | DP with memo or tabulation | n = 0 or 1               |
| \[ ] | [Stock III](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-iii/)                     | Hard       | Track two buys/sells       | Prices always decreasing |
| \[ ] | [Stock with Cooldown](https://leetcode.com/problems/best-time-to-buy-and-sell-stock-with-cooldown/) | Hard       | DP with cooldown states    | Single price             |
| \[ ] | [Egg Drop Puzzle](https://leetcode.com/problems/super-egg-drop/)                                    | Hard       | State = (eggs, floors)     | 1 egg, 0 floor           |

### Math/Misc

| ✅    | Problem                                                                                     | Difficulty | Hint                        | Edge Cases         |
| ---- | ------------------------------------------------------------------------------------------- | ---------- | --------------------------- | ------------------ |
| \[ ] | [Ugly Number](https://leetcode.com/problems/ugly-number/)                                   | Easy       | Divide by 2,3,5 repeatedly  | Negative numbers   |
| \[ ] | [Reverse Integer](https://leetcode.com/problems/reverse-integer/)                           | Easy       | Modulo, check 32-bit bounds | Overflow/underflow |
| \[ ] | [First Unique Character](https://leetcode.com/problems/first-unique-character-in-a-string/) | Easy       | Frequency count then index  | All repeated       |

---

## 🏗️ System Design Questions

| ✅    | Problem                 | Key Concepts                              | Java Tech Stack               | Hint                            |
| ---- | ----------------------- | ----------------------------------------- | ----------------------------- | ------------------------------- |
| \[ ] | Card Payment System     | Fault Tolerance, Security, Reconciliation | Spring Boot, Kafka, SQL       | Use atomicity, retries, queue   |
| \[ ] | Stock Trading Exchange  | Low Latency, Matching Engine              | Java NIO, Redis, Kafka        | Sliding window + event queuing  |
| \[ ] | Chat App                | Real-time, Pub/Sub                        | WebSockets, Redis, Kafka      | Use Redis pub-sub and sockets   |
| \[ ] | Microservice E-commerce | Scalability, Async Calls                  | Docker, K8s, gRPC, Kafka      | Decompose by domain + event bus |
| \[ ] | Search Engine           | Inverted Index, Crawling                  | Lucene, Elastic, Spring       | Parse content + store keywords  |
| \[ ] | File Sharing System     | Replication, Consistency                  | S3, HDFS, Kafka               | Consistent hashing, CDN         |
| \[ ] | Parking Lot System      | IoT, Payment                              | Spring, Sensors, Gateway APIs | Use RFID or ticket scanning     |
| \[ ] | Social Feed             | Fanout, Personalization                   | Graph DB (Neo4j), Redis       | Precompute for high users       |
| \[ ] | SQL DB with Sharding    | Load Distribution, Availability           | Postgres + Shard Proxy        | Hashing + query router          |
| \[ ] | Your Own Project        | End-to-end discussion                     | Your Tech Stack               | Focus on trade-offs, decisions  |
