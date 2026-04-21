# Interview System Design Template

Use this template as a generic structure for guiding your System Design interview discussions. Remember that a 45-minute interview is brief, so spend time only on what's critical.

---

## 1. Requirement Collection & Scope (5 mins)
*Always start by clarifying the question and narrowing down the scope.*

### Functional Requirements
*   What should the system do? (e.g., "Users should be able to upload a video", "Users can search for a video", "Users can view a video")
*   Are there any background processes? (e.g., "Videos must be compressed automatically")

### Non-Functional Requirements
*   **Highly Available vs Highly Consistent?** (CAP Theorem)
*   **Latency:** Does it need to be low latency?
*   **Scale:** Can it scale globally?
*   **Fault Tolerance:** What happens if a node goes down?

## 2. Capacity Planning & Estimations (5 mins)
*Keep this brief. Use back-of-the-envelope calculations.*
*   Read/Write ratio?
*   Traffic Estimates (QPS - Queries Per Second)
*   Storage Estimates (per day, per 5 years)
*   Bandwidth Estimates

## 3. API Design (5 mins)
*Define the exact contract between the client and the server.*
*   `uploadVideo(user_id, video_file, title, description)` -> `video_id`
*   `getVideo(video_id)` -> `video_url`

## 4. Database Schema (5 mins)
*Define the data models based on the API.*
*   Relational (SQL) vs Non-Relational (NoSQL)? Why?
*   Tables:
    *   `Users` (uuid, name, email)
    *   `Videos` (video_id, user_id, s3_path, metadata, created_at)

## 5. High Level Design (10 mins)
*Draw the core architecture. Walk through a request's lifecycle.*
*   Client -> Load Balancer -> Web/App Servers -> Database / Cache
*   Where does asynchronous processing fit in? (Message Queues)
*   Where is the file storage? (Object Storage like S3 or GCS)

## 6. Detailed Design & Bottlenecks (10-15 mins)
*Deep dive into specific areas based on interviewer's interests.*
*   **Scaling the Database:** Sharding (how do we shard?), Replication (Master-Slave).
*   **Caching Strategy:** Eviction policies (LRU), Cache aside vs Write-through.
*   **Concurrency Issues:** How to handle two users booking the same seat?
*   **Failure Scenarios:** Discuss Single Points of Failure (SPOF) and how to mitigate them.
