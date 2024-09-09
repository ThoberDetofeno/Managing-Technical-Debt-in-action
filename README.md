# Managing technical debt in action: Process, Strategies and Tools

## Abstract
Context: Technical Debt (TD) is a metaphor that expresses the immaturity of software artifacts and their impacts on maintenance activities and product evolution. As organizations become able to identify and understand the effects of TD, challenges arise when making investment decisions to pay it off. Although several theoretical and practical studies have been developed recently, studies that adapt the context and stakeholders objectives for TD Management (TDM) are still lacking.

Objective: This paper aims to present an incremental and evolutionary TDM process, as well as strategies and tools. At each new iteration, or cycle, the results are evaluated, the objectives and the teams' capacity are reviewed to evolve in the TDM goal. The approach can be implemented as a whole or in parts, depending on the context and the goals of the organization.

Method: This research was developed using the action research method. Two cycles were carried out in partnership with a software development company over almost three years. The duration of each cycle was linked to the annual management cycle of the company involved in the research, which provides for the planning of goals and actions for the following year.

Results: As a result, a TDM process was proposed and validated. We found evidence that the defined process improved internal software quality with an annual decrease of ~65% in the most critical TD and a ~30% decrease in the average number of bugs identified per customer, leading to software product quality improvement.

Conclusion: The research presents a proposal for TDM with empirical evidence of use in the software industry. The process is detailed, as is the building path, the results are analyzed, and the decision-making processes are documented. This experience can help other software development companies in implementing TDM.

## Keywords: 
Technical Debt, Technical Debt Management, Source Code Technical Debt, Action Research on Technical Debt Management, Empirical studies in Technical Debt Management.

## 1. Introduction
Software development is a complex social task undertaken by people who cope with legacy requirements, evolving according to market expectations [1]. Software is rarely developed from scratch. Moreover, it changes in time, according to new and unpredictable requirements. Thus, maintenance is one of the most complex and costly phases of the software life cycle [2].

Maintenance activities are compromised when it is decided to sacrifice the quality of the software product to meet the pressures in delivery, generating the accumulation of problems, which worsen over time and lead to the emergence of what has been called Technical Debt (TD) [3].

The metaphor of TD appeared in 1992 by Ward Cunningham to describe, in financial terms, the increase in software development costs that is caused by the low quality of the source code [4]. According to Kruchten et al. (2012), TD still lacks a precise definition [5]. More recently, Avgeriou et al. (2016) [6] defined TD as “(…) a collection of design or implementation constructs that are expedient in the short term but set up a technical context that can make future changes more costly or impossible. TD presents an actual or contingent liability whose impact is limited to internal system qualities, primarily maintainability and evolvability.”

It is estimated that between 25% and 36% of all development time is wasted due to TD and that most of the time is wasted in understanding and/or managing TD [7, 8]. Studies show that the age of the software influences the amount of time spent to pay for the TD [9]. If unmanaged, TD can result in significant cost surpluses, serious quality problems, reduced developer morale [10], and limited ability to add new features [11]. It may even reach a crisis point when a huge and expensive refactoring or complete system replacement needs to be performed [12].

Because the internal quality aspects of the software do not generate revenues in the short term, developers and companies managers often disagree about decisions to invest resources in projects of this nature, which are crucial to the sustainability of the product but invisible to management and customers [5]. 
Technical Debt Management (TDM) includes identifying, monitoring, and paying TD items incurred in a system [13]. Its main goal is to enable decision-making about the need to eliminate a TD item (TDI) and the most appropriate time to do this [14]. According to Kruchten et al. (2012) [15], TD can be a good investment as long as the project team knows about its presence and the increased risks it imposes on the project. If properly managed, it can help the project achieve its goals sooner or more cheaply. Thus, the management of TD focuses on reducing its negative impact, being a decisive factor for software projects' success [16].

If TDIs are not managed, they can cause financial and technical problems, increasing software maintenance and evolution costs and leading to a crisis point where the entire future of the software will be compromised [17, 12]. Managing TD is necessary to keep it under control. TDM identifies the source of extra cost when changing software and analyzes when it is profitable to invest effort into improving the software system [18].

Aspects associated with TDM in a software development process are still less explored, according to Rios et al. (2021) [19]. According to Oliveira et al. (2015) [20], a strategy for managing TD is still a challenge, and its definition should be part of the software development process. Holvitie et al. (2018) [21] report that it remains unknown how TD manifests itself and affects software development processes.

After an organization understand the impacts of TD, it needs an efficient TDM to minimize losses. The success of TDM will depend on the effectiveness of the management structure, providing guidance, and a consistent process that ensures that TD is managed effectively, efficiently, and consistently with the organization's needs. But, as Rios et al. (2018) has identified, most approaches focus in a particular TDM problem (such as a TDM Activity, TDM Strategy with or without support tool) making it difficult to implement TDM in an organization.

The problem is TDM requires a holistic approach, that address all significant elements of how TD should be managed, and adapt to the context and the objectives of the organizations.

This research aims to define and implement an incremental and evolutionary process of Technical Debt Management in software development, validated in a real industry application context. This study includes a new process to manage TD, which can be used to guide the company in the search for better results, periodically reviewing the practices and decisions adopted. The process provides guidelines that can be tailored for other organizations or contexts.
The paper is structured as follows: Section 2 presents a review of the literature; Section 3 presents the research method; Section 4 describes the context and proposal of the research; Section 5 describes the first cycle of the action research; Section 6 presents the second cycle of the action research, and the process for managing TD is described in Section 7; Section 8 shows the discussions, comparisons with the related studies, and main contributions. And finally, Section 9 presents the conclusion and future works.
