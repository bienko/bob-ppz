**GETTING STARTED**
# **BUSINESS PARTNERS | REGISTRATION AND SETUP**

---

## **i. Before you begin**

<!-- VIDEO EMBED (add once recorded):
![type:video](./_videos/Registration and Setup [Bob PPZ L3].mp4)
!!! note ""
    Christopher Bienko *(AI Enablement GTM Product Manager)* provides an overview of the *Registration and Setup* module for the hands-on enablement. **<a href="SEISMIC-LINK" target="_blank">[n min]</a>**
-->

!!! warning ""
    These instructions apply to **IBM Business Partners**. IBM regular employees have their own instructions available via **[IBMers | Registration and setup](setup-ibmers.md){:target="_blank"}**, which routes the Premium Package request through the w3 add-ons portal.

Before diving into the hands-on modules, complete the following registration and setup steps to prepare your machine with an authenticated **IBM Bob** account entitled to the **IBM Bob Premium Package for Z** (PPZ), along with a local copy of the *CBSA* sample banking application that the first two hands-on modules build upon. The work proceeds in six stages:

- Request the **Premium Package for Z** entitlement through **IBM Technology Zone**, which provisions both the IBM Bob service and the package against your IBMid
- Install and authenticate the Bob IDE on your local machine, then bind it to the entitlement
- Install the **IBM Bob Premium Package for Z** extension and its companions from the Extensions view, plus the **Draw.io Integration** extension used for diagramming
- Create a fresh project workspace
- Retrieve the **CBSA** application source files (COBOL programs, copybooks and BMS screen maps) with Bob in Agent mode
- Establish the workspace **rules** that govern where Bob files its documents, tools and diagrams throughout the lab

---

## **ii. Prerequisites**

Ensure that you have each of the following in hand before starting; most setup stalls trace back to one of these.

!!! success "BEFORE YOU BEGIN"
    - Valid **IBMid** credentials (the same IBMid you use to sign in to IBM Technology Zone)
    - Administrative rights to install software on your local machine
    - Internet access to **github.com** — the lab files are retrieved from a public repository

    No Intranet or VPN connection is required.

!!! warning "THIS LAB REQUIRES THE PREMIUM PACKAGE FOR Z"
    Without the **IBM Bob Premium Package for Z** (PPZ) entitlement, IBM Bob can still open and read mainframe code, though the *Z Code* and *Z Architect* modes and the specifically-trained capabilities that the package provides will be missing. If neither mode appears in your Agentic Sidebar by the end of this chapter, the entitlement has **not** been linked to your Bob account.
    
!!! note "ALREADY HAVE IBM BOB?"
    An existing IBM Bob account (a Free Trial, for example) does not carry the Premium Package for Z. Complete the entitlement request in section *iii* regardless; if the Bob IDE is already installed on your machine, you can skip the download in section *iv* and go straight to signing in.

---

## **iii. Request the Premium Package for Z entitlement**

!!! tip ""
    **Business Partner** reservation requests for *IBM Bob Premium Packages* are made **separately** from the requests for a general-purpose IBM Bob account. In other words: requesting an IBM Bob account (such as you completed earlier) does not carry entitlements for any Premium Packages (such as PPZ). A separate reservation request must be filed for such entitlements, which the following steps will guide you through.

---

1. Requests for Premium Package for Z entitlements are made via **IBM Technology Zone**. Visit the following collection to begin the process:

    !!! warning ""
        **URL: <a href="https://techzone.ibm.com/collection/bob-business-partner-enablement/environments" target="_blank">https://techzone.ibm.com/collection/bob-business-partner-enablement/environments</a>**

    From the left-hand side of the page, click the **Environments** tab.

    ![](_attachments/partners-IBMi-1.png){ width="600" }

---

2. Four options will be available:

    - Request entitlement for IBM Bob Enterprise
    - Request entitlement for IBM Bob Premium Package for i
    - *Request entitlement for IBM Bob Premium Package for Z*
    - Request entitlement for IBM Bob Premium Package for Java

    Click the **Reserve it** button below the *Request entitlement for IBM Bob Premium Package for Z* tile.

    ![](_attachments/partners-IBMi-2.png){ width="600" }

---

3. *Step 1: General* of the configuration process will ask you to specify a **Name** and **Description** for your reservation. When ready, click **Next** in the bottom-right corner to continue.

    ![](_attachments/partners-IBMi-3.png){ width="600" }

---

4. *Step 2: Business purpose* must be set to **Test** in order to bypass the need for an opportunity number. If you mistakenly click the wrong option, or if the reservation system does not allow you to continue without an opportunity number, exit out from this page and try again (making sure to only click *Test*). When ready, click **Next** to continue.

    ![](_attachments/partners-IBMi-4.png){ width="600" }

---

5. *Step 3: Deployment* will ask you to specify the **Geography** for your deployment. Select the data center location that is closest to you. When ready, click **Next** to continue.

    ![](_attachments/partners-IBMi-5.png){ width="600" }

---

6. *Step 4: Scheduling* will ask you to specify the go-live and termination dates for your entitlement. Choose a window that comfortably covers the time you expect to spend on this lab. If the entitlement lapses before you finish, you can submit a new request using these same instructions. When ready, click **Next** to continue.

    ![](_attachments/partners-IBMi-6.png){ width="600" }

---

7. *Step 5: Configure* can be left **blank** (default state of *"There is nothing to configure here."*) When ready, click **Next** to continue.

    ![](_attachments/partners-IBMi-7.png){ width="600" }

---

8. *Step 6: Review and submit* will ask you to review your configuration settings before submitting the request. Scroll down through your reservation details and, if you approve, check the **I agree to IBM Technology Zone's terms & conditions and user security policies.** box at the bottom of the page. When ready, click **Submit** to initiate the reservation request.

    ![](_attachments/partners-IBMi-8.png){ width="600" }

---

9. The web browser will redirect automatically to IBM Technology Zone's *My requests* dashboard. From this page, you can monitor and track the progression of your reservation request as it moves from `Scheduled` to `Provisioning` to `Ready`.

    !!! warning ""
        Average deployment times are roughly `5 minutes` or less.

    **Wait** until the request is marked as `Ready` before advancing.

    ![](_attachments/partners-IBMz-9a.png){ width="600" }

    ![](_attachments/partners-IBMz-9b.png){ width="600" }

    ![](_attachments/partners-IBMz-9c.png){ width="600" }

---

10. When the reservation is `Ready`, you will receive an email to your inbox providing you with a link to the environment **and** the same details will also be accessible via the *My requests* dashboard (where you were tracking the reservation request).

    Click either the **View your request** link in the email body *OR* click the arrow to the left of your reservation name on the *My requests* dashboard to expand details about the request.

    ![](_attachments/partners-IBMz-10.png){ width="600" }

    ![](_attachments/partners-IBMz-11.png){ width="600" }

---

11. Both links will direct to the IBM Bob dashboard:

    !!! warning ""
        **URL:** **<a href="https://bob.ibm.com/admin" target="_blank">https://bob.ibm.com/admin</a>**

    Authenticate and log in using your **IBMid** — the same one you used to sign in to IBM Technology Zone. The entitlement you just requested is associated with it.

---

12. The web browser will redirect to a welcome splash screen reading *"Welcome [your username]!"* where you are prompted to **Choose workspace**.

    If you previously registered for IBM Bob by another route (such as a *Free Trial*), the default option below this may display text such as `Free Trial` or something else entirely.

    - Click the box below **Choose workspace** to open a drop-down menu
    - Your request via IBM Technology Zone will have added a new option to this list, similar to `TECHZONE-BobathonV2 (us-east)`: this is your newly-provisioned Premium Package for Z entitlement
    - Select the `TECHZONE-...` option as your workspace and then continue with the login

    !!! warning "EXACT WORDING VARIES BY REGION"
        The label of the workspace depends on the geography you selected in *Step 5* and may not read exactly as it does in the screen capture. Look for the option prefixed with `TECHZONE`.

    ![](_attachments/partners-IBMz-12.png){ width="600" }

---

13. The web browser will automatically load into the IBM Bob dashboard.

    - Verify in the top-left corner that the `TECHZONE-...` workspace is selected for **Organization**
    - Click the **Subscription** tab to view your plan type and seat count, as well as your Bobcoin balance
    - Towards the bottom of the panel, under the **Premium packages** section, an *IBM Z* tile marked as `Active` confirms that your IBM Bob account is now linked to (and entitled for use with) the Premium Package for Z license

    ![](_attachments/partners-IBMi-9.png){ width="600" }

---

## **iv. Install and authenticate the Bob IDE**

With the entitlement provisioned, install the Bob IDE (if you have not already done so) and sign in with the same IBMid.

---

1. If the Bob IDE is not yet installed on your machine, **<a href="https://bob.ibm.com/download" target="_blank">download and install</a>** it now. Select the version that matches your operating system.

    ![](_attachments/setup-v2-1.png){ width="600" }

---

2. Open the Bob IDE and press **Log in to Bob**.

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/823f4c70-03dd-4452-b24b-50480c73112c/File_880f1ea2136e4d1b96c1f5c9f3f9b39d_text_export.jpeg" alt="" width="600" />
    </p>

---

3. Press **Allow** on the pop-up window, followed by **Open** on the subsequent pop-up window.

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/3d0178cf-b6e7-430d-83b0-c743985dac0e/File_6ed4e34559254ec1ba55dbbde5ff524b_text_export.jpeg" alt="" width="600" />
    </p>

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/84967b1a-441e-4566-a534-259aadd68ed3/File_a13363f84f5f4e62bc077b0703d5227e_text_export.jpeg" alt="" width="600" />
    </p>

---

4. On the IBM Verify sign-in page, expand the *"Choose an option"* drop-down and press **IBMid.** Sign in with the same IBMid that you used on IBM Technology Zone.

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/78b54a7a-6edf-417f-b14a-e4f7407858aa/File_8ba4dc1789ee451f867f3ec45530e014_text_export.jpeg" alt="" width="600" />
    </p>

---

5. You should be redirected to an **"Authentication Successful!"** screen within the Bob IDE.

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/568d1073-3c7e-422a-92f8-1a0a015e3d3a/File_15d119df77ee4384a003ea73832c2588_text_export.jpeg" alt="" width="600" />
    </p>

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/08b3f0b4-6d25-4191-b130-7b16f68b5857/File_eb57339049244ac58cf539fcd8ec5b7e_text_export.jpeg" alt="" width="600" />
    </p>

    <p align="left">
    <img src="https://colony-recorder.s3.amazonaws.com/files/2026-04-27/bed46d69-8811-430c-88ee-4f4582357f13/File_d1a0c6a0088b4f448fbeb1f3cfd4c67e_text_export.jpeg" alt="" width="600" />
    </p>

---

## **v. Install the Premium Package for Z extension**

With the entitlement in place, the next stage installs the extension that delivers it inside the Bob IDE. The Premium Package arrives through the Bob IDE's own **Extensions** view and brings three companion extensions with it.

---

1. Click the **Extensions** icon in the left Activity Bar (the square icon), or press ++ctrl+shift+x++. This opens the Extensions Marketplace panel where you can search for and install the extensions required for this lab.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/55f055ef-fbe5-4b5f-bb9a-f0b5c2b345c1/user_cropped_screenshot_84362d0a9b66411dbf2a1e27b20c26da_text_export.jpeg" alt="" width="600" />
    </p>

---

2. The Extensions panel opens in the left sidebar, with the *Search Extensions in Marketplace* search bar at the top.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/e36ce451-6f48-45f6-9d74-e5e7739e38ae/user_cropped_screenshot_835f89cab2b34ccdaec5ddff9f96cbef_text_export.jpeg" alt="" width="600" />
    </p>

---

3. In the search bar, filter on the following text:

    ```
    Premium Package For Z
    ```

    The top result should be **IBM Bob Premium Package for Z** with *IBM* marked as the publisher. Several similar-named extensions appear below it — make sure you select the correct one.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/cd90274f-696b-424f-bce0-981b368cc681/user_cropped_screenshot_35080c5212914f7cac155095b90527db_text_export.jpeg" alt="" width="600" />
    </p>

---

4. Click the **IBM Bob Premium Package for Z** result to open its detail page. Verify that the publisher is **IBM** and that the version is **3.0.0 or higher**, which this lab requires. The detail page confirms this is the correct extension before you commit to installing it.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/4e84043b-3277-455b-9256-678c89f56c9b/user_cropped_screenshot_46819e920bc24703b7973999c138d371_text_export.jpeg" alt="" width="600" />
    </p>

---

5. Click the **Install** button on the IBM Bob Premium Package for Z detail page.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/f3fc1ac2-fed3-4cca-9f44-81638336861c/user_cropped_screenshot_380c708b51134a21ae59bcaac6b3e00a_text_export.jpeg" alt="" width="600" />
    </p>

---

6. Click the **Clear Extensions Search Results** icon (next to the search box). Clearing the search filter resets the Extensions view so you can see your installed extensions and verify that the package components were properly added.

    !!! warning ""
        You may receive a pop-up window prompting you to restart after downloading the extension. If so, click the restart button to allow Bob to refresh.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/bb3429e1-cb69-42c9-a4ca-c8e6b921a7ad/user_cropped_screenshot_1ecdd6e96b2c4851a59e41f5ba70eaaa_text_export.jpeg" alt="" width="600" />
    </p>

---

7. Under the **INSTALLED** section of the Extensions sidebar, verify that four extensions have been installed as part of the package:

    | EXTENSION | PUBLISHER | PURPOSE |
    | --------- | --------- | ------- |
    | **IBM Bob Premium Package for Z** | IBM | Mainframe-specific AI agents, modes and workflows |
    | **IBM Z Open Editor** | IBM | Language support and syntax highlighting for COBOL, PL/I, HLASM, REXX and JCL |
    | **Mermaid** | MermaidChart | Renders architecture and flow diagrams directly within the editor |
    | **Zowe Explorer** | Zowe | Interaction with z/OS datasets, Unix System Services (USS) files and jobs |

    These companion extensions work together to provide complete mainframe development and diagramming capabilities within IBM Bob.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/bf6705ae-42cc-43da-94e9-62ad5aa0b469/user_cropped_screenshot_3994041f26dc4deaa14b9f0bf943b4f1_text_export.jpeg" alt="" width="600" />
    </p>

---

8. Upon completing the installation, multiple welcome tabs open — for example, **Welcome to IBM Bob Premium Package for Z** in the main editor area. This welcome page outlines getting-started steps, key commands such as creating an `AGENTS.md` file using `/init`, and the available skills and workflows. Close all of these welcome tabs.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-10-08/d983deeb-dccf-4d1b-a4d3-59f9390ba3c8/user_cropped_screenshot_25b278d6eeb54d5a841d7225c3a1acb8_text_export.jpeg" alt="" width="600" />
    </p>

---

## **vi. Bind the IDE to your entitlement**

The extension is installed, but the Bob IDE still needs to be pointed at the TechZone workspace that carries your entitlement. Two settings complete the connection.

---

1. Look towards the bottom-right corner of the Bob IDE interface. Along the bottom edge of the interface there will be an interactable button labelled **Bob Settings** — click this button to open the *Settings* panel.

    ![](_attachments/partners-IBMz-16.png){ width="600" }

---

2. From the *Settings* panel, make sure the **General** tab (left side) is the one being displayed.

    - Locate the **Team** setting, which by default at this stage might be set to `Trial` or some other variation
    - Click the name of your **Team** to pull open a drop-down menu
    - Select the `TECHZONE-...` option to connect the IDE to your Premium Package for Z entitlement

    ![](_attachments/partners-IBMz-17.png){ width="600" }

    ![](_attachments/partners-IBMz-18.png){ width="600" }

---

3. Further down the panel, adjacent to the **Add ons** setting, you should now see `IBM Bob Premium Package for Z` displayed.

    - Look further to the *right* of this setting to locate the **Install** button
    - Click **Install** to initiate an *Install addon* operation. This might seem redundant, but it is a required activation within Settings to fully connect the Premium Package
    - Wait a moment for a pop-up notification to appear in the bottom-right corner of the Bob IDE interface
    - Bob IDE might request an application restart to implement the changes; if this is the case, **accept** and restart the IDE

    ![](_attachments/partners-IBMi-10.png){ width="600" }

    ![](_attachments/partners-IBMi-11.png){ width="600" }

---

4. Open the **Mode selector** drop-down in the bottom panel of the Agentic Sidebar (the mode pill next to the prompt area). A Bob Mode is a named persona with a specific role, tool access and behavioral constraints. Alongside the default *Agent*, *Plan* and *Ask* modes, two new specialized mainframe modes now appear:

    - **Z Code**: designed for implementing, refactoring and explaining mainframe code (such as COBOL, PL/I and JCL)
    - **Z Architect**: tailored for high-level application analysis, architecture mapping and program relationship discovery across mainframe assets

    The remainder of the lab depends on these two modes. If the entitlement was granted and the extension installed, they populate automatically.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/c1755caf-233f-4f41-a713-2b7cf2dd3515/user_cropped_screenshot_ac5f2a72fbe14d898d022481cea9328f_text_export.jpeg" alt="" width="600" />
    </p>

    !!! warning "TROUBLESHOOTING: THE Z MODES ARE MISSING"
        If the extension is installed but these modes do not appear, the IDE is not yet bound to the entitlement. Re-check that the **Team** setting shows the `TECHZONE-...` workspace and that the *Install addon* operation completed, then restart the IDE once more.

---

## **vii. Install the Draw.io Integration extension**

One additional diagramming extension is required for the lab.

---

1. Click the **Extensions** icon on the left Activity Bar to return to the marketplace. The Extensions panel re-opens with the search input ready at the top.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/f8ce8491-207d-4307-8f28-cabc83bd13eb/user_cropped_screenshot_c0e8aaa6e1b34e4699fedbd931a2ab4f_text_export.jpeg" alt="" width="600" />
    </p>

---

2. In the search box, filter on the following text:

    ```
    Draw.io Integration
    ```

    From the search results list, locate **Draw.io Integration** with `hediet` marked as the publisher. Make sure to identify the correct extension among similar entries before installing it.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/b4a58ee5-0226-4d86-b32d-771a0d52b1ea/user_cropped_screenshot_997384f2ee5d4bc282bf6aeda55173c2_text_export.jpeg" alt="" width="600" />
    </p>

---

3. Click the **Draw.io Integration** entry in the list to open its details tab and verify that it is the correct extension.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/06c324ba-865e-45b9-baf2-e690ffd1c5c1/user_cropped_screenshot_e604dd8dd67246e195c41da7b4406468_text_export.jpeg" alt="" width="600" />
    </p>

---

4. Click the blue **Install** button on the Draw.io Integration details page (or in the search results list). This starts the extension installation into your Bob IDE environment.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/7a8b6e3c-03cb-402f-ab0b-a8434f5d01f0/user_cropped_screenshot_0f8bf7a487104ec6a1ebe6e71f842302_text_export.jpeg" alt="" width="600" />
    </p>

---

5. A confirmation dialog titled *"Do you trust the publisher 'hediet'?"* appears. Click **Trust Publisher & Install** to authorize the installation of the third-party extension into IBM Bob.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/d779d898-a726-4668-8145-01def9dc897f/user_cropped_screenshot_338fe00c5e504fcba0854dd7239fe0e9_text_export.jpeg" alt="" width="600" />
    </p>

---

6. Click **Clear Extensions Search Results** (the ++x++ icon in the Extensions search bar) to dismiss the search and return to the full Extensions list view.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/83353ab5-7474-40e3-88e4-f4be306eaa9d/user_cropped_screenshot_d8d330a14734421590c2dce219770c4b_text_export.jpeg" alt="" width="600" />
    </p>

---

7. The Extensions panel now shows **Draw.io Integration** (by hediet) in the **INSTALLED** list alongside the other extensions you added earlier:

    !!! warning ""
        - IBM Bob Premium Package for Z
        - IBM Z Open Editor
        - Mermaid
        - Zowe Explorer
        
    This confirms that all required extensions are in place.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/d88a4642-d91d-4c0e-a177-da56565f0a00/user_cropped_screenshot_5a4bfe9d9f5345eab85db392cdf74740_text_export.jpeg" alt="" width="600" />
    </p>

---

## **viii. Create the project workspace**

Bob and the other extensions need a workspace folder to operate in. You will create a dedicated, empty folder for the lab and open it as the root of your project.

---

1. Click the **Explorer** icon (the page icon at the top of the Activity Bar on the far left) to switch from the Extensions view to the File Explorer view.

    - The panel shows **NO FOLDER OPENED**, since the Bob IDE does not yet have a workspace folder set.
    - Click the **Open Folder** button to open a system file-picker dialog.
    - The Agentic Sidebar on the right is visible and already active, confirming Bob is ready as soon as a folder is loaded.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/fd0da714-e73c-463f-bfaa-f55316248923/user_cropped_screenshot_51ac0528c5554586bbd6eb36c9509992_text_export.jpeg" alt="" width="600" />
    </p>

---

2. The file-picker dialog opens. Create a dedicated folder for your lab work by clicking the **New folder** button.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/0ebdedc1-c9c2-4efc-a88b-c8816765dd9a/user_cropped_screenshot_3dcde559bdcb4fbbb759ecec53e400a9_text_export.jpeg" alt="" width="600" />
    </p>

---

3. A new folder appears in the file-picker with its name field open for editing. Type a memorable name for your lab workspace — the example shown uses `Bob PPZ L3` — and press ++return++ to confirm the name.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/70e5add0-6430-4920-ba62-26a7ea3820cc/user_cropped_screenshot_09875b4e48cd4b638b491d5f1e76c530_text_export.jpeg" alt="" width="600" />
    </p>

---

4. With the `Bob PPZ L3` folder created and selected in the file-picker, click **Select Folder** to open it as your workspace. This tells the Bob IDE to treat this folder as the root of your project for the rest of the lab.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/3051fe7f-5c55-4b53-b0da-d7a757ebb5bb/user_cropped_screenshot_96a12c5bcdae482aaf4e83e2e3687c2d_text_export.jpeg" alt="" width="600" />
    </p>

---

5. The Bob IDE opens the `Bob PPZ L3` workspace and the installed extensions automatically display their welcome tabs again: **Welcome to IBM Z Open Editor in IBM Bob** and **Welcome to IBM Bob Premium Package for Z**. Close both welcome tabs by clicking the ++x++ button on each tab.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/b5e16da0-f45b-47bf-a42b-48570464323f/user_cropped_screenshot_ca89966f5c174601be1e8e5be60d661c_text_export.jpeg" alt="" width="600" />
    </p>

    ??? warning "RESTRICTED MODE"
        When opening a new directory, the Bob IDE may automatically enable **Restricted Mode**, which locks out extensions and executables until such restrictions are lifted. If a blue **Restricted Mode** shield icon is showing in the bottom-left corner of the IDE:

        - Click the **Restricted Mode** button to pull open the configuration screen
        - Examine the two options under the *You are in Restricted Mode* panel: `In a Trusted Folder` and `In Restricted Mode`
        - Click the **Trust** button under the `In a Trusted Folder` option to disable restrictions
        - Click the ++x++ icon in the top-right corner of the panel to return to the main Bob IDE dashboard

---

## **ix. Retrieve the CBSA lab files**

The first two modules of this courseware work against the same application: **CBSA**, the CICS Banking Sample Application. Its COBOL programs, copybooks and BMS screen maps live in a public GitHub repository. You will have Bob retrieve the one sub-directory the lab needs, which spares you from cloning the repository by hand.

---

1. Click the mode selector to open the **Modes** picker and select **Agent** mode. In Agent mode Bob can read, write and execute actions autonomously within your workspace — the right choice for pulling down the lab files in the next step.

    Notice again that **Z Code** and **Z Architect** appear in the list. These are the two custom modes added by the IBM Bob Premium Package for Z extension; the lab depends on them from the first module onward.

    !!! warning "TROUBLESHOOTING: THE Z MODES ARE MISSING"
        If the extension is installed but these two modes do not appear in the list, there is an issue with your entitlement. Return to section *vi* and confirm the entitlement before continuing; IBM regular employees can also request support in the **#bob-and-friends** Slack channel.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/3db820bc-9b31-4f7b-977c-e68ec6bcb86b/user_cropped_screenshot_884665213c9f47a5a1f97205f3b6a9c6_text_export.jpeg" alt="" width="600" />
    </p>

---

2. With Bob in **Agent** mode, paste the following prompt into the Agentic Sidebar and press ++return++ (or click the send button) to submit it:

    ```text
    Retrieve the sub-directory named "src/base" in the CBSA directory from the GitHub repository https://github.com/ovallod/Bob4z-a-thon.git and place it in the current workspace folder. Then remove any temporary working directory you would have created.
    ```

    This instruction tells Bob to clone only the `src/base` subdirectory from the CBSA repository (`https://github.com/ovallod/Bob4z-a-thon.git`) into your workspace folder, then clean up any temporary working directory it created. Bob issues the git commands on your behalf, so you do not need to work with Git yourself.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/7a014797-6ab7-42b6-a717-5376f3fa8b27/user_cropped_screenshot_ca34767d8d7646d7a8675f71c117d3bc_text_export.jpeg" alt="" width="600" />
    </p>

---

3. Bob plans its approach and pauses for your approval before running any shell commands. The *Tools awaiting approval* section shows that Bob intends to execute a `git clone --depth 1 --filter=blob:none --sparse` command: a lightweight sparse clone that fetches the required subdirectory instead of the entire repository.

    Click **Approve for task** to authorize Bob to run this and all subsequent allowed commands for this task. This approval step is a built-in safety control: Bob executes terminal commands only after you consent.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/5284bad8-cf98-4133-8908-f04f446957a0/user_cropped_screenshot_13a591b2a0b540e7b624abf28382ea1e_text_export.jpeg" alt="" width="600" />
    </p>

---

4. Bob is now executing the task. The Agentic Sidebar shows the sequence of tool calls it is making: it ran the sparse `git clone` command, then listed the files inside the `_temp_repo` temporary directory it created to verify the clone succeeded.

    You can see `_temp_repo` has appeared in the Explorer panel on the left. The status at the bottom of the panel reads *Working on it...* — Bob is still in progress and will continue without further input.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_6e7093923d7d4b1abdd3557a4ef0d78b_c275ab3542244720907c8c08184d2a4c_78075dbdb1cc472dbb7905e951704dec_text_export.jpeg" alt="" width="600" />
    </p>

---

5. Bob continues working autonomously. It has now drilled further into the cloned repository: the tool log shows it listing files in `_temp_repo` and then in `_temp_repo\CBSA`, navigating the directory tree to locate the `src/base` subdirectory. No action is required from you at this point; wait while Bob completes its work.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_9294a5ca1e5441d4a5bcb9454c3ae138_49d0d90b280141c3954e744a3b48cacd_cb312382805d4ee09bab699588a2a246_text_export.jpeg" alt="" width="600" />
    </p>

---

6. Bob has located the target files. The tool-call log shows it navigated step by step through `_temp_repo` → `CBSA` → `src` → `base`, confirming the full path `_temp_repo\CBSA\src\base`. The status bar now reads *Processing...* as Bob copies the files from the temporary clone into your workspace. No action is needed; continue waiting.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_b9e42c9b2c3a444c8c6f9426c98d84b5_49c1e7f6b6d64d93ad8a2a3d983308ec_c20f2e1af27a413cb53345fed280db2d_text_export.jpeg" alt="" width="600" />
    </p>

---

7. Bob pauses for a second approval. Having confirmed the file location, it now wants to run an `xcopy` command to copy the contents of `_temp_repo\CBSA\src\base` into a `src\base` folder in your workspace, then delete the temporary directory.

    Click **Approve for task** to authorize this final step. This copy-and-cleanup sequence is the behaviour you asked for in the original prompt.

    !!! note ""
        The documented run is on Windows operating systems.
        
        On **macOS** or **Linux**, Bob proposes the equivalent `cp` command instead. Approve it in the same way.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/72cfc789-9e1c-47ec-88e4-a9eef66dd6c3/user_cropped_screenshot_e0d6fb3ffe124e9bbb2102249e841899_text_export.jpeg" alt="" width="600" />
    </p>

---

8. Bob has completed the task. The Explorer panel now shows a `src` folder in the workspace, and the temporary `_temp_repo` directory has been removed as requested. Bob's completion summary in the panel confirms the **Retrieved Structure**: `src/base/bms_src/` (9 BMS map definition files), `src/base/cobol_copy/` (34 COBOL copybooks), `src/base/cobol_src/` (32 COBOL source files) and `src/base/README.md`. All the CBSA application source files needed for the lab are now in place.

    !!! note "TWO VALID FOLDER LAYOUTS"
        Depending on how Bob copies the files, you may find the folder structure is either `src/base/...` directly in your workspace, or `CBSA/src/base/...` with a `CBSA` parent folder. Both are correct, and the lab steps work the same way in either case. The screenshot here shows `src` directly at the workspace root with no `CBSA` parent.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_29b686e851e84cd4ae30204c5ea91cce_fa5df71bea0b4f4b9b0369b455dc8a74_a45e32a8257b4d5aa0e6b444c50ce18b_text_export.jpeg" alt="" width="600" />
    </p>

---

9. In the Explorer panel, **click** the `src` folder to expand it and verify the lab files are present.

    !!! warning ""
        If your structure has a `CBSA` parent folder:

        - Expand `CBSA` first
        - Then expand `src` inside it

    The Agentic Sidebar on the right confirms what you should find: `src/base/bms_src/`, `src/base/cobol_copy/`, `src/base/cobol_src/` and `src/base/README.md`.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/4d844697-3d78-46b9-a183-4c04ffa693bd/user_cropped_screenshot_300b7684939c416984de6f9d3be24572_text_export.jpeg" alt="" width="600" />
    </p>

---

10. **Expanding** `src\base` confirms the three core folders required for this lab are present:

    - `bms_src` — BMS map definitions, the screen layout files for the CBSA CICS application
    - `cobol_copy` — COBOL copybooks, the shared data structure definitions
    - `cobol_src` — the COBOL source programs

    You will also see `README.md`. These three folders contain all the mainframe application code you will work with throughout the lab.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/57104371-7fdf-409d-ad1d-52ab7e27e3a2/user_cropped_screenshot_dc19d44f17854491864462ef64277d69_text_export.jpeg" alt="" width="600" />
    </p>

---

11. **Expand** `bms_src` to confirm it contains the 9 BMS map definition files (for example, `BNK1ACC.bms` and `BNK1CAM.bms`).

    **Expand** `cobol_copy` and `cobol_src` as well to confirm those folders are also populated before proceeding.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/4dc82373-1c59-4540-806d-0fae197d5ed3/user_cropped_screenshot_8540e2b762d547d59181fb7591a76517_text_export.jpeg" alt="" width="600" />
    </p>

---

12. In the bottom-right corner of the Agentic Sidebar, click **New task**. This clears the current conversation and opens a fresh task context, ensuring Bob starts the next instruction without any carry-over from the file-retrieval task you have completed.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/8aa144ac-ef3a-46e8-996d-cda36b2fbcc9/user_cropped_screenshot_79f328860bac44a6bc410310516ed5c4_text_export.jpeg" alt="" width="600" />
    </p>

---

## **x. Create the workspace rules**

*Rules* are the always-on constraints you first met in **<a href="https://ibm.github.io/bob-l3/tailor/3-2/" target="_blank">Module 3 | Tailor</a>** of the *Climbing the AI Maturity Curve* courseware: short, persistent instructions that Bob reads at the start of every task. Here they tell Bob where its documents, tools and diagrams belong — and how to name them — for the rest of the lab.

---

1. Continue in **Agent** mode. Paste the following prompt into the Agentic Sidebar and hit ++return++ to execute:

    ```text
    Create the following Bob rules (file in .bob/rules): 
    - Documents must be stored in the docs/ directory. Documents specific to a program should be stored in a sub-directory of docs/ using the program name. For example, documents about BNKMENU should be stored in docs/BNKMENU/ directory.
    - Tools must be stored in the tools/ directory.
    - Schemas, drawings and graphs must be stored in graph/ directory.

    Document, schemas, drawings and graphs file names must follow these conventions:

    -- Prefix: program name (e.g., BNKMENU) if the document concerns a specific program, or CBSA for the application, or GLOBAL for cross-cutting documents

    -- Document type: analysis, archi, docu, inv, plan, spec

    -- Format: [PREFIX]-[TYPE]-[description].md
    ```

    !!! warning ""
        Because the prompt spans multiple lines, Bob displays it as a collapsed *pill* in the input area rather than showing it inline. Click the pill to expand and review the full prompt text before it is sent.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/6df00f4c-094b-42df-a398-642547d1da3c/user_cropped_screenshot_d6718ab9967047ca9feb6c54c9ae6814_text_export.jpeg" alt="" width="600" />
    </p>

---

2. The expanded prompt preview dialog (*Pasted text #1 - xx lines*) shows the full instructions you are giving Bob: create a rules file at `.bob/rules/` that defines the file-organisation conventions for this workspace.

    - Documents go in `docs/`, with per-program subdirectories
    - Tools go in `tools/`
    - Schemas, drawings and graphs go in `graph/`
    - All file names follow the `[PREFIX]-[TYPE]-[description].md` format

    Review the text to confirm it matches, then click **Save** to confirm the prompt and return it to the input field ready to send.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/3c2c4e99-9e0b-4263-9909-b64a91597de2/user_cropped_screenshot_0c375f96991c4fde98f7f8afeac00719_text_export.jpeg" alt="" width="600" />
    </p>

---

3. Click the **Send message** button in the bottom-right corner (or hit ++return++ for an equivalent keyboard shortcut) to submit the file-organisation rules prompt to Bob.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/26a96f0d-04d3-487d-8b73-2c28137a062e/user_cropped_screenshot_6fb538e92fda4c5ba0443089a61250d0_text_export.jpeg" alt="" width="600" />
    </p>

---

4. Bob begins executing the task immediately. It explores the workspace structure, then attempts to write `.bob/rules/file-organisation.md`. In the documented run the write failed, because the `.bob/rules/` directory did not yet exist; the error *Failed to write file .bob/rules/file-organisation.md* is visible in the panel. Bob detects this automatically and requests permission to create the missing directory in the next step.

    !!! warning ""
        Due to the non-deterministic nature of generative AI, you may not encounter the exact same issues. When issues are encountered, Bob often tries to debug them automatically.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_98292fa919f549919598f38e8417365d_2816ae5de01a4538a178aa63903af264_03c5f84d3abe48beb915a9a1d79a0b59_text_export.jpeg" alt="" width="600" />
    </p>

---

5. Bob has recognised that the write failed because `.bob/rules/` does not exist, and requests permission to run `mkdir .bob\rules` — a shell command that creates the missing directory.

    Click **Approve for task** to allow Bob to create the directory and resume writing the rules file. The approval is required because the `execute` tool group (which controls shell command access) needs explicit user consent before running commands on your machine.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/b662588e-b8ce-4d6d-8261-a5f3b40b775e/user_cropped_screenshot_afef832d913248feb50e978568091c81_text_export.jpeg" alt="" width="600" />
    </p>

---

6. After approving the `mkdir` command, a `rules` folder appears inside `.bob` in the Explorer panel. The Agentic Sidebar confirms the full recovery sequence: it detected the write failure, ran `mkdir .bob\rules` to create the directory, and is now actively writing the rules file. This `.bob/rules/` directory is where Bob stores workspace-scoped rules — persistent instructions that Bob reads at the start of every task to guide its behaviour in this project.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/org_c5a86d7505634b408ffed7c02e1a91dc/team_1e16acc894ad4e0eba6e176fd42bdcc1/document_51963d6ab2444e2b8e2d43fe28577fea/steps/step_62990ee9bd684f8aa1600a7f23d3a8d1_a7ff000575434c6fb9ffae9b977dccb4_96f53530017f431e822f052492b4718c_text_export.jpeg" alt="" width="600" />
    </p>

---

7. Bob has completed the task. In the Explorer panel, `.bob/rules/file-organisation.md` is now visible: a new rules file containing the file-organisation conventions you specified. The panel summarises what was written. Tools go in `tools/` and schemas, drawings and graphs in `graph/`. All files follow the `[PREFIX]-[TYPE]-[description].md` naming convention:

    - Prefix: `<PROGRAM>`, `CBSA` or `GLOBAL`
    - Type: `analysis` / `archi` / `docu` / `inv` / `plan` / `spec`

    Bob will now apply these conventions automatically whenever it creates or places files in this workspace.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/73edb5cb-fd58-4f9b-8f0d-8f05b0e5a797/user_cropped_screenshot_474ed44c78cc45ab89b66f79b632a6f1_text_export.jpeg" alt="" width="600" />
    </p>

---

8. With the file-organisation rules task complete and `file-organisation.md` confirmed in the Explorer, click **New task** in the lower-right corner of the Agentic Sidebar. This clears the current task context so that the next prompt starts fresh.

    <p align="left">
    <img src="https://colony-recorder.s3.us-west-1.amazonaws.com/files/2026-09-28/f9c0b235-8983-469b-ae4e-b870e79f1eb6/user_cropped_screenshot_b6e959ca955d4077b76e5d60d4141bc1_text_export.jpeg" alt="" width="600" />
    </p>

---

## **xi. Verify the environment**

Before any module work begins, confirm that every piece of the environment is in place.

!!! success "READINESS CHECK"

    Before proceeding, verify each of the following items:

    - **Bob Settings → General** shows the `TECHZONE-...` workspace as your **Team**, and the *Install addon* operation for the Premium Package for Z has completed
    - The Extensions view lists five installed extensions: the **IBM Bob Premium Package for Z** with its three companions (IBM Z Open Editor, Mermaid and Zowe Explorer) plus **Draw.io Integration**
    - The Agentic Sidebar's mode selector lists **Z Code** and **Z Architect** alongside Agent, Plan and Ask
    - The `Bob PPZ L3` workspace is open and trusted (no *Restricted Mode* shield in the bottom-left corner)
    - The workspace contains `src/base/` (or `CBSA/src/base/`) with `bms_src`, `cobol_copy`, `cobol_src` and `README.md`
    - The workspace contains `.bob/rules/file-organisation.md`

!!! warning "A WORD ON WORKING WITH GENERATIVE AI"

    IBM Bob is powered by generative AI and LLMs, and a defining trait of these systems is that they are *non-deterministic* — unlike the *deterministic* tools most developers are accustomed to. In practice, that means the same prompt can produce different code from one run to the next. This is both a strength and a quirk of the technology, and it is something to work *with* rather than against.

    **Precision is what tips the odds in your favor.** The more clearly you describe what you want, the more closely Bob's output will mirror your intent; conversely, the smallest change in wording can meaningfully change the generated code. Throughout this lab, your results may differ from the solutions shown — and that is expected, not a defect. Whenever an output diverges, you have three good options: refine the prompt and try again, edit the generated code by hand, or simply proceed if the variation still compiles and runs. Human review remains essential at every step, and never more so than while you are still learning the tool.

---

## **xii. Key takeaways**

---

- Business Partners obtain both IBM Bob and the **Premium Package for Z** through a single IBM Technology Zone request: *Business purpose* set to **Test** and the nearest geography, with a `TECHZONE-...` workspace appearing at `bob.ibm.com/admin` within minutes.
- The entitlement is bound to the Bob IDE in two places: **Bob Settings → General → Team** (select the `TECHZONE-...` workspace) and the **Add ons** setting's *Install addon* operation.
- The **IBM Bob Premium Package for Z** installs from the Bob IDE's Extensions view and brings three companions with it: *IBM Z Open Editor* (language support), *Mermaid* (diagrams in the editor) and *Zowe Explorer* (z/OS datasets, USS files and jobs). The third-party *Draw.io Integration* extension completes the diagramming toolkit.
- Two new modes — **Z Code** for implementing and explaining mainframe code and **Z Architect** for application analysis and architecture mapping — are the visible sign that the entitlement is live; if they are missing from the mode selector, the entitlement has not landed.
- Bob in **Agent mode** retrieves the lab's source files for you with a sparse `git clone`, pausing at each *Tools awaiting approval* checkpoint; **Approve for task** is the control that lets it run the rest of a task without interruption.
- The **CBSA** application arrives as `src/base/` with 9 BMS maps, 34 copybooks and 32 COBOL programs; a `CBSA/` parent folder is equally valid.
- Workspace **rules** in `.bob/rules/` govern where Bob files documents, tools and diagrams and how it names them. Bob reads them at the start of every task, which is why they are established before any module begins.
- **New task** between prompts clears the context window so that each instruction starts clean.

</br>

Registration and setup are complete. The first hands-on module, **[Module 1 | Understanding the CICS Banking Sample Application](analyze/1-1.md){:target="_blank"}**, begins from this workspace.

---
