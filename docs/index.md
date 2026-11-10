**IBM BOB PREMIUM PACKAGE FOR Z**
# **INTRODUCTION**

---

## **i. Modernization is indispensable to the enterprise IT agenda**

![type:video](./_videos/Introduction [Bob PPZ L3].mp4)
!!! note ""
    Christopher Bienko *(AI Enablement GTM Product Manager)* introduces the *IBM Bob Premium Package for Z* curriculum for hands-on enablement. **<a href="https://ibm.seismic.com/Link/Content/DCfj8Bq7m3RpfGQThPRHq2mgmW3G" target="_blank">[5 min]</a>**

!!! success "RECOMMENDED: *CLIMBING THE AI MATURITY CURVE* (LEVEL 3)"
    This course assumes you have completed the <a href="https://ibm.github.io/bob-l3/" target="_blank">**Climbing the AI Maturity Curve with IBM Bob**</a> Level 3 curriculum and that its concepts are familiar ground: the Agentic Sidebar and its modes, Bob Rules and custom configuration, and the context window and its economics. The discipline that carried through every stage of that course applies here as well — Bob does the building, while the developer stays in control. The material ahead builds directly upon those foundations and will reference them throughout.

IBM sellers and business partners know first-hand from client engagements that the most expensive mistakes in modernization planning are the ones that are never scoped or accounted for in the planning steps. Certain elements are easy to ignore, but carry great costs if overlooked:

- Hidden assumptions baked into the legacy code
- The need to run old and new systems side-by-side during transition
- The true shape of the dependency tree
- Data conversion and organizational readiness
- The external interfaces that must keep working throughout

A useful discipline for sizing this work considers six dimensions of AI-assisted modernization estimation:

1. **Structural scope** — what is physically in-scope?
2. **Semantic complexity** — what behavior has to survive the change?
3. **Knowledge transparency** — can the system explain itself? Searchable internal knowledge changes the economics of modernization, well beyond developer convenience.
4. **Integration and data surface** — which boundaries must keep working? Modernization often fails at the edges: REST APIs, SOAP services, message queues and the like.
5. **Feedback readiness** — how quickly do you learn that something has broken?
6. **Operational and governance constraints** — what rules shape the work before it even begins?

Taken together, these dimensions resolve to a readiness test worth carrying into any client conversation. A codebase is well suited to AI-assisted assessment when intent is visible and boundaries are documented, when feedback is fast, and when changes can be sliced safely enough to verify. A codebase is poorly suited when the opposite holds true:

- Internal frameworks lack documentation and real payloads have no examples
- Contract tests and test data are missing
- The local build is unreliable
- Shared libraries have no clear owner
- There is no safe slice to run

As you will see in **[Module 1 | Understanding the CICS Banking Sample Application](analyze/1-1.md){:target="_blank"}**, building a rigorous understanding of the legacy application is what moves an estate from ill-suited toward modernization-ready.

!!! note "COBOL IN THE PRESENT DAY"
    Many organizations today continue to rely on business-critical applications that were written decades ago. These systems power core business processes and have earned their longevity through decades of dependable service. One of the most common programming languages found within these environments is **COBOL** (Common Business-Oriented Language).

    First introduced in 1959, COBOL was purpose-built for business data processing, and it remains one of the most widely deployed enterprise programming languages in the world. For more than sixty years, organizations have used COBOL to build systems that process vast volumes of financial and transactional data with exceptional reliability. Today, a significant portion of the world's business transactions continue to pass through COBOL applications running on IBM mainframes. Typical COBOL workloads include:

    - Banking and payment processing
    - Insurance policy administration
    - Government records systems
    - Airline reservation systems
    - Payroll processing
    - Retail and inventory management
    - Financial accounting applications

Despite their reliability, many present-day COBOL applications now face mounting modernization pressures: aging codebases that have evolved over decades; limited (or altogether absent) documentation; a shrinking pool of COBOL expertise in the labor market; difficulty integrating with modern systems; and growing demand for cloud-native architectures and modern user experiences. As a result, organizations increasingly seek ways to transform these applications while preserving the business logic that has been trusted for years — and that is the challenge IBM Bob was designed to address.

Those pressures take a recognizable shape on IBM Z. Mainframe applications are complex and mission-critical, and they often involve millions of lines of code, which calls for platform awareness and a deep understanding of IBM Z technologies. Four challenges recur in client conversations:

| CHALLENGE | REAL WORLD EXAMPLE |
| --- | --- |
| **Costs and complexity** | Millions of lines of code across thousands of programs. The result is a set of deeply interconnected programs that are expensive to maintain and evolve |
| **Scalability and agility** | Lengthy release cycles, heavy governance and low developer productivity slow innovation and extend time to value |
| **Skills** | A reduced talent pool and a reliance on scarce domain experts leave teams without application understanding |
| **Risk and reliability** | Modernization carries high operational risk. An unintended change can affect mission-critical workloads, compliance and business continuity |

!!! note "THE MARKET IS ALREADY MOVING"
    Gartner expects 90% of enterprise software engineers to use AI code assistants by 2028, up from less than 14% in early 2024.<sup>1</sup> Kyndryl's 2025 survey of mainframe organizations found that 88% have implemented or plan to implement generative AI tools as part of their mainframe modernization efforts.<sup>2</sup> For most mainframe clients, the principal challenge is accelerating application modernization in support of broader business transformation.

    <sup>1</sup> <a href="https://www.gartner.com/en/newsroom/press-releases/2025-07-01-gartner-identifies-the-top-strategic-trends-in-software-engineering-for-2025-and-beyond" target="_blank">Gartner, *Top Strategic Trends in Software Engineering for 2025 and Beyond*, July 2025</a>
    <sup>2</sup> <a href="https://www.kyndryl.com/us/en/campaign/state-of-mainframe-modernization" target="_blank">Kyndryl, *2025 State of Mainframe Modernization Survey*, September 2025</a>

---

## **ii. What is IBM Bob?**

***IBM Bob* is an AI-powered modernization and software engineering partner that supports the entire software development lifecycle.** Where a traditional code-completion tool is anchored to the moment of writing code, Bob is designed to support the lifecycle around it. Bob plans, executes, validates and governs multi-step tasks on a developer's behalf, which lets teams:

- Understand existing applications and analyze their business logic
- Generate technical documentation and architectural artifacts
- Modernize legacy systems and build new features
- Create automated tests and accelerate development workflows in general

Enterprises are entering a phase of AI-driven development in which tools do more than suggest or autocomplete code: they operate and coordinate across systems. Four requirements follow from that shift and each is built into how clients work with IBM Bob:

!!! note ""
    - **Support across the SDLC**, from planning through development. The value appears when AI operates inside the existing delivery pipeline
    - **Understanding of entire applications.** Safe orchestration requires application-wide context, which file-level reasoning cannot provide
    - **Governance, security and human oversight by design**, so that policy and accountability are enforced as the work happens
    - **Execution of multi-step workflows.** Outcomes require orchestration, iteration and validation, and a single prompt rarely supplies all three

Bob operates directly within the development environment, allowing developers to work alongside AI while maintaining complete visibility into every stage of the process. Throughout this lab, Bob will help you understand, extend and refactor two CICS COBOL applications in place. You (the developer) remain in the decision seat for every consequential step along the way.

---

## **iii. What the Premium Package for Z adds**

![type:video](./_videos/Recording of Client Presentation - IBM Bob Premium Package for Z [Bob PPZ L2].mp4)
!!! note ""
    Christopher Bienko *(AI Enablement GTM Product Manager)* delivers a client-facing overview of *IBM Bob Premium Package for Z*. **<a href="https://ibm.seismic.com/Link/Content/DC39HX2DmbQG6GWDPCXc3gDgfBTB" target="_blank">[15 min]</a>**

***IBM Bob Premium Package for Z (`PPZ`)* adds deep mainframe expertise to Bob, so that large and complex IBM Z applications can be modernized accurately and efficiently.** It is an extension for the Bob IDE and Bob Shell that uses structured workflows, automation and AI-driven insights to examine, restructure and document legacy mainframe code. It supports COBOL, PL/I, JCL, REXX and HLASM, along with the CICS, IMS, MQ and Db2 middleware those programs depend on. In this lab you will work in COBOL and CICS throughout.

What sets *IBM Bob Premium Package for Z* apart from other coding assistants in the marketplace today are four key value pillars:

| PILLAR | VALUE |
| --- | --- |
| **Modernization accelerator** | Mainframe expertise and application metadata are embedded in the workflows themselves, which scales end-to-end modernization, accelerates onboarding and reduces reliance on scarce expertise. |
| **Streamlined experience** | Code analytics are unified with multi-model intelligence to enable *literate coding*: developers express intent directly in code and receive context-aware changes in place. |
| **Enterprise-wide awareness** | Centralized mainframe code metadata can be shared across the enterprise, so the model reasons beyond file-level scope and gains consistency and accuracy. |
| **Secure, governed AI** | IBM Z domain expertise embeds platform-aware security controls and governance-aligned guidance into the workflows, for compliant and context-aware outcomes at scale. |

---

Those pillars are delivered through a handful of concrete mechanisms (that this hands-on lab will also exercise):

| MECHANISM | WHAT IT DOES | LAB SECTION |
| --- | --- | --- |
| **Specialized modes** | Purpose-built AI personas for specific tasks. **Z Architect** plans and analyzes mainframe applications before any implementation; **Z Code** explains, generates, modifies and refactors mainframe code. Users can switch between modes without losing context. | Module 1 runs in Z Architect; Modules 2 and 3 run in Z Code. Their presence in the mode selector is the visible proof that your entitlement is live |
| **Workflows** | Guided multi-step analyses with built-in prompts. Examples include *Explain code*, *Generate data dictionary*, *Extract business rules* and *Generate refactored service program* | Module 1 opens with the *Explain code* workflow |
| **Skills** | Reusable instructions that make a task run the same way every time, such as *impact-analysis*, *data-dictionary-management* and COBOL code generation. | Module 1 (impact analysis), Module 2 (code generation) and Module 3 (the data-dictionary skill in Bob's to-do list) |
| **Tools** | The actions Bob can take: read and write files, run commands, scan the application into a metadata database (`scan_program`) and query it. | Module 3 scans GenApp before it analyzes a single program |
| **Rules and AGENTS.md** | Repo-level files that set standards and guardrails for AI behavior, so outcomes are governed by default and predictable across teams. | *Registration and setup* creates `.bob/rules/file-organisation.md` |
| **zContext** | Purpose-built IBM retrieval (RAG) that enriches the model with curated Z knowledge (languages, middleware, patterns and code samples) with no setup on your part | Module 3's to-do list includes the step *Assess Z Context needs and call z_context_tool* |

!!! info "WHY DO DATA DICTIONARIES MATTER?"
    Mainframe variable names are terse, and a model that infers meaning from an abbreviation alone will guess. An enterprise-specific data dictionary gives Bob authoritative business context instead. In one documented example, a program's `VO-FILE` was explained as a *voucher/order transaction file* without a dictionary; with one, Bob correctly described the program as a flight-management routine that reads flight records for pilot statistics. The same context improves documentation, rule extraction and explanations while reducing hallucinations. You will see the *data-dictionary-management* skill appear in Bob's plan during Module 3.

Beyond the scope of this lab, the package also exposes enterprise-scale application metadata for architecture-aware analysis across hundreds of programs, and runtime awareness that captures execution paths and frequency patterns for production-aligned impact analysis.

---

## **iv. How a prompt becomes a governed workflow**

Any time that a user sends a prompt to Bob— such as *"Create a new COBOL program that does X using my coding standards"* —the *Premium Package for Z* works through four stages before it answers:

1. **Intent analysis and mode selection** — Bob interprets the request and confirms the mode best suited to it
2. **Governance** — Bob selects the applicable skills and the rules (or AGENTS.md) that constrain how the work is done
3. **Execution** — Bob selects its tools: scanning the application and querying the resulting metadata, retrieving variables, and reading and editing files
4. **Reason and response** — Bob synthesizes the results and reports back, with every file change presented as a diff for your approval

You will witness this deterministic workflow in action within the hands-on work ahead. In **Module 1**, Bob recognizes an impact-analysis request, loads the corresponding skill, and drafts a to-do list before reading the copybook. In **Module 3**, Bob's first to-do list runs according to the same pattern: it confirms the metadata database and scans the application; invokes the data-dictionary skill and assesses Z Context needs; and only then does Bob read the three programs it was asked about.

---

## **v. The environment: two CICS applications**

This lab works against two sample applications, each containing a small (but nevertheless realistic) CICS system of the kind found in banking and insurance estates.

**The CICS Banking Sample Application (CBSA)** is the subject of Modules 1 and 2. It is an enterprise-grade z/OS reference application that simulates core retail banking operations: customer onboarding and account management, together with deposits, withdrawals and fund transfers. It is built on IBM CICS Transaction Server for z/OS, Db2 for z/OS and VSAM, with a clear separation between its presentation, business service and data layers.

| ARTIFACT | ROLE IN THE APPLICATION |
| --- | --- |
| 29 COBOL programs under `cobol_src` | Presentation drivers, business logic services, an asynchronous credit bureau simulation and utilities |
| 9 BMS maps under `bms_src` | The 3270 screen layouts, including the main menu map `BNK1MAI` |
| Copybooks under `cobol_copy` | Shared record layouts and screen definitions, such as `BANKMAP.cpy` and `CUSTOMER.cpy` |
| `BNKMENU` | The entry point (transaction `OMEN`) that routes users to each screen driver |
| `BANKDATA` | The batch utility that generates the application's data |
| `INQCUST` | The customer inquiry service that five other programs call |
| `CUSTOMER` (VSAM KSDS) and `ACCOUNT`, `PROCTRAN`, `CONTROL` (Db2) | The persistence layer |

**GenApp**, the CICS general insurance sample application published by the CICS development team, is the subject of **Module 3**. Its policy programs (`LGAPDB01`, `LGUPDB01` and `LGDPDB01`) sit in the middle of a three-tier `LINK` chain that runs from the 3270 screen programs, through a business-logic tier, down to Db2 and VSAM. They share the `LGCMAREA` copybook as their `COMMAREA` contract and the `LGPOLICY` copybook for policy-specific definitions. Each of them validates requests in its own code, which is the duplication that **Module 3** consolidates into a single service.

!!! info "WHAT IS `CICS`?"
    **CICS** (Customer Information Control System) is IBM's transaction processing middleware on z/OS. A *transaction* starts a program; programs hand work to one another with `EXEC CICS LINK` and exchange data through a **COMMAREA** (communication area), a shared record whose layout lives in a copybook. Screens are defined as **BMS** (Basic Mapping Support) maps, which exist in two forms that must stay in sync: a physical map that CICS renders and a symbolic map that programs reference through a copybook. Data lives in **VSAM** files (a **KSDS** is a key-sequenced data set) and in **Db2** tables, and a program abends with a four-character code such as `ASRA` when it fails. Every one of these terms appears in the modules ahead.

Both applications are intentionally small. They nonetheless contain many of the same programming concepts found within the real-world COBOL systems of banks, insurers, governments and financial institutions. Working against a believable codebase from start to finish, rather than a series of disconnected snippets, lets you watch Bob operate the way it would inside a client's modernization initiative.

---

## **vi. Lab objectives**

!!! note "TO EFFECTIVELY MODERNIZE, YOU MUST FIRST UNDERSTAND A CLIENT'S ESTATE"

    Modernization projects frequently involve millions of lines of legacy code and decades of accumulated business logic. Rewriting that code is seldom the hardest part of the initiative. The far greater difficulty lies in understanding four things: what the application does, why it behaves that way, which business rules must be preserved, and how changes can be introduced safely. In the era of AI-generated code this understanding gains even greater significance. The developer's day shifts away from authorship and toward steering, constraining, verifying, and cleaning up what an agent produces. Judgment, in other words, becomes the scarce resource.

    Enterprise mainframe environments add a difficulty of their own. They are vast and highly interconnected, with tens of thousands of tightly coupled artifacts and poorly defined boundaries, which makes the impact of any change hard to assess. Establishing clear application and solution boundaries is the first step toward scoping and modernizing these systems safely, and it is the reason this lab insists on understanding before change. Module 1 traces the potential impact from any changes to a single field before even touching a line of code. Module 3 documents the business rules and maps the dependencies across two full reports before any snippets of code are adjusted.

    IBM Bob helps accelerate each of these activities, from application understanding and architecture discovery to code transformation, automated testing and documentation generation. All the while, the developer stays in control of the process.

This lab follows a realistic workflow for understanding and changing a mainframe application. You will use the Premium Package for Z to perform the same activities that teams undertake during modernization initiatives, organized across three modules that progress from analysis to change.

| CHAPTER | TOPIC | WHAT YOU'LL TAKE AWAY |
|---------|-------|------------------------|
| [**Setup for IBMers**](setup-ibmers.md){:target="_blank"} | **IBM REGULAR EMPLOYEES ONLY.** Register internally, request the Premium Package for Z entitlement through the w3 add-ons portal, install the extension and retrieve the CBSA source files with Bob | A Bob IDE with the Z Code and Z Architect modes live, a workspace holding CBSA and the workspace rules Bob will follow |
| [**Setup for Business Partners**](setup-partners.md){:target="_blank"} | **BUSINESS PARTNERS ONLY.** Request the entitlement through IBM Technology Zone, bind the IDE to it and complete the same workspace setup | The same validated environment, with no IBM intranet access required |
| [**1. Analyze**](analyze/1-1.md){:target="_blank"} | **ALL AUDIENCES.** Explain a program with the *Explain code* workflow, document the CBSA architecture in Z Architect mode and trace the full impact of shrinking one copybook field | Application understanding produced in minutes, with an impact report that separates true dependencies from look-alike fields |
| [**2. Build**](build/2-1.md){:target="_blank"} | **ALL AUDIENCES.** Ask Bob for a plan to add customer search by email, review it, have Bob implement the COBOL and verify its syntax | The plan-first habit, and a generated program that follows the conventions of the surrounding suite |
| [**3. Refactor**](refactor/3-1.md){:target="_blank"} | **ALL AUDIENCES.** Identify GenApp's duplicated validation rules, map their dependencies, extract them into a shared `LGPOLVAL` service and wire the callers to it | A monolith refactored in place, with every rule traced to its source and every change approved as a diff |

---

## **vii. Lab prerequisites**

The hands-on work ahead assumes you have completed the core curriculum of the *Climbing the AI Maturity Curve* L3 course, or that you hold equivalent familiarity with the Bob IDE and the Agentic Sidebar as well as Rules and AGENTS.md. Your environment begins as a fresh workspace: nothing from the *Galaxium Travels* project carries over, and Bob retrieves the mainframe source files for you with a sparse `git clone`, so you will not work with Git directly.

---

What you ***do*** need:

!!! success "REQUIREMENTS"
    - **IBM Bob** installed and authenticated: the *Registration and setup* chapter has two versions (for IBM regular employees and IBM business partners)
    - Your **IBMid** credentials are at hand (IBM regular employees sign in with their w3id)
    - **IBM regular employees:** access to the **<a href="https://w3.ibm.com/w3publisher/bob/addons" target="_blank">w3 add-ons portal</a>** to request the Premium Package for Z entitlement. Approval is manual and takes 24 to 48 hours, so request it before the day you plan to run the lab
    - **Business Partners:** access to **IBM Technology Zone** to request the Premium Package for Z entitlement
    - Internet access to **github.com**, where both sample applications are hosted
    - A local folder is available to serve as your Bob project workspace

    No additional downloads or staged files are required before you begin.

!!! warning "BUSINESS PARTNERS"
    **Business Partners** obtain their entitlement through IBM Technology Zone and follow their own Setup page, **[Business Partners | Registration and setup](setup-partners.md){:target="_blank"}**. That route is fully self-contained and requires neither the w3 add-ons portal nor an IBM intranet connection.

!!! info "A WORD ON TOKEN BUDGETS"
    Every module ends with a reminder to watch your Bob token budget. Mainframe applications involve large and interconnected codebases, so the prompts in this lab consume more than a comparable task on a small project. Finish each module's prompts before you experiment with the optional variations.

---

## **viii. Next steps**

In the chapter ahead, you will register for IBM Bob and obtain the Premium Package for Z entitlement, in accordance with your job role:

!!! quote ""
    - **<a href="https://bienko.github.io/bob-ppz/setup-ibmers/" target="_blank">IBM regular employees</a>** through the w3 add-ons portal
    - **<a href="https://bienko.github.io/bob-ppz/setup-partners/" target="_blank">Business Partners</a>** through IBM Technology Zone

All participants will afterwards install the PPZ extension and its companions, then have Bob retrieve the CBSA source files into a fresh workspace. The first module begins by analyzing CBSA: a business-level explanation of one program, an architecture document for the whole application and an impact analysis for a single field change. That understanding is the foundation for the feature you build in *Module 2* and the refactoring you carry out in *Module 3*.

---
