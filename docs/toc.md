<!-- toc-page -->
<style>
  /* Hide the ToC on its own standalone site page (screen), but keep it
     visible inside the combined print page (#print-site-page) so it can
     render into the PDF. Never touches .md-main__inner or the site chrome. */
  @media screen {
    .toc-page { display: none; }
    #print-site-page .toc-page { display: block; }
  }
  /* Keep the ToC's own group headers flowing on one page in print,
     without re-paginating h2 headings anywhere else in the document. */
  @media print {
    .toc-page h2 { page-break-before: auto !important; }
  }
</style>

<div class="toc-page" markdown>

# **Table of Contents**

## [Introduction](index.md#introduction)

- [1. Modernization is indispensable to the enterprise IT agenda](index.md#i-modernization-is-indispensable-to-the-enterprise-it-agenda)
- [2. What is IBM Bob?](index.md#ii-what-is-ibm-bob)
- [3. What the Premium Package for Z adds](index.md#iii-what-the-premium-package-for-z-adds)
- [4. How a prompt becomes a governed workflow](index.md#iv-how-a-prompt-becomes-a-governed-workflow)
- [5. The environment: two CICS applications](index.md#v-the-environment-two-cics-applications)
- [6. Lab objectives](index.md#vi-lab-objectives)
- [7. Lab prerequisites](index.md#vii-lab-prerequisites)
- [8. Next steps](index.md#viii-next-steps)

## [IBMers | Registration and Setup](setup-ibmers.md#ibmers-registration-and-setup)

- [1. Before you begin](setup-ibmers.md#i-before-you-begin)
- [2. Prerequisites](setup-ibmers.md#ii-prerequisites)
- [3. Internal registration](setup-ibmers.md#iii-internal-registration)
- [4. Request the Premium Package for Z entitlement](setup-ibmers.md#iv-request-the-premium-package-for-z-entitlement)
- [5. Install the Premium Package for Z extension](setup-ibmers.md#v-install-the-premium-package-for-z-extension)
- [6. Install the Draw.io Integration extension](setup-ibmers.md#vi-install-the-drawio-integration-extension)
- [7. Create the project workspace](setup-ibmers.md#vii-create-the-project-workspace)
- [8. Retrieve the CBSA lab files](setup-ibmers.md#viii-retrieve-the-cbsa-lab-files)
- [9. Create the workspace rules](setup-ibmers.md#ix-create-the-workspace-rules)
- [10. Verify the environment](setup-ibmers.md#x-verify-the-environment)
- [11. Key takeaways](setup-ibmers.md#xi-key-takeaways)

## [Business Partners | Registration and Setup](setup-partners.md#business-partners-registration-and-setup)

- [1. Before you begin](setup-partners.md#i-before-you-begin)
- [2. Prerequisites](setup-partners.md#ii-prerequisites)
- [3. Request the Premium Package for Z entitlement](setup-partners.md#iii-request-the-premium-package-for-z-entitlement)
- [4. Install and authenticate the Bob IDE](setup-partners.md#iv-install-and-authenticate-the-bob-ide)
- [5. Install the Premium Package for Z extension](setup-partners.md#v-install-the-premium-package-for-z-extension)
- [6. Bind the IDE to your entitlement](setup-partners.md#vi-bind-the-ide-to-your-entitlement)
- [7. Install the Draw.io Integration extension](setup-partners.md#vii-install-the-drawio-integration-extension)
- [8. Create the project workspace](setup-partners.md#viii-create-the-project-workspace)
- [9. Retrieve the CBSA lab files](setup-partners.md#ix-retrieve-the-cbsa-lab-files)
- [10. Create the workspace rules](setup-partners.md#x-create-the-workspace-rules)
- [11. Verify the environment](setup-partners.md#xi-verify-the-environment)
- [12. Key takeaways](setup-partners.md#xii-key-takeaways)

## [Understanding the CICS Banking Sample Application](analyze/1-1.md#understanding-the-cics-banking-sample-application)

- [1. Understanding the codebase](analyze/1-1.md#i-understanding-the-codebase)
- [2. Why this matters](analyze/1-1.md#ii-why-this-matters)
- [3. Explaining a program with Bob Workflows](analyze/1-1.md#iii-explaining-a-program-with-bob-workflows)
- [4. Documenting the CBSA architecture with Z Architect mode](analyze/1-1.md#iv-documenting-the-cbsa-architecture-with-z-architect-mode)
- [5. Analyzing the impact of a field change](analyze/1-1.md#v-analyzing-the-impact-of-a-field-change)
- [6. Key takeaways](analyze/1-1.md#vi-key-takeaways)

## [Implementing a New Feature in COBOL](build/2-1.md#implementing-a-new-feature-in-cobol)

- [1. From understanding to building](build/2-1.md#i-from-understanding-to-building)
- [2. Why this matters](build/2-1.md#ii-why-this-matters)
- [3. Planning the change with Z Code mode](build/2-1.md#iii-planning-the-change-with-z-code-mode)
- [4. Implementing the plan](build/2-1.md#iv-implementing-the-plan)
- [5. Verifying the generated code](build/2-1.md#v-verifying-the-generated-code)
- [6. Key takeaways](build/2-1.md#vi-key-takeaways)

## [Monolithic COBOL Refactoring and Service Integration](refactor/3-1.md#monolithic-cobol-refactoring-and-service-integration)

- [1. From duplication to a shared service](refactor/3-1.md#i-from-duplication-to-a-shared-service)
- [2. Why this matters](refactor/3-1.md#ii-why-this-matters)
- [3. Retrieve the GenApp lab files](refactor/3-1.md#iii-retrieve-the-genapp-lab-files)
- [4. Identifying the business rules](refactor/3-1.md#iv-identifying-the-business-rules)
- [5. Checking the dependencies](refactor/3-1.md#v-checking-the-dependencies)
- [6. Creating the validation service](refactor/3-1.md#vi-creating-the-validation-service)
- [7. Adding the link code to the main programs](refactor/3-1.md#vii-adding-the-link-code-to-the-main-programs)
- [8. Key takeaways](refactor/3-1.md#viii-key-takeaways)
- [9. Earn accreditation](refactor/3-1.md#ix-earn-accreditation)

</div>