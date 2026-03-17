# How We Work: Roles, Goals, and Expectations

<!-- mtoc-start -->

* [Introduction](#introduction)
* [Clear break between research and clinical](#clear-break-between-research-and-clinical)
* [Clear break between research and clinical](#clear-break-between-research-and-clinical-1)
* [Roles](#roles)
  * [The Principal Investigator (PI)](#the-principal-investigator-pi)
  * [The PI's Research Team](#the-pis-research-team)
  * [The MSI Informatics Team](#the-msi-informatics-team)
  * [The MSI Bioinformatics Analyst](#the-msi-bioinformatics-analyst)
    * [Our Goals](#our-goals)
* [Working with sensitive data (IRB)](#working-with-sensitive-data-irb)
* [GEO/SRA/dbGaP submissions, when? embargos, should be uploaded with lead time.](#geosradbgap-submissions-when-embargos-should-be-uploaded-with-lead-time)
* [Authorship](#authorship)
  * [What We Provide](#what-we-provide)
* [What You Must Provide](#what-you-must-provide)
* [Project Lifecycle](#project-lifecycle)
  * [Project Initiation](#project-initiation)
* [Project Lifecycle](#project-lifecycle-1)
  * [Project Initiation](#project-initiation-1)
* [TODO Timelines, Deadlines -- really hard to define (especially for clinical pipelines).](#todo-timelines-deadlines----really-hard-to-define-especially-for-clinical-pipelines)
* [Data backup](#data-backup)
* [Manuscript prep and review](#manuscript-prep-and-review)
* [Expectations and Responsibilities](#expectations-and-responsibilities)
* [Project Life Cycle](#project-life-cycle)
  * [Project Initiation](#project-initiation-2)
  * [Assignment and Time Allocation](#assignment-and-time-allocation)
  * [Communication and Milestones](#communication-and-milestones)
* [How we're funded](#how-were-funded)
* [Our Values](#our-values)
* [Conclusion](#conclusion)

<!-- mtoc-end -->

## Introduction

The Department of Laboratory Medicine and Pathology (LMP) and the Minnesota Supercomputing Institute (MSI) have formed a dedicated partnership to advance bioinformatics research and clinical diagnostics using NGS. This collaboration is focused around working on discrete "projects," broadly defined in two main categories.

1. Research: Supporting bioinformatics-based research projects initiated by LMP Principal Investigators (PIs).
2. Clinical: Developing and maintaining CLIA-validated and CAP-certified pipelines for somatic and germline variant testing.

Our LMP bioinformatics team includes five analysts working within MSI’s Research Informatics (RI) – Bioinformatics section, which comprises approximately 20 analysts in total. This document outlines how we work: our roles, project goals, values, and expectations when partnering with collaborators. It builds on elements of the MSI/LMP Memorandum of Understanding (MOU) and provides practical guidance for day-to-day collaboration.

<<<<<<< HEAD
## Clear break between research and clinical

Our group of five analysts supports both research and clinical efforts, which differ in structure and scope. For research projects, we typically collaborate with principal investigators (PIs) and their lab members on discrete, month-to-month efforts that can be extended as needed. In contrast, development of clinical pipelines is an iterative and ongoing process that depends on input from multiple stakeholders, including genetic counselors, collaborators in the Advanced Research and Diagnostics Laboratory (ARDL), and members of the Molecular Diagnostics Laboratory (MDL). Analysts contributing to clinical projects ultimately report to the LMP bioinformatics supervisor as well as the director of the MDL.

||||||| parent of 0bb4519 (Todd's refactoring)
## Clear break between research and clinical


=======
>>>>>>> 0bb4519 (Todd's refactoring)

## Roles

There are approximately four role categories for work in our group. Each category has some flexibility (especially, between research or clinical projects). However, the purpose of this section is to define the general expectations for each category.   

### The Principal Investigator (PI)

- Defines the research question and overall goals
- Provides experimental context and input on results
- Supplies funding or support for analyst time (or secures [financial support from the LMP Department](https://med.umn.edu/pathology/research/research-support))
- Is responsible for scientific integrity and directs the publication process

### The PI's Research Team

- May include postdocs, graduate students, or lab scientists
- Engages with analysts on project-specific details
- Helps with data interpretation and generating follow-up questions
- Supplies important metadata, wet-bench manuals/methods
- **Manages communication with other collaborators** (e.g. UMGC/BPIC/UIC)
- Is responsible for generating final "publication ready" figures

### The MSI Informatics Team

- Includes the LMP bioinformatics manager, other analysts, and core staff (e.g., UMGC contacts)
- Offers technical guidance and relates previous experience to the primary analyst at weekly group meetings (or whenever possible)
- If a project needs to switch analysts, we all work together to maintain a smooth transition
- The LMP bioinformatics manager is responsible for assigning an analyst to a project based on timing and best fit
- The LMP bioinformatics manager is available to support the dedicated analyst and/or PI team if communication or technical issues arise  


### The MSI Bioinformatics Analyst

#### Our Goals

- Advises on experimental design and feasibility (communicates the plan and adapts based on PI feedback)
- Architects and executes the code for the analysis. However, we generally use a structure optimized for reproducibility:
  - input files (provided to us, or generated without code)
  - source code
  - output files generated by code only
  - metadata (any other related files not used directly as inputs)
- Presents findings and agree on next steps via weekly meetings
  - This may include walking through output files via file browser
  - A presentation (i.e. PPTX) may be effective in rough-draft format (but we want to communicate exploratory results quickly and limit extra work)
  - Markdown or AI summaries could also be helpful communicating dynamic updates
    - Email summaries (bullet points) can be helpful for tracking what was done, and where the focus needs to be
- Communication timing may be non-linear, but when important feedback is needed, we connect as soon as possible
    - Maintains professional and collaborative communication
    - Generates timely results and communicates roadblocks as soon as possible
    - We attempt to reply to emails within 1 day or less (during working hours)
- Writes a custom methods section for any results included in publications
  - Writing a separate methods section for all analysis is not generally useful
  - These summaries become out of date (incorrect) quickly
  - We will rely on our code to be the correct source for analysis methods
- Use the high-performance computing (HPC) and core infrastructure provided by MSI or other University resources
- All project code will be synced with GitHub.com
- Ensures data continuity, backups, transparency, and reproducibility
  - Raw data (e.g. FASTQs) are backed up into PI-owned MSI Tier 2 buckets
  - Project results are eventually backed up to PI-owned MSI Tier 2 buckets
  - The location of these backups will be included in the project README file
- Our interactions are collaborative, but are not focused on training others (we support projects, but not long-term, hands-on training of collaborators or their teams)
- Commitment to robust, scalable, and interpretable analysis

## Working with sensitive data (IRB)

## GEO/SRA/dbGaP submissions, when? embargos, should be uploaded with lead time.
- What is our role, what is lab memeber's role


## Authorship
- we're scientific collaborators, not analysts for hire
- Who we are?! We're staff scientists,
- What is our role with trainees?
- we produce data using best practices, but we're 

#### What We Provide

- Customized expert analysis using the most appropriate tools and methods
  - This may require building our own tools
  - It may require using stable (older) tools
  - It may require using cutting-edge untested methods
- Experimental design consultation
- Comprehensive and reproducible workflows
- Reports
  - Comprehensive reports may be needed for certain activities (documentation of a clinical pipeline)
  - In other cases, simplified summaries via email, Google Doc, or README files will be sufficient
  - We aim to balance time spent documenting results vs writing clear and concise code that can be reviewed by anyone
- Grant and manuscript support
- Data management and continuity between analysts
- Reviewing wet lab procedures (e.g. sequencing library specifics) and integrating these features into the analysis
- Best practices in method selection and documentation
- Responsiveness and adaptability to project needs

## What You Must Provide

- Final edits of .pdf outputs requiring Adobe Illustrator or similar tools
  - Our goal is to get a figure 80% there, but resizing, font changes, etc. are best done in dedicated tools.
- Specialized subject matter expertise on a project's biology
  - We can cover the informatics and general biology, but we are not experts on each lab's specific topics

## Project Lifecycle

### Project Initiation

Projects typically begin when a PI reaches out to discuss a research or clinical question. We meet to review:

- Experimental design
- Project scope and objectives
- Timelines
- Roles and responsibilities

When does this happen? 
- Ideally an initial project meeting will occur before the sequencing experiment has started, this allows analysts to provide input on ideal numbers of biological replicates, sequencing design and more
- Depending on other projects we have in the queue it may be a couple of months before we can schedule a project, so meeting early helps set expectations about when we can complete the work
- 
Communication  
- Style and frequency of communication will vary by PI preference buy typically includes regular email updates and/or meetings, either in person or via Zoom

## Project Lifecycle

### Project Initiation

Projects typically begin when a PI reaches out to discuss a research or clinical question. We meet to review:

- Experimental design
- Project scope and objectives
- Timelines
- Roles and responsibilities

TODO: communication style and frequency
TODO: When we should talk? Before, during, after... (define all of those)
TODO: what background reading do we do? Do we do a lot of background? or focus more on the tools? 
TODO: our job is to get the data analyzed correctly 
TODO: we may not be able to "give the answer" -- set realistic expections

In particular, our analysis is often in the  


## TODO Timelines, Deadlines -- really hard to define (especially for clinical pipelines).
- TODO: Creating arbitray deadlines is not helpful
- TODO: Include manager in strict deadline decisions
- TODO: do we want to write statements of work?
- "custom" bioinformatics, not just running pipelines, we're cross-disciplinary
- we're not algorithm developers (per se!)

## Data backup

## Manuscript prep and review
 

## Expectations and Responsibilities
## Project Life Cycle

### Project Initiation

Projects typically begin when a PI reaches out to discuss a research or clinical question (contact Todd Knutson <knut0297@umn.edu> to get started). We meet to review:

- Experimental design
- Sequencing strategy
- Project scope and objectives
- Timelines
- Roles and responsibilities

### Assignment and Time Allocation

An analyst is assigned to the project based on their availability, interest, experience, and/or best fit. Assignments are typically planned in monthly increments, with regular reviews of progress and needs. Dedicated time is frequently extended (2+ months) depending on funding and project complexity. Funding may come from the LMP department or from PI-supported grants as a percent effort.

### Communication and Milestones

We maintain regular communication through meetings, email, and shared documentation. Analysts provide updates on progress, request clarification when needed, and document all methods and code. Deliverables are shared in stages, with an emphasis on clarity, reproducibility, and feedback. 



## How we're funded

We are employees of MSI and our effort is supported by the Department of Laboratory Medicine and Fairview. If you need support, we can set up a meeting to discuss your specific project, experimental design, sequencing plans, etc. for free. Email the manager: Todd Knutson <knut0297@umn.edu> to get started. Depending on the project, our work is funded in three main ways: 

- PIs can request a _Letter of Support_ from MSI (Research Computing) for their grant applications.
    - This letter describes the compute resources available at MSI, and how bioinformatics analysts can support the specific project.
    - The letter ends by listing the percent effort of a bioinformatics analyst's time is needed for the project, per year (e.g. 25% of an analysts effort per year).
    - After the grant is funded, we will support the project as requested (with flexible scheduling over the grant period).
- PIs can provide a UMN chart string account number and schedule specific support time.
- Request free support from the LMP department (typically one month). [Details are described here](https://med.umn.edu/pathology/research/research-support) (expand the second section: _Research Bioinformatics Support_).




## Our Values

- **Clarity:** Code, reports (emails, etc.), and decisions should be understandable now and in the future (especially by our future selves).
- **Collaboration:** We work _with_ teams, not _for_ them. We want to be a close partner in your research and understand your issues at deep level. This approach allows us to find best-fit solutions for your project, versus just being assigned tasks. 
- **Integrity:** We admit mistakes quickly and operate within our areas of expertise.
- **Trust:** We maintain consistent, professional communication and follow through on commitments. We will voice any analysis concerns if they arise. 
- **Innovation:** We stay current with bioinformatics and wet lab methods.
- **Respect:** Everyone brings expertise—scientific, clinical, or technical, regardless of their role or status and will listen consider multiple perspectives.
- **Creativity and Autonomy:** Analysts have room to explore better approaches and suggest new ideas.
- **Feedback:** We encourage feedback from our collaborators and coworkers, and are empowered to share feedback with them.

## Conclusion

This document sets a foundation for collaboration and helps clarify how the LMP bioinformatics team contributes to research success. By aligning our goals with shared expectations and values, we hope to deliver rigorous, timely, and impactful work across all our projects.
