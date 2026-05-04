# Interview Q&A Preparation Notes

## 1. Introduction
**Q:** Tell me about your background.

**A:**
I’m a Lead Full-Stack Engineer with 15+ years of experience working with Java Spring Boot microservices and React applications. Currently, I work at Highmark Health building large-scale healthcare systems supporting claims processing and enrollment. My focus is on scalable APIs, performance optimization, cloud deployment (AWS, Docker), and building resilient distributed systems.

---

## 2. Project Deep Dive
**Q:** Describe a project you are proud of.

**A:**
Worked on a claims processing system using microservices and Kafka. Designed scalable APIs, implemented event-driven architecture, and optimized performance. The system supported high traffic with strong reliability and improved operational efficiency.

---

## 3. High Volume & Resiliency
**Q:** How did you handle high traffic and resiliency?

**A:**
Used microservices, Kafka for async processing, horizontal scaling, circuit breakers, retries, and observability tools. Ensured idempotency and implemented load balancing with auto-scaling.

---

## 4. Kafka Design
**Q:** Explain Kafka setup (topics, partitions, consumers).

**A:**
Used topic-based event flow (claims-submitted, processed, etc.), partitioned by claim ID, scaled consumers via consumer groups, handled lag via scaling and optimization, and used DLQs for bad data.

---

## 5. CI/CD Tools
**Q:** Favorite vs least favorite CI/CD tool?

**A:**
Favorite: GitHub Actions (easy integration, debugging, reusable workflows).
Least: Jenkins (complex, plugin issues, maintenance overhead).

---

## 6. Canary Deployments
**Q:** Experience with canary deployments?

**A:**
Implemented progressive rollout (10%, 25%, etc.), monitored via Prometheus and Grafana, used alert-based rollback, and relied on human + automated validation.

---

## 7. Deployment Duration
**Q:** How long does deployment take?

**A:**
Typically 1–2 hours end-to-end, including CI, staging, and canary rollout.

---

## 8. Canary Failure Scenario
**Q:** Did canary ever fail?

**A:**
Yes, due to a data edge case causing latency issues. Canary detected early, rollout stopped, rollback executed, and fix applied.

---

## 9. On-call Experience
**Q:** Describe your on-call experience.

**A:**
Handled production alerts, triaged incidents, stabilized systems, and performed root cause analysis. Focused on reducing alert fatigue and improving reliability.

---

## 10. Major Incident
**Q:** Describe a severe incident.

**A:**
Kafka consumer lag caused claims delay. Scaled services, paused ingestion, rolled back deployment, identified inefficient logic, and fixed root cause.

---

## 11. Spring Boot DB Issue
**Q:** Connection pool exhausted issue?

**A:**
Likely DB connection exhaustion due to leaks or slow queries. Checked pool metrics, DB health, logs. Restarted service, scaled, and later fixed root cause.

---

## 12. Chaos Engineering & SRE
**Q:** Thoughts on chaos engineering?

**A:**
Supports fail-fast culture. Helps improve MTTD/MTTR. Focus on automation, self-service tooling, and tying experiments to real incidents.

---

## 13. Questions Asked to Interviewer
- How is reliability measured?
- How does on-call rotation work?
- What deployment strategies are used?
- What does success look like in 3–6 months?

---

## 14. Closing Statement
**A:**
I really enjoyed the discussion. The work around reliability, chaos engineering, and high availability aligns strongly with my experience. I’m excited about the opportunity and look forward to next steps.
