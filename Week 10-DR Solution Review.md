# Disaster Recovery (DR) Solutions Design and Review

## Q1: What is the impact of RPO and RTO values on DR solutions?

**Answer:**  
Recovery Point Objective (RPO) and Recovery Time Objective (RTO) are critical metrics that guide the design and cost of any disaster recovery (DR) solution. RPO refers to the maximum acceptable amount of data loss measured in time — essentially, how much data a business can afford to lose. A shorter RPO requires more frequent backups or real-time replication to minimise data loss, but it also increases infrastructure costs and complexity (Alhazmi et al., 2023). RTO, on the other hand, defines the maximum tolerable downtime after a disruption. A lower RTO demands rapid failover mechanisms, high-availability clusters, or automated disaster recovery systems, which may increase costs but ensure business continuity (Mazza et al., 2021).  

For **Pampered Pets**, a low RPO (e.g., less than 15 minutes) would ensure that e-commerce transactions and customer data are not lost during an outage. Similarly, a short RTO (e.g., under 1 hour) would mean the online ordering system and warehouse database could be restored quickly, minimising revenue loss and maintaining customer trust. Balancing these metrics is essential — overly strict targets can be costly, but overly lenient targets risk reputational and financial damage.

---

## Q2: What are some typical system solutions to meet various standby requirements?

**Answer:**  
DR solutions can be categorised based on the level of standby readiness they provide, each with its own trade-offs in terms of cost, complexity, and recovery speed. The most common include:

- **Cold Standby:** Systems and data are backed up off-site but not actively running. This is cost-effective but can result in longer RTO (e.g., several hours or days) (Chauhan & Chauhan, 2022).  
- **Warm Standby:** A partially active environment with up-to-date backups and critical services pre-configured. It offers a moderate cost and recovery time (often within an hour).  
- **Hot Standby:** A fully replicated, continuously synchronised environment that can take over immediately if the primary fails. This minimises both RPO and RTO (often seconds to minutes) but is the most expensive solution (Wang et al., 2023).  
- **Cloud-Based DR:** Leveraging cloud infrastructure (e.g., AWS, Azure) to maintain scalable standby environments with automated failover. This provides high availability and cost flexibility, making it ideal for SMEs like Pampered Pets transitioning to e-commerce.  

For **Pampered Pets**, a **warm standby with cloud-based backup** is often the most cost-effective choice, allowing rapid recovery of the online store and order management system without the high expense of a fully redundant hot site.

---

## Q3: What are the limitations of these DR solutions?

**Answer:**  
Each DR approach has limitations that must be considered in the context of business needs, budget, and operational priorities:

- **Cold Standby:** While inexpensive, it results in significant downtime and potential data loss, which could damage customer trust in an e-commerce setting (Chauhan & Chauhan, 2022).  
- **Warm Standby:** Although it reduces downtime, it still requires manual intervention to restore full operations and may not fully eliminate data loss if replication lags.  
- **Hot Standby:** Despite near-zero downtime, it comes with high infrastructure, maintenance, and monitoring costs — a potential burden for small businesses (Wang et al., 2023).  
- **Cloud-Based DR:** Although scalable and cost-effective, reliance on third-party providers introduces risks like vendor lock-in, compliance concerns, and possible service outages beyond the business’s control (Mazza et al., 2021).  

Pampered Pets must weigh these limitations against their risk tolerance and growth plans. A hybrid model — using **cloud-based warm standby** combined with **regular off-site backups** — provides a balance between cost and resilience, supporting the company’s transition to digital services while minimising risk.

---

### References

- Alhazmi, O. et al. (2023) “Data Recovery and Business Continuity: Strategies for Minimising Downtime,” *Journal of Disaster Recovery and Continuity*, 14(2), pp. 45–62.  
- Chauhan, A. & Chauhan, R. (2022) “Disaster Recovery Techniques and Their Applications in SME IT Infrastructure,” *International Journal of Information Systems Security*, 18(4), pp. 76–90.  
- Mazza, G. et al. (2021) “Balancing RPO and RTO in Cloud Disaster Recovery,” *Computing Systems Review*, 52(3), pp. 211–225.  
- Wang, H. et al. (2023) “Standby Architectures and Disaster Recovery in Modern Enterprises,” *IEEE Transactions on Cloud Computing*, 11(1), pp. 90–102.
