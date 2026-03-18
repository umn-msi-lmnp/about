# How We Work

*Roles, Goals, and Expectations*


<!-- mtoc-start -->

* [Introduction](#introduction)
* [Roles](#roles)
  * [The Principal Investigator (PI)](#the-principal-investigator-pi)
  * [The PI's Research Team](#the-pis-research-team)
  * [The MSI Informatics Team](#the-msi-informatics-team)
  * [The MSI Bioinformatics Analyst](#the-msi-bioinformatics-analyst)
* [Project Life Cycle](#project-life-cycle)
  * [Project Initiation](#project-initiation)
  * [How We're Funded](#how-were-funded)
  * [Assignment and Time Allocation](#assignment-and-time-allocation)
  * [Communication and Milestones](#communication-and-milestones)
* [An Example Project](#an-example-project)
* [Our Values](#our-values)
* [Conclusion](#conclusion)

<!-- mtoc-end -->



## Introduction

The Department of Laboratory Medicine and Pathology (LMP) and the Minnesota Supercomputing Institute (MSI) have formed a dedicated partnership to advance bioinformatics research and clinical diagnostics using NGS. This collaboration is focused on discrete "projects," broadly defined in two main categories.

1. Research: Supporting bioinformatics-based research projects initiated by LMP Principal Investigators (PIs).
2. Clinical: Developing and maintaining CLIA-validated and CAP-certified pipelines for somatic and germline variant testing.

Our LMP bioinformatics team includes five analysts working within MSI’s Research Informatics (RI) – Bioinformatics division. Our research and clinical efforts differ in structure and scope. For research projects, we typically collaborate with principal investigators (PIs) and their lab members on discrete, month-to-month efforts that can be extended as needed. In contrast, development of clinical pipelines is an iterative and ongoing process that depends on input from multiple stakeholders, including members of the Fairview Molecular Diagnostics Laboratory (MDL).

This document outlines how we work: our roles, project goals, values, and expectations when partnering with collaborators. It builds on elements of the MSI/LMP Memorandum of Understanding (MOU) and provides practical guidance for day-to-day collaboration.


## Roles

The purpose of this section is to define the general expectations for each role category.

### The Principal Investigator (PI)

- Defines the research question and overall goals
- Provides experimental context and input on results
- Supplies funding or support for analyst time (or secures financial support from the LMP Department)
- Directs the publication process

### The PI's Research Team

- May include postdocs, graduate students, lab scientists, or outside collaborators
- Engages with analysts on project-specific details
- Helps with data interpretation and generating follow-up questions
- Supplies important metadata, wet-lab manuals/methods
- Manages communication with other collaborators (e.g. UMGC/BPIC/UIC)
- Is responsible for generating final "publication-ready" figures

### The MSI Informatics Team

- Includes the LMP bioinformatics manager, other MSI analysts, and core staff (e.g., UMGC contacts)
- Offers technical guidance and shares previous experience with the primary analyst at multiple weekly group meetings (or whenever needed)
- If a project needs to switch analysts, we all work together to maintain a smooth transition
- The LMP bioinformatics manager is responsible for assigning an analyst to a project based on timing and best fit
- The LMP bioinformatics manager is available to support the dedicated analyst and/or the PI team if communication or technical issues arise


### The MSI Bioinformatics Analyst

- Advises on experimental design and feasibility (communicates the plan and adapts based on PI feedback)
- Designs and executes the code for the analysis
- Presents findings and next steps via weekly meetings
- Uses the high-performance computing (HPC) and core infrastructure at MSI or other University resources
- Provides customized expert analysis using the most appropriate tools and methods
- We view our work as a research collaboration




## Project Life Cycle

### Project Initiation

Projects begin when a PI reaches out to the LMP bioinformatics manager (Todd Knutson <knut0297@umn.edu>) to discuss a research or clinical question. Ideally, we'd meet prior to sequencing to discuss:

- Project scope and objectives
- Experimental design
- Sequencing strategies
- Timelines
- Roles and responsibilities

### How We're Funded

We are employees of MSI and our effort is supported by the Department of Laboratory Medicine. If you need support, email the LMP bioinformatics manager (Todd Knutson <knut0297@umn.edu>) to get started. Depending on the project, our work is funded in three main ways:

- PIs can request a *Letter of Support* from MSI (Research Computing) for their grant applications.
    - This letter describes the compute resources available at MSI, and how bioinformatics analysts can support the specific project.
    - The letter ends by listing the percentage of analyst effort needed for the project per year (e.g. 25% of an analyst's effort per year).
    - After the grant is funded, we will support the project as requested (with flexible scheduling over the grant period).
- PIs can provide a UMN chart string account number and schedule specific support time.
- PIs can request free support from the LMP department (typically one month). [Details are described here](https://med.umn.edu/pathology/research/research-support) (expand the second section: *Research Bioinformatics Support*).


### Assignment and Time Allocation

An analyst is assigned to the project based on their availability, interest, experience, and/or best fit. Assignments are typically planned in monthly increments, with regular reviews of progress and needs. Dedicated time is frequently extended (2+ months) depending on funding and project complexity. The bulk of the work needs to be done within the dedicated time allocation, but we also can follow up on projects on an ad hoc basis. We call this effort "office hours" time and limit that to 4 hours or less per week, for all non-dedicated projects. This time is useful for regenerating results based on small changes (i.e. redoing a heatmap, etc.). PIs should simply ask for what they need, and we'll do our best to estimate whether the work can be done in office hours or requires dedicated time.

### Communication and Milestones

We maintain regular communication through meetings, email, and shared documentation.

- Analysts provide updates on progress, request clarification when needed, and document all methods (primarily in code).
- We sync our project code with GitHub and provide collaborators access to the online repository.
- Deliverables are shared in stages (usually weekly), with an emphasis on clarity, reproducibility, and feedback.
    - Generally, this work is exploratory in nature, so we generate several intermediate results that are reviewed and revised as a group.
- Data are processed and stored on MSI systems and everyone is expected to access the files from that system.
    - There are several ways to access MSI, but [Open OnDemand](https://ondemand.msi.umn.edu/) (OOD) web app is the easiest way to browse files





## An Example Project

Our work is structured differently than most academic environments. It can be considered closer to consulting, but since we work with many of the same PIs repeatedly, we invest time in learning the PI's research biology at a deeper level. Below is a general description of how we approach and analyze a new project. We've added several details around communication, what types of work we do, and some things we leave for our PI teams to handle.


- The PI has a new single-cell analysis they would like analyzed
    - The PI contacts the LMP bioinformatics manager (email) to inquire about feasibility
    - A brief meeting is held to discuss priorities, experimental design, timelines, etc.
    - Funding for bioinformatics time is discussed and secured; a start time and analyst are agreed upon
- The PI research team communicates with UMGC about sequencing timelines, samples, etc.
    - The PI research team should forward emails from UMGC regarding the location of output files
- A meeting is held between the analyst and PI's research team before (or at the start) of the dedicated time to plan priorities
- The analyst starts the work
    - This may require building our own tools
    - It may require using stable (older) tools
    - It may require using cutting-edge untested methods
- The analyst may need to review some wet-lab procedures (e.g. sequencing library specifics) and integrate these features into the analysis
- Communication timing may be non-linear, but when important feedback is needed, we connect as soon as possible and maintain professional, collaborative communication
    - The analyst generates timely results, communicates roadblocks as soon as possible, and attempts to reply to emails within one business day (during working hours)
- Weekly meetings are scheduled (approximately) to review the project status and update priorities
    - This may include the analyst presenting output files via a file browser (e.g. Open OnDemand)
    - A presentation (i.e. PPTX) or Markdown summaries may be effective in rough-draft format (but we want to communicate exploratory results quickly and limit extra work). We will not always generate these documents. Our goal is to move quickly through the exploratory phase of an analysis and not polish reports (at this stage). Each project is different, and sometimes these can help guide the priorities, other times they are not needed.
    - Email summaries (bullet points) can be helpful for tracking what was done, and where the focus needs to be (in addition to, or following, meetings)
- The analyst has a commitment to robust, scalable, and interpretable analysis
- The analyst and bioinformatics team do their best to set realistic timelines and expectations, and communicate honestly if roadblocks occur
- The analyst ensures data continuity, backups, transparency, and reproducibility
  - The entire project (inputs, code, results) are saved in the PI-owned MSI storage space
  - All project code will be synced with GitHub.com (and access provided to the PI research team)
  - Raw data (e.g. FASTQs) are backed up into PI-owned MSI Tier 2 buckets
  - Project results are eventually backed up to PI-owned MSI Tier 2 buckets
  - The location of these backups will be included in the project README file
- The PI research team and the Informatics team will determine when the project is sufficiently complete (i.e. no longer requires dedicated effort)
- Office hours tasks can be requested of the bioinformatics analyst
    - Frequently, sequencing data needs to be deposited to public databases, including GEO, SRA, or dbGaP.
    - This can be an office hours request, but it will take several hours to complete. The PI research team should communicate this need as soon as they know what samples they plan to publish. We can always keep the data private until the papers are published/public.
- If the bioinformatics results are included in a manuscript:
    - We use the same criteria as most journals for authorship. If we provide an intellectual contribution, we expect to be included as an author in the publication.
    - The bioinformatics analyst will write a custom methods section for any results included in publications
      - Writing a separate methods section for all analysis is not generally useful
      - Broad summaries become out of date (incorrect) quickly
      - We will rely on our code to be the true source for analysis methods
    - We will provide critical review of the entire manuscript (with a special focus on the bioinformatics). We ensure the publication aligns with current bioinformatics language/presentation styles
    - We will upload raw data to the databases and share code however needed by the publisher (e.g. GitHub, Zenodo, etc.)
- Our primary goal for the collaboration is completing the analysis
    - Generally, we do not provide coding/bioinformatics training for the PI research team. All of our work is open and shared, but we cannot spend substantial time teaching others how to do this work




## Our Values

- **Clarity:** Code, reports (emails, etc.), and decisions should be understandable now and in the future (especially by our future selves).
- **Collaboration:** We work _with_ teams, not _for_ them. We want to be a close partner in your research and understand your issues at a deep level. This approach allows us to find the best-fit solutions for your project, versus just being assigned tasks.
- **Integrity:** We admit mistakes quickly and operate within our areas of expertise.
- **Trust:** We maintain consistent, professional communication and follow through on commitments. We will voice any analysis concerns if they arise.
- **Innovation:** We stay current with bioinformatics and wet lab methods.
- **Respect:** Everyone brings expertise (scientific, clinical, or technical), regardless of role or status, and we listen and consider multiple perspectives.
- **Creativity and Autonomy:** Analysts have room to explore better approaches and suggest new ideas.
- **Feedback:** We encourage feedback from our collaborators and coworkers, and are empowered to share feedback with them.

## Conclusion

This document sets a foundation for collaboration and helps clarify how the LMP bioinformatics team contributes to research success. By aligning our goals with shared expectations and values, we hope to deliver rigorous, timely, and impactful work across all our projects. We review and update this document annually.
