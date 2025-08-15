# Threat Modeling Techniques and Their Application

Threat modeling is a structured approach for identifying, assessing, and mitigating potential threats to systems, applications, and processes. It helps organizations anticipate risks early and design security measures accordingly. Various techniques exist, each suited to different contexts, threat landscapes, and stakeholder needs.

---

## Threat Modeling Techniques

**STRIDE**  
Developed by Microsoft, STRIDE classifies threats into six categories: Spoofing, Tampering, Repudiation, Information Disclosure, Denial of Service, and Elevation of Privilege (Shevchenko et al., 2018). It is particularly effective in identifying security requirements in software development and assessing the impact of potential vulnerabilities.

**PASTA (Process for Attack Simulation and Threat Analysis)**  
A risk-centric model following a seven-stage methodology to align business objectives with security requirements (Shevchenko et al., 2018). Suitable for organizations needing a comprehensive, business-driven threat analysis that bridges technical risks with business impact.

**OCTAVE (Operationally Critical Threat, Asset, and Vulnerability Evaluation)**  
Developed by Carnegie Mellon’s Software Engineering Institute, OCTAVE emphasizes organizational risk management rather than focusing solely on technical vulnerabilities (NIST, 2022). It is valuable for enterprises where process maturity and policy evaluation are critical.

**Attack Trees**  
A hierarchical modeling method that visualizes how various attack paths can lead to a particular objective (Aven & Thekdi, 2025). Useful for breaking down complex threats and identifying countermeasures for each branch.

**VAST (Visual, Agile, and Simple Threat)**  
Tailored for Agile environments, integrating threat modeling into development workflows without disrupting delivery cycles (Tarandach & Coles, 2020). It supports scalability for large development teams and complex applications.

**LINDDUN**  
A privacy-focused framework categorizing threats as Linkability, Identifiability, Non-repudiation, Detectability, Disclosure of information, Unawareness, and Non-compliance (Shevchenko et al., 2018). Highly suitable for projects handling personal or sensitive data, aligning with regulatory requirements such as GDPR.

**DREAD (Damage, Reproducibility, Exploitability, Affected Users, Discoverability)**  
A numerical scoring model that ranks threats based on five factors to prioritize remediation efforts. While straightforward to apply, DREAD has been largely deprecated by Microsoft and is less common in modern practice due to subjectivity, inconsistent scoring, and lack of standardized weighting (Shevchenko et al., 2018). It can still be useful for **quick prioritization** in small teams or as a supplementary method to quantify risk after using qualitative models like STRIDE.

---

## Choosing the Right Technique

The selection depends on project scope, security process maturity, and expected threats:

- **STRIDE**: Best for the design phase of software projects to map threats to security requirements.
- **PASTA**: Ideal when deep business risk understanding is needed.
- **OCTAVE**: Suitable for organizations integrating security into governance and risk management.
- **VAST**: Fits fast-paced Agile environments.
- **LINDDUN**: Essential for privacy-centric systems like healthcare and finance.
- **Attack Trees**: Effective for penetration testing and red team exercises.
- **DREAD**: Useful as a secondary scoring mechanism when prioritization speed is critical.

---

## Hybrid Models

Combining techniques can address individual limitations and provide a more holistic threat perspective.

- **STRIDE + Attack Trees**: Classify threats first, then map attack paths in detail (Popov et al., 2022).
- **PASTA + LINDDUN**: Address business risks and privacy threats simultaneously.
- **OCTAVE + STRIDE**: Cover both governance-level and technical-level threats, useful in critical infrastructure projects (Aven & Thekdi, 2025).
- **STRIDE + DREAD**: Identify threats, then rank them numerically for remediation priority.

Hybrid approaches are beneficial when:
- A single method cannot fully address the threat landscape.
- Systems span multiple domains (technical, operational, regulatory).
- Stakeholders from various disciplines require tailored insights.

By adopting hybrid models, organizations can address both high-level business risks and granular technical vulnerabilities, ensuring comprehensive risk mitigation.

---

## Conclusion

No single threat modeling technique is universally superior. Effectiveness depends on alignment with project goals, threat types, and organizational maturity. Selecting the right model—or an appropriate hybrid—ensures thorough coverage and actionable outcomes, strengthening the overall security posture.

---

## References

- Aven, T., & Thekdi, S. (2025). *Risk Science*. Routledge.  
- NIST. (2022). *IT Laboratory Computer Security Resource Center*.  
- Popov, G., Lyon, B., & Hollcroft, B. (2022). *Risk Assessment*.  
- Shevchenko, N., et al. (2018). *Threat modeling: a summary of available methods*. Carnegie Mellon University Software Engineering Institute.  
- Tarandach, I., & Coles, M. (2020). *Threat Modeling*.  
