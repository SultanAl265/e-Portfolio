# Disaster Recovery (DR) Solutions Design and Review

---

## Q1: What is the impact of RPO and RTO values on DR solutions?

The **Recovery Point Objective (RPO)** and **Recovery Time Objective (RTO)** are critical parameters that directly influence the design and effectiveness of a disaster recovery (DR) strategy. RPO refers to the maximum acceptable amount of data loss measured in time, meaning how far back an organisation can afford to restore data after a disaster. For example, an RPO of 15 minutes requires near real-time data replication, whereas a 24-hour RPO can rely on daily backups (Wallace & Webber, 2017). RTO, on the other hand, defines the maximum acceptable time it takes to restore systems and resume operations after a disruption. Shorter RTOs require rapid failover systems and often involve higher infrastructure costs (Snedaker & Rima, 2014). Together, these metrics shape the DR solution by dictating the level of redundancy, data replication frequency, backup technologies, and investment required to meet business continuity goals.

---

## Q2: What are some typical DR system solutions used to meet various standby requirements?

Several DR system solutions are designed to meet different RPO and RTO requirements. **Cold standby** involves keeping backup systems offline until needed. It is cost-effective but has longer recovery times, making it suitable for non-critical systems. **Warm standby** keeps backup systems partially operational, reducing recovery time while maintaining moderate costs. **Hot standby (active-active)** solutions continuously replicate data and keep systems fully operational, allowing near-instant failover with minimal downtime, though at a higher cost (Wallace & Webber, 2017). Additionally, **cloud-based DR** solutions offer scalable and flexible alternatives by replicating workloads to cloud environments, providing faster recovery without heavy investment in physical infrastructure.

---

## Q3: What are the limitations of these DR solutions?

Each DR approach has its limitations based on cost, complexity, and performance. **Cold standby** solutions suffer from high RTO and potential data loss due to less frequent backups. **Warm standby** reduces downtime but may still involve manual intervention and limited automation. **Hot standby** delivers the best performance but requires significant investment and ongoing maintenance, which may not be feasible for all organisations. **Cloud-based DR**, while cost-effective and scalable, depends heavily on network connectivity and cloud service availability, and it may raise compliance and latency concerns (Snedaker, 2013). Therefore, organisations must carefully evaluate their RPO, RTO, budget, and risk tolerance when selecting a DR solution.

---

## References

- Snedaker, S. (2013) *Business Continuity and Disaster Recovery Planning for IT Professionals*. 2nd edn. Waltham: Syngress.  
- Wallace, M. & Webber, L. (2017) *The Disaster Recovery Handbook: A Step-by-Step Plan to Ensure Business Continuity and Protect Vital Operations, Facilities, and Assets*. 3rd edn. New York: AMACOM.
