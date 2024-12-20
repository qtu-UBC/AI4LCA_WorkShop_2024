# AI4LCA Workshop 2024: Accelerating Sustainability Through AI-Powered Life Cycle Assessment

![group photo](https://grouptu.sites.olt.ubc.ca/files/2024/12/IMG_9263-scaled.jpg)
## *TL'DR*
The workshop underscored the need for a collaborative effort between academia, industry, and policymakers to address data scarcity, develop robust benchmarking methods, and ultimately leverage LCA to drive meaningful decarbonization across diverse sectors. The integration of AI is essential to scale LCA and maintain human-centered verification and avoid biased outputs.

## Key Themes & Insights
### LCA in Practice: Challenges and Opportunities
- Resource Intensive: LCA is acknowledged as both resource and data-intensive. The cost of acquiring data and performing detailed analysis is a major hurdle. 
- Data Scarcity & Quality: A recurring problem is the scarcity of high-quality, up-to-date data, particularly for emerging technologies and specific impact categories like water contamination and human health. 
- Scaling Issues: Manually conducting LCAs for millions of products is not scalable. There's a strong push for automation of LCA processes using AI.

### Emission Factor Recommendation
- EF Selection Bottleneck: The manual selection of emission factors is time-consuming, requires expertise, and is prone to inconsistencies.
- "Parakeet": An algorithm using embeddings and LLMs was proposed for automated EF selection. It includes a retrieval stage (identifying semantically similar EFs) and a generation component (LLM recommendation with justification).
  - [Article](https://www.amazon.science/publications/parakeet-emission-factor-recommendation-for-carbon-footprinting-with-generative-ai)
- Performance: "Parakeet" achieved a precision@1 of 92% for spend-based EFs and 72-74% for process-based EFs in initial benchmarking.
- Challenges: Errors included misinterpretations of text, failing to identify when "no match" is appropriate, and annotation errors. This highlights the need for continued improvement and human oversight. 

### LCA Quality
- Contextual Quality: The definition of "quality" in LCA is heavily context-dependent, and related to the intended use of the model. The panel questioned, "what is good enough? 
- Resource Constraints: Sustainability teams in companies often have limited resources and time, making it difficult to collect high-quality data for every component.
- Directional Accuracy: The panel emphasizes "directionality" as a key aspect of quality. It is important to be confident that the proposed changes will actually reduce emissions.
- Uncertainty Management: Uncertainty is inherent in LCA, particularly with scaling. It's critical to determine acceptable levels of uncertainty and identify where to focus data collection. "If you have meticulous activity data, then it is straightforward to calculate uncertainty. But that is not practical."
  - A relevant study: [“Exploring the Viability of Probabilistic Under-Specification To Streamline Life Cycle Assessment”](https://pubs.acs.org/doi/10.1021/es3042934)
- Continuous Improvement: The emphasis is on iterative improvement rather than achieving a "perfect solution" immediately. The goal should be a "directionally correct" approach that is refined over time. "Instead of trying to build a perfect solution, start from what you have and improve on it."
- Benchmarking: The workshop highlighted the need for robust benchmarking, both to assess performance and to guide decisions. As noted in multiple sessions: "How can we determine that a system is performing at the level you wanted to? How do we do that at scale?" and "We also need to be able conduct benchmarking at scale".
- Metrics for AI-Powered LCA Systems: While metrics like precision and recall are standard for AI/ML, they don't fully capture the complexities of LCA.
- Auditability & Traceability: Critical aspects include the auditability of processes, lineage of data, and complete validation fields. "Have the ability of auditability of human processes will be critical to understand how we automate it."
- Standardization: There is a call for machine-readable data schema, pre-vetting assumptions, and standardizing the LCA process.
- Human Oversight: The role of human verifiers is crucial to address bias in AI-generated results. 

### LCA Data Availability
- Scattered & Unstructured Data: Data is often scattered, unstructured, and not easily comparable. Different LCAs may include or exclude specific factors, making direct comparisons challenging. 
- Schema Development: Creating metadata schemas for specific domains (e.g., buildings) is a potential solution to facilitate data sharing and interoperability. 
  - Relevant information
    - [“Elementary flow mapping across life cycle inventory data systems: A case study for data interoperability under the Global Life Cycle Assessment Data Access (GLAD) initiative”](https://link.springer.com/article/10.1007/s11367-024-02286-x)
    - [“A Shared Semantic Vocabulary as a Path Forward for Harmonized Inventory Data”](https://zenodo.org/records/14196000)
    - [“The Data Liberation Toolkit - An Open Source Set of Tools for Harmonization and Maintenance”](https://zenodo.org/records/14197043)
- Supplier Data Issues: Data from suppliers often arrives as spreadsheets with manual errors, requiring extensive processing. Also, there is a struggle to get the right attributes for carbon predictions from suppliers.
- Proprietary Data: Proprietary data poses a challenge to open access and the development of shared benchmarks.
- Need for Benchmarking: Access to vetted data is crucial for developing and comparing different LCA methodologies. "If we are to come up with the right methods, we need access to the data that has been vetted. Then we start comparing against the same data."
- Crowdsourcing: The idea of using Amazon Mechanical Turk-like platforms for crowdsourcing LCA data was suggested.
- "Ground Truth" Challenge: Finding a true "ground truth" for LCA is difficult, as many values are based on models and assumptions. Consistent methodology is seen as more important than achieving perfect accuracy, to allow for measurable progress. 

### Decarbonization with LCA
- Data Collection Bottleneck: The time and effort involved in data collection is a significant barrier.
- Generative AI: There's potential for generative AI to create models of industrial processes, including new materials and properties.
- Real-time Data: The need for real-time data for operational decarbonization was raised, particularly for sectors like buildings.
- Beyond Carbon: A move towards considering other environmental impacts beyond carbon was suggested, as well as a better understanding of the trade-offs of different decisions. 
- Scaling Challenges: Scaling LCA across sectors requires considering consequential LCA and system-level interactions, not just individual products.
- Linking LCA and Cost: It is critical to link LCA with cost and business benefits to encourage adoption. It was discussed that a "TEA" (Techno-Economic Assessment) should go hand-in-hand with LCA.
- Policy Drivers: Policy is seen as a major driver for the adoption of LCA. 

### Actions
- Future R&D:
  - [Evaluation] Develop metrics to evaluate the quality of an LCA
  - [Validation] Use AI to automate the critical review process (which is essentially a collection of heuristics developed by LCA practitioners)
-   Create a community that co-evolves scientific breakthrough (e.g., new algorithm for generating data) with industrial pilot-testing (e.g., to provide real world benchmark data)

### Additional resources
- 🤖 [Applications of AI in streamlining the LCA modeling](https://lnkd.in/gtwze-6N) [Recording]
- 🔢 [Data, Algorithm, Tools for LCA: Challenges, Opportunities, and Consensus of LCA Data](https://lnkd.in/g8aWdbAJ) [Recording]
- 🛠 [Next-Gen LCA Tools: Unveiling the Latest Developments and Solutions](https://lnkd.in/ggXBPdxY) [Recording]

### Future events
- [1-4 July 2025] 12th International Conference on Industrial Ecology: https://isie2025.sg/. Featuring Special Session(s) on AI, Data and Tools. Abstract submission deadline: Dec.31, 2024
- [16-18 June 2025] International Symposium on Sustainable Systems and Technology (ISSST) 2025 Conference: (https://issst.net/). Featuring Theme "Innovative Tools and Methods in LCA and Sustainability Analysis". Abstract submission deadline: Jan.17, 2025


-----------
## Overview
Life cycle assessment (LCA) is a crucial tool for understanding and mitigating the environmental impact of products and services. However, the complexity and data-intensive nature of LCA pose significant challenges in scaling sustainable solutions.

The AI4LCA Workshop 2024 aims to harness the power of artificial intelligence (AI) to streamline and enhance the LCA process. By bringing together leading experts in AI and LCA, this event will explore how cutting-edge AI techniques can be leveraged to address the grand challenges faced by LCA researchers and practitioners.

The workshop's key objectives are to:

- Identify the fastest pathways to decarbonization and how AI can simplify LCA to accelerate sustainable transformation.

- Discuss critical scaling challenges in LCA (e.g., data availability, interoperability).

- Establish a shared understanding of LCA ground truth, performance metrics, and "good enough" standards.

- Foster collaboration on data exchange, benchmark datasets, and innovation-driving competitions.

- Coverage across diverse industry domains and best practices for cross-sector implementation.

By facilitating meaningful dialogue and showcasing the latest advancements, the AI4LCA Workshop 2024 aspires to catalyze the widespread integration of AI into the LCA workflow, ultimately empowering organizations and policymakers to make more informed, data-driven decisions that accelerate the transition to a sustainable future.

## Date and Location
**Date:** December 14, 2024  
**Location:** Ponderosa Commons North ([venue photo](https://hostatubc.com/venues/ponderosa-ballroom/), [map](https://www.maps.ubc.ca/?code=PCN), address: 6445 University Blvd, Vancouver, BC), University of British Columbia, Vancouver, Canada <br>
**Parking:** Closest location is UBC West Parkade (2140 Lower Mall, Vancouver, BC V6T 1Z2), and the rate is $2.00 for 1/2 hr - Max $10 23:59 for weekends. For more information related to parking at UBC, please refer to: https://parking.ubc.ca/map

The workshop is **in-person only**; there will be no virtual attendance option.

## Agenda

### Morning Session
9:00 - 9:15 AM: Coffee social

9:15 - 9:45 AM: Welcome and Opening Remarks
- Qingshi Tu, University of British Columbia

9:45 - 10:15 AM: LCA Practice in Industry
- Lin Shi, Amazon

10:45 - 11:15 AM: Emission Factor Recommendation
- Fahimeh Ebrahimi, Amazon
- Nina Domingo, Amazon

11:15 - 11:45 AM: *Coffee break*

11:45 AM - 12:45 PM: Panel Discussion - LCA Quality
- Panelists
  - Valerie Thomas, Georgia Tech
  - Jeremie Hakian, Amazon
  - Valentina Prado, Sphera
  - Harris Chalat, Muir.ai
- Moderator: Ethan Roday, Amazon

### Afternoon Session
2:00 - 3:00 PM: Panel Discussion - LCA Data Availability
- Panelists
   - Shaena Ulissi, Watershed
   - Yuvraj Agarwal, Carnegie Mellon University
   - Anran Wang, Amazon
- Moderator: Kellen Axten, Amazon

3:00 - 3:30 PM: *Coffee break*

3:30 - 4:30 PM: Panel Discussion - Driving Decarbonization with LCA
- Panelists
  - Prashant Shenoy, University of Massachusetts at Amherst
  - Bichlien Nguyen, Microsoft
  - Miguel F. García Claro, Bombardier
  - Qingshi Tu, University of British Columbia
- Moderator: Andrew Dumit, Watershed


4:30 - 5:00 PM: Closing Remarks and Next Steps

### Happy Hour
5:30 - 8:00 PM at [Browns Crafthouse UBC](https://www.brownscrafthouse.com/)

## Registration
**Nov 15, 2024**. Registration is closed. 

## Organization
[Qingshi Tu](https://forestry.ubc.ca/faculty-profile/qingshi-tu/) and [Bharathan Balaji](https://www.linkedin.com/in/bharathanbalaji/)
