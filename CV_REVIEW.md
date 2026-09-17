# CV review and revision notes

Reviewed on 17 September 2026. Target: remote platform engineering, DevOps and SRE roles in Poland, with EU opportunities also in scope; mid-level and senior individual contributor positions.

This accompanies the revised `index.html`. It records the research, editorial decisions and proposed additions. Unconfirmed suggestions below are not part of the CV.

## Assessment

Your strongest positioning is an infrastructure engineer who can own a platform, improve how teams use it, and handle production operations. The combination of sole DevOps responsibility at Oper, observability across a large service estate at XTB, customer deployment automation and practical AI tooling gives you several concrete interview stories.

The existing CV already contains useful results. Its main weakness is uneven evidence: cost savings and installation speed are clear, while several senior-level capabilities appear only as responsibilities or skills. More precise ownership, adoption and operational outcomes would strengthen the senior case. A longer technology list would contribute less.

Mid-level applications are reasonable on the described experience. Senior applications are also worth pursuing where the role matches your ownership and technical depth. This is an assessment of the CV's evidence, not a claim that seniority is consistent between employers. Keep historical job titles accurate.

## Research and its practical implications

### 1. Write for a person assessing evidence

Harvard's career guidance favours specific, factual, active language and visible results. It also cautions that generative AI can produce generic application material. For this CV, use direct verbs such as built, operated, automated and migrated, followed by the actual system and the result. Avoid stock descriptions such as “results-driven professional” and “proven track record.” [Harvard resume guidance](https://careerservices.fas.harvard.edu/resources/create-a-strong-resume/)

The short first-person summary is a deliberate editorial choice to preserve your voice. Harvard's student-oriented template advice discourages pronouns; that is a style convention, not evidence of a universal screening rule. Experience bullets remain concise and omit pronouns.

### 2. Keep the application document easy to parse

Greenhouse documents parsing problems with image-based resumes, complex columns, tables, graphics, unclear sections, and contact details inside document headers, footers or text boxes. It also documents a 2.5 MB parsing limit. That supports a single content column, ordinary text, clear headings and visible contact information. It does not prove that every formatted CV fails or that a failed parse means automatic rejection. [Greenhouse parsing documentation](https://support.greenhouse.io/hc/en-us/articles/200989175-Unsuccessful-resume-parse)

Your revised HTML keeps the name and contacts in the main document flow. An HTML `<header>` element is not the repeated page-header area of a Word document. The print layout uses text rather than a screenshot. Actual extraction and application autofill still need review on the exported file; there is no universal “ATS score” to guarantee acceptance.

### 3. Aim for two readable pages

For six roles plus relevant technical breadth, my recommendation is a two-page application CV. Prospects recommends normally keeping a CV to two A4 pages, while allowing the content and experience to guide selection. This is useful guidance, not a Poland-specific rule or an ATS requirement. [Prospects CV guidance](https://www.prospects.ac.uk/careers-advice/cvs-and-cover-letters/how-to-write-a-cv/)

Keep all six roles in reverse chronological order. Give recent roles more detail and retain Wirtualna Polska as a short entry. Keep the two SentiOne periods separate so that the intervening Allegro role remains clear. Preserve a comprehensive master CV; tailor the emphasis for individual applications.

### 4. Platform engineering needs evidence of developer benefit

CNCF's platform maturity model covers adoption, interfaces, operations, investment and measurement. Self-service and feedback from internal users are central themes. Your alerting tools, QA deployments and routine-task pipelines are relevant platform work even without a developer portal. [CNCF platform engineering maturity model](https://tag-app-delivery.cncf.io/whitepapers/platform-eng-maturity-model/)

The next useful details are who used these tools, what manual dependency disappeared, how adoption happened and what improved. Do not add Backstage, golden paths, a platform roadmap or an entire internal developer platform unless those accurately describe work you did.

### 5. SRE needs reliability decisions and learning from failure

Google's SRE guidance treats SLOs and error budgets as inputs to decisions and prioritisation. A CV becomes more persuasive when it explains which service behaviour was measured and what changed as a result. [Google SRE: implementing SLOs](https://sre.google/workbook/implementing-slos/)

You already describe on-call, postmortems, recovery drills, instrumentation and SLOs. A confirmed example of a recurring failure eliminated, an alert made actionable, or a recovery demonstrated would make this work more tangible. A recovery target is different from an observed recovery time; neither implies continuous availability.

### 6. DevOps outcomes go beyond maintaining pipelines

DORA's current guidance uses five software delivery performance metrics and emphasises context at the application or service level. It warns against misleading comparisons across unlike systems. For your CV, delivery time, deployment frequency, failed-deployment recovery or reduced rework can be useful evidence if you actually measured them. Do not retrofit DORA terminology onto unrelated measurements. [DORA performance metrics](https://dora.dev/guides/dora-metrics/)

Your confirmed “days to minutes” installation result already tells a clear story. A useful next detail is whether it measures automated execution, engineer effort or the complete customer onboarding process.

### 7. Employer descriptions support three different emphases

I used these as illustrative requirements, not as a representative labour-market survey or a shortlist of verified available jobs:

- **Platform:** Moss's description combines Kubernetes/GCP, Terraform, deployment safety, observability, troubleshooting and engineering collaboration. Your cloud migration, JVM operations and observability are relevant evidence. Its advertised Berlin/hybrid arrangement does not match your remote preference; it is a role-content benchmark only. [Moss platform role](https://jobs.ashbyhq.com/moss/89470d75-c6e1-4056-8a18-f7878572350b/?trk=public_post-text)
- **DevOps:** OptiPlay's Poland/remote description stresses infrastructure ownership, modular Terraform, Kubernetes, CI/CD, GitOps and operational visibility. Your Oper role is the clearest match to that ownership pattern. The posting's part-time employment label also means it should not be treated as a generic full-time opportunity. [OptiPlay DevOps role](https://jobs.ashbyhq.com/optiplay/21eb5534-ee2e-4037-b241-5b19f6b4e610)
- **SRE:** TechInsights' remote-Poland description combines SLOs, incident response, recovery, developer enablement, automation and AI operations. It also requires specific tools and senior scope that should not be inferred from your adjacent experience. [TechInsights SRE role](https://techinsights.applytojob.com/apply/z58HhzvoCT/Senior-Site-Reliability-Engineer-Remote-Poland)

## Review of each role

### XTB

The scale is compelling: 800+ services and terabytes of daily telemetry. These describe the environment; they do not establish that you individually owned all those services. You clarified direct ownership of four pieces: a self-service alerting-as-code platform for roughly 60 or more developer teams, common alerts intended to cover all services, LLM-based incident detection from internal chat, and a RAG tool correlating incidents with previous incidents, runbooks and postmortems. You described the remaining work as collaborative.

The revised entry leads with those four contributions. It uses “approximately 60” to preserve your estimate and says the platform was built “for” those teams, without claiming a measured adoption rate. Common alerts are described by their coverage purpose, without claiming a verified 100% rollout. The RAG bullet describes faster investigation and recovery as its purpose; no measured MTTR reduction has been supplied or claimed.

The remaining bullets explicitly describe team contributions or shared operational work, including instrumentation, the log scanner and reporting. Keep the OpenTelemetry/JVM detail: it is more specific than a generic monitoring claim. Nine bullets preserve the full scope in this master CV; a targeted application can shorten the supporting team-work bullets. The next useful detail is the implementation of the alerting-as-code platform or an observed outcome from the incident tools, if available.

### Oper Credits

This is the clearest evidence of autonomy. Sole DevOps responsibility is now an explicit scope statement, followed by the cloud migration result. The savings are qualified using your confirmed quarter-over-quarter comparison after migration.

Keep repeated production restores, self-service QA deployments and the ISO 27001 infrastructure work. Before an interview, be ready to explain what was included in the cost comparison and your specific certification responsibilities. The CV does not claim zero downtime, equivalent workload volumes, a particular recovery time, or ownership of the entire certification programme.

### SentiOne — DevOps / AI Infrastructure Engineer

The strongest bullet is customer setup reduced from days to minutes. Keep the mix of cloud, on-premises and GPU infrastructure because it shows breadth beyond managed Kubernetes. Automated recovery provides another useful reliability story.

Potential improvement: clarify the installation boundary, number of deployments or customers, and a representative recurring failure. Those are proposed evidence additions, not established facts.

### Allegro Pay

Keep this short role. Both existing bullets describe delivered automation, and it establishes Azure and PowerShell experience. The draft retains August–November 2022 as the four full months you described. No reason for leaving or contract arrangement has been invented.

### SentiOne — Junior DevOps Engineer

The start date is corrected to July 2021. Bare-metal provisioning, Elasticsearch operations and on-call work explain your progression well. The wording now says you took part in 24/7 coverage, which avoids suggesting that you personally worked continuously.

### Wirtualna Polska

Keep one concise line. Data-center operations are relevant foundations for your later infrastructure work. Restoring an extensive list of early duties would reduce the space available for more recent evidence.

## Changes made in the draft

- Preserved all six roles, existing technical breadth, languages and the open-source contribution.
- Corrected the first SentiOne start to July 2021 and the second to December 2022, immediately after the four full months at Allegro Pay (August–November 2022).
- Added the approved measurement context to the approximately 40% cost reduction.
- Shortened the summary and brought the 800+ service context into the introduction.
- Reordered bullets to expose scope, self-service capabilities and results earlier.
- Incorporated your confirmed XTB contributions and approximate team scope; corrected the remaining XTB work to collaborative attribution. Historical job titles remain unchanged.
- Grouped skills by function; PowerShell is now also listed under programming because it already appears in the Allegro experience.
- Removed redundant calculated tenure labels, while preserving the month/year ranges.
- Simplified the design to one column, restrained colour, standard local fonts, text contact links and consistent headings.
- Added a print action and A4 print styles, with an intended page break between Oper and the second SentiOne stint.

The open-source contribution is independently supported by the linked merged PR, which describes the Forex calendar, tests and documentation. It is useful concrete evidence of code contribution and should remain. [Merged pandas_market_calendars PR #436](https://github.com/rsheftel/pandas_market_calendars/pull/436)

## Proposals requiring your confirmation

These are drafting patterns, not claims about your experience. None of the bracketed material has been added to the CV. A useful qualitative result is preferable to an invented number.

1. **Alerting implementation and adoption:** The ownership and approximate intended team scope are now confirmed. Further detail could identify the configuration workflow, validation, deployment and actual uptake. No particular stack, adoption percentage or reduction in support requests is assumed.
2. **Recovery evidence:** “Validated recovery of [scope] in [observed time] during [number] drills.” Confirm what recovered, what was measured and whether the figure is a target or a demonstrated result.
3. **Reliability improvement:** “Automated recovery from [failure mode], reducing [measured out-of-hours pages or recurring incidents] from [baseline] to [result] over [period].” If records are unavailable, describe the failure and automation without a percentage. Likewise, a quantified MTTR improvement from the RAG tool requires separate evidence.
4. **Senior contribution:** Replace a generic leadership skill with one example of mentoring, a design decision, standards adoption or coordinating a migration. Confirm the people or teams involved and your responsibility.
5. **Security contribution:** Specify the infrastructure controls or audit evidence you handled for ISO 27001. Do not add SOC 2, policy-as-code or security architecture ownership merely because employers request them.

The backup also mentions enterprise infrastructure consulting, documentation and knowledge sharing, a CODE:ME front-end course, personal trading systems, and additional languages/tools such as Go and C#. These have not been restored. Confirm their accuracy, dates and current relevance before considering them; the course's date range and stated duration in the backup are inconsistent.

The second SentiOne start is now December 2022, based on your clarification that it followed immediately after four full months at Allegro Pay (August–November 2022). This supersedes the conflicting dates in the previous CV and backup. The corrected first SentiOne date leaves July 2020–June 2021 outside the listed employment history. No explanation has been invented; add an activity only if it actually belongs in your history.

Location, remote availability, work authorisation, education and certifications should only be added using your own confirmed details. Targeting Poland/EU roles does not by itself establish residence or eligibility.

## Tailoring once you choose an offer

- **Platform application:** lead with self-service alerting, QA deployment workflows and customer installation automation. Use the offer's target title in the headline; keep actual employment titles intact.
- **DevOps application:** prioritise the Oper scope and migration, Kubernetes, Terraform/Ansible, GitOps and release automation. Preserve each role's chronology while reordering bullets within it.
- **SRE application:** prioritise observability, SLOs, incident response, automated recovery and disaster recovery. Keep AI tooling prominent when the role specifically values it.

For each application, match terminology where it is accurate, retain the strongest relevant skills, and move older or peripheral tools out of the application copy when space is needed. Avoid claims of equal depth in every cloud. Confirm exact CI/CD product names before replacing the current GitHub/GitLab wording with more specific names.

## Delivery and review status

The changes are local and have not been committed or published. Source and diff were reviewed; no tests were added or run, in accordance with your instructions. Computer-use permissions prevented a browser preview, so the rendered appearance, PDF page count and PDF text extraction are not yet verified.

The print stylesheet is designed for a two-page A4 CV; that remains a layout target until rendered. When exporting, select A4 and disable browser-generated headers and footers. Check that the phone number appears, links remain usable, all six roles are present and no text is clipped. Review extracted application fields before submitting. Use the file type requested by the employer; the website itself is not a substitute for an uploaded CV where one is required.
