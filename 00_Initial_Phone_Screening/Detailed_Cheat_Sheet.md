# Google Initial Phone Screening: Detailed Script & Cheat Sheet

This document is designed to give you **detailed, easy-to-read scripts** for your interview. If you don't know the deep technical details of your projects, **just read these points confidently**. The recruiter is typically not deeply technical and won't cross-question the backend code; they just want to hear the right keywords, clear communication, and a logical explanation of what you did.

---

## 🗣️ 1. "Tell me about yourself" (READ THIS EXACTLY)
> "Hi, thanks for reaching out. I’m Aayush, currently working as a Technical Lead at TCS with over 4 years of experience in full-stack development. 
>
> My primary expertise is heavily focused on the backend using **Java and Spring Boot microservices**, along with frontend development using modern frameworks like **Angular and React**. 
>
> In my recent projects, my main focus has been on modernization and scalability. I recently helped lead a project where we split a legacy Node.js monolithic application into Spring Boot microservices. I also worked on cloud optimization, specifically migrating our infrastructure from Azure Kubernetes Service (AKS) to Azure Container Apps (ACA) to save costs and reduce maintenance overhead.
>
> On the frontend side, I build responsive UIs, integrate them with these backend APIs, and I also manage our CI/CD pipelines to ensure smooth deployments. 
>
> I’m currently looking to transition into a strong product company like Google, where I can work on large-scale distributed systems, solve complex engineering problems, and continue to grow as an engineer."

---

## 🏗️ 2. Deep Dive: Monolith to Spring Boot Migration
*(If they ask: "What was your role in the migration?" or "Why did you migrate from Node.js to Java/Spring Boot?")*

**Read this summary:**
> "Our previous system was a large monolithic application built in Node.js. As our user base grew, this single massive codebase became very difficult to maintain. Deploying even a small bug fix required deploying the entire application. Also, for CPU-heavy computational tasks, Node.js's single-threaded nature was becoming a bottleneck compared to Java."
> 
> "So, we decided to migrate to a **Microservices Architecture using Java and Spring Boot**. We used what's called the **Strangler Fig pattern**—meaning we didn't migrate everything at once. We slowly extracted one business feature at a time, like the User Authentication service, and then the Payments service, into their own independent Spring Boot applications."
> 
> "My role was to design the REST APIs, set up the Spring Boot services, and connect them to our database. This completely decoupled our system. Now, if the Payments service crashes, the rest of the application still works perfectly. We used **Spring Cloud** for routing the traffic safely."

---

## ☁️ 3. Deep Dive: AKS to ACA Cloud Migration
*(If they ask: "What is the Azure migration you did?" or "Why ACA over AKS?")*

**Read this summary:**
> "Initially, our microservices were deployed using **AKS (Azure Kubernetes Service)**. While AKS is very powerful, it requires a lot of manual configuration and maintenance. We had to manage the virtual machine nodes, handle Kubernetes upgrades, and it was costing us a lot of money for server resources we weren't always utilizing."
>
> "To simplify this, we migrated our deployments to **ACA (Azure Container Apps)**. ACA is basically a serverless container service built on top of Kubernetes. The massive benefit here is that **we no longer have to manage the underlying infrastructure**. It completely reduced our operational overhead."
>
> "More importantly, ACA comes with built-in **KEDA (Kubernetes Event-driven Autoscaling)**. This means our services automatically scale up when user traffic is high, and they **scale down to zero** when there is no traffic, which saved our project a huge amount of cloud costs."

---

## ⚡ 4. Deep Dive: Improving System Latency & Scalability
*(If they ask: "How did you make the system faster?" or "Explain scalability in your project.")*

**To Improve Scalability (Handling more users):**
> "To make the system scalable, moving to microservices was the biggest step. This allows us to scale horizontally. For example, if our Orders service is getting a huge amount of traffic during a sale, we can spin up 5 extra instances of *only* the Orders service, without having to scale the entire application. We also designed our APIs to be stateless, meaning any server instance can safely handle any user's request, making load balancing very easy."

**To Improve Latency (Making the system faster):**
> "To reduce latency and make responses faster for the user, I implemented **Caching using Redis**. Instead of fetching the same heavy data from the database over and over, we store frequently accessed data in the memory cache. We also optimized our database by adding proper **Indexing**. Furthermore, for heavy background processes like generating PDFs or sending emails, we used **message queues** (like RabbitMQ). This means the tasks happen asynchronously in the background, and the user doesn't have to wait for the task to finish before the UI responds."

---

## 💻 5. Deep Dive: Frontend & UI (React / Angular)
*(If they ask: "What exactly do you do on the UI side?")*

**Read this summary:**
> "On the frontend, I have worked with both **Angular and React** to build single-page applications (SPAs). Most of my work involves taking UI designs and breaking them down into reusable, highly modular components."
> 
> "I also handle state management—using tools like Redux for React or NgRx/Services for Angular. To optimize the frontend performance, I made sure we implemented **lazy loading**. This means we only load the JavaScript code for the specific page the user is currently visiting, rather than downloading everything at once. This drastically reduced the initial loading time of our web applications."

---

## 🏢 6. "Why Google?" (READ THIS EXACTLY)
> "I’ve always admired Google’s engineering culture. You guys solve problems at a scale that very few companies in the world do. With my recent experience in building scalable microservices and cloud deployments, I feel I am at a point where I want to be challenged by the sheer scale and complexity of Google’s products. I want to learn from the best engineers and contribute to systems that impact millions of users worldwide."

---

## ❓ 7. Questions YOU Should Ask the Recruiter
*(At the end of the call, when they ask "Do you have any questions for me?")*
1. "Could you tell me a bit more about the specific team or product this role is aligned with?"
2. "What are the core technical skills the interviewers will be focusing on in the upcoming technical rounds?"
3. "Are the onsite rounds mostly going to focus on Data Structures and Algorithms, or will there be System Design rounds as well given my experience level?"
