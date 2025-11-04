
---

### TL;DR Summary

California’s Department of Health Care Services (DHCS) has implemented a process for PACE organizations to receive referral leads (prospective enrollees who chose PACE on state enrollment forms) via the Secure Data Exchange Services (SDES) platform. To get access, InnovAge must submit SDES New Account Request Forms for the appropriate staff – one form per user, signed by both the user and an authorized InnovAge representative. DHCS initially asked for these forms by Nov 25, 2022 (ahead of PACE being added to choice forms effective Jan 2023). Once DHCS (and their contractor, Maximus) processes the request, the designated users receive SDES accounts and can log in to download Weekly Plan Files (WPF) containing the new PACE enrollments/referrals. These files are tab-delimited text extracts of enrollment data posted to SDES each week. Due to internal delays, InnovAge did not complete this onboarding in 2022. In fact, DHCS indicates that two InnovAge employees – Stryder and Christena Duccini – already have SDES access and received the technical instructions back in late 2022. However, the process wasn’t operationalized, prompting renewed efforts now to finalize access and start capturing California PACE leads for our centers.

---

**Subject:** Request for SDES Access to Weekly PACE Lead Files

**To:** PACE@dhcs.ca.gov

Hi DHCS PACE Team,

We’re ready to begin receiving PACE referral leads for our California locations. Could you please confirm the current process for accessing these leads via SDES? Specifically:

- Can we receive the Weekly Plan Files (WPF) via API ?
- If not, we’re prepared to download the files manually from the SDES portal.
- Please advise on the required steps to activate or confirm our access, including any forms or technical setup needed.

We appreciate your support and look forward to getting started.

Best regards,  
Mark Cetola  
Revenue Operations Sales Enablement Analyst  
InnovAge

---


### ✅ DHCS Lead Access Setup – Action Checklist

- [ ] Contact Stryder and Christena Duccini to confirm their SDES access and retrieve any onboarding materials they received.
- [ ] Identify additional InnovAge users who need SDES access (e.g. sales ops, analytics).
- [ ] Complete a separate SDES New Account Request Form for each user, including:
    - [ ] User details and business name
    - [ ] Folder access: check “Weekly Plan Files (WPF)”
    - [ ] Access level: select “Read-only”
    - [ ] External IP address (from IT)
    - [ ] Signatures from user and authorized rep
- [ ] Email completed forms to PACE@dhcs.ca.gov with a request for account setup.
- [ ] Follow up with DHCS and/or Maximus Help Desk to confirm receipt and processing.
- [ ] Once accounts are created, distribute login credentials and test access to SDES portal.
- [ ] Navigate to “Weekly Plan Files” folder and download a recent file to validate access.
- [ ] Share sample file with analytics/CRM team to confirm format and plan for lead intake.
- [ ] Assign responsibility for weekly file retrieval and set calendar reminders.
- [ ] Enable email notifications for new file uploads (if available).
- [ ] Communicate progress to internal stakeholders and document the SOP for future use.
---

#### Key SDES Onboarding Details (California PACE Leads)

|**Step/Item**|**Details**|
|---|---|
|**Account Request Form**|“SDES New Account Request or Access Change Request” – one form per person needing access. Fill in all required fields (user info, business/org name, etc.) and specify “Weekly Plan Files (WPF)” as the folder to access. Indicate desired access level (typically Read-only to download files) and the outward-facing IP address/range from which that user will connect (obtain from IT). The form must be signed by the user and an authorized rep of InnovAge. Submit the completed form to DHCS via email (PACE@dhcs.ca.gov). DHCS’s initial instruction was to submit by Nov 25, 2022, but since that window has passed, we should send it ASAP to initiate access.|
|**SDES Platform & Access**|SDES is a secure file-transfer web portal (using MOVEit software) managed by Maximus on behalf of DHCS. After DHCS approves the account, the user will receive credentials to log in. Access can be via web browser (HTTPS) or SFTP; for SFTP, the user’s IP must match the one provided on the form. The site URL is http://healthcareoptions.maximus.com/sdes/. Users must accept a security notice and then log in with the provided username/password. (Passwords must be changed every 60 days.) DHCS retains sole authority to grant/revoke access. For any login issues or setup help, the Maximus HCO Help Desk can assist (916-364-2000, M–F 8am-5pm).|
|**Folder Structure**|Once logged in, the user’s home page will show a directory for "Weekly Plan Files." The user should click “Weekly Plan Files” then navigate to InnovAge’s folder (typically named for our PACE organization). Inside, DHCS will post our weekly referral files. Each week, new files will appear there for download. We might also receive access to other folders if applicable (e.g. “Provider Data” or MET files), but for PACE lead referrals, the WPF folder is primary. Ensure the user’s account has at least Read access to that folder so they can download files. Optionally, the form allows enabling email notifications to alert when new files are uploaded.|
|**File Format & Naming**|The Weekly Plan File (WPF) is delivered as a text file (ASCII encoding), with tab-delimited fields, and no header or trailer row. Each record represents an enrollment or disenrollment transaction for a beneficiary. DHCS generally provides two files each cycle: a transaction detail file (T_yymmdd.###) and a summary file (S_yymmdd.###), where ### is the 3-digit plan code. The layout of the detail file is defined in the attached DHCS specs – it includes fields such as Plan Code, Member Name, DOB, Medi-Cal ID, enrollment or disenrollment indicator, effective date, etc. Note: These files contain no PHI beyond contact and enrollment info, and are intended to inform us of new PACE selections; DHCS cautions they are for forecasting/outreach use, not as final eligibility confirmation.|
|**Retention Timeline**|Time-sensitive: Files on SDES are not stored indefinitely. The official retention is 90 days – any file older than 90 days is automatically purged from the system. However, DHCS has advised PACE plans to download each file within 30 days of it being posted. This means we should retrieve files promptly (ideally as soon as notification of availability is received). Failing to download in time could result in losing that lead data. We should set up an internal routine or automated job to pull these files weekly and back them up on our end.|
|**Internal Status**|InnovAge’s onboarding lagged after the initial 2022 rollout. Emails indicate that Roslyn Paulson and others tried to push this forward in 2024, as the lack of direct referrals was hurting CA centers. We learned that Stryder and Christena Duccini had been granted access and given these instructions – likely they attended a DHCS/Maximus walkthrough webinar in Nov 2022 and received login info and a PowerPoint guide. Despite that, the process wasn’t implemented (possibly due to unclear ownership or turnover). Now, with Revenue Operations involved, the plan is to finally complete the setup so that our CA PACE marketing and enrollment teams start receiving state leads. VP Anthony Horner explicitly flagged this (“please ask Stryder where he's at with them”) and believes our team can “unlock” these leads. There is high internal visibility and expectation to get this done quickly.|

---

### Next Steps – Enabling DHCS Leads for CA PACE

1. **Re-engage Existing Account Holders:** Coordinate immediately with Stryder and Christena Duccini, who according to DHCS already have SDES accounts and the onboarding materials. Confirm their credentials are still active and gather any documentation they received (e.g. the SDES portal URL, login instructions, or a copy of the “SDES Walkthrough for PACE Plans” PPT). If they can log in, have them verify whether InnovAge’s Weekly Plan Files folder is visible and if any files have been posted over the past year (there may be historical files since Jan 2023 if the system was active even while we weren’t pulling them).
2. **Identify Needed Users & Submit Forms:** Determine who at InnovAge needs ongoing access to these lead files. Besides the two existing users, consider adding someone from the data/analytics team or sales ops for redundancy. For each additional person, complete the SDES New Account Request Form. Fill out all required fields and check the “Weekly Plan Files (WPF)” access box (and any other relevant folders) with “Read-only” permission to start. Be sure to include the external IP address for each user’s connection (coordinate with IT – likely our corporate public IP). Have each user sign their form and get an authorized InnovAge manager to sign off. Email the forms to PACE@dhcs.ca.gov with a brief note requesting account setup. Even though the original deadline has passed, DHCS will still process new access requests; emphasize that we are a PACE organization now ready to onboard.
3. **Follow Up with DHCS/Maximus:** After sending the forms, proactively follow up with the DHCS PACE Program team to confirm receipt and ask for an estimated timeline for account setup. DHCS indicated that once forms are submitted, accounts will be established and further instructions sent to the technical contacts. If we don’t get a response within a few days, contact the Maximus HCO Help Desk (916-364-2000 or their email) to ensure they’re processing our access. We should also verify if Stryder and Christena Duccini’s existing accounts are still valid or if new forms are needed for them (if their access was never used, it should still be in place).
4. **Secure Credentials & Test Access:** Once DHCS/Maximus confirms account creation, ensure each user receives their SDES login credentials (username and temporary password). Log in to the SDES web portal to test access for each account. Upon first login, users might need to set a new password and possibly install the MOVEit upload/download wizard (if using the web interface) – follow any prompts. Navigate through the portal to confirm the “Weekly Plan Files > [InnovAge PACE]” directory is accessible and list the files. Attempt to download a recent file as a test. If any issues arise (e.g., login problems or folder access errors), involve the help desk immediately. Additionally, note if the system offers an SFTP connection method; if so, we may want IT to set up an automated SFTP pull (which would require whitelisting our IP – already part of the form – and using the given credentials in an SFTP client or script).
5. **Process the Retrieved Files:** Take one of the downloaded weekly plan files and parse it to ensure we understand the format. The file is tab-separated text with no header row; using the layout specification provided by DHCS, map the columns (e.g. Name, DOB, Contact info, etc.) and verify the data looks valid. It’s likely a list of individuals who chose InnovAge PACE during that week’s enrollment cycle, possibly including whether it’s a new enrollment or disenrollment. Share a sample with the analytics or CRM team to decide how to import or use this data. (For instance, we might create a process to upload these leads into CRM for outreach). If two files are provided (detail and summary), the summary just aggregates counts – the detail file is what we’ll use for individual follow-up.
6. **Establish Ongoing Retrieval & Notifications:** Going forward, assign responsibility for weekly lead retrieval. Ideally, one of the account holders (or an automated job) should download the new WPF every week as soon as it’s available. We should take advantage of the notification option – if not already set, ask DHCS/Maximus if an email alert can be sent when a new file is posted, either to the user or a group mailbox. In any case, set a recurring calendar reminder (e.g. every Monday if files post weekly on Fridays) to check SDES. Download files within 30 days of posting to avoid missing any leads (best practice is to download immediately upon notification). Store the files on a secure InnovAge drive for backup, and update whatever internal tracker or database will hold these leads.
7. **Communicate Internally & Close the Loop:** Update all stakeholders on our progress. Let Anthony Horner and Shadie Qaqish know once access is live and leads are flowing – this has been a long-standing issue, so positive news here is important. Also inform Roslyn Paulson and the California center managers that we have begun receiving state referrals directly. Ensure that our sales/marketing teams in California have a plan to promptly contact or mail these PACE leads once we receive them (to maximize enrollment conversion). Finally, document the process (perhaps a short SOP on how to log in and get the files) so that if personnel change or backup coverage is needed, we won’t let the process lapse again.