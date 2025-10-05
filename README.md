# Phishing Email Analysis Mini-Project

![Cybersecurity Banner](https://img.shields.io/badge/Category-Cybersecurity%20Threat%20Analysis-blue)
![Static Badge](https://img.shields.io/badge/Status-Completed-success)

A practical mini-project focused on deconstructing a sample phishing email to identify and document attacker tactics.

---

## 📋 Table of Contents

- [Project Goal](#-project-goal)
- [Tools Used](#-tools-used)
- [Methodology](#-methodology)
- [Analysis of a Sample Email](#-analysis-of-a-sample-email)
- [Foundational Concepts Q&A](#-foundational-concepts-qa)
- [Conclusion & Key Learnings](#-conclusion--key-learnings)

---

## 🎯 Project Goal

The goal of this project was to identify the characteristics of a phishing email by analyzing a suspicious sample. The outcome is a greater awareness of phishing tactics and improved skills in email threat analysis.

---

## 🛠️ Tools Used

* A saved email file (`.txt`) containing the phishing sample.
* A free online header analyzer to inspect the email's technical details.

---

## 🔬 Methodology

The project followed a systematic approach to deconstruct the sample email:

1.  **Obtain Sample**: First, a safe phishing email sample was obtained from an online source.
2.  **Surface Analysis**: The visible components of the email were examined, including:
    * The sender's email address for signs of spoofing.
    * The email body for urgent or threatening language.
    * The presence of spelling or grammar errors.
3.  **Technical Analysis**: The hidden components were then analyzed:
    * Links were inspected by hovering to check for mismatched URLs.
    * Email headers were examined for discrepancies using an online header analyzer.
4.  **Summarize Findings**: Finally, all the identified phishing traits were documented in a clear report.

---

## 📧 Analysis of a Sample Email

For this project, I analyzed a sample email impersonating the financial technology company **Airwallex**. The email attempts to panic the user by claiming their account has been disabled due to failed MFA attempts.

![Airwallex Phishing Sample](image_04714d.png)

### Phishing Indicators Found

The following table details the specific red flags identified in the email sample.

| Indicator Type       | Evidence from Sample                                           | Severity | Explanation                                                                                                                              |
| :------------------- | :------------------------------------------------------------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------------- |
| **Spoofed Sender** | `info[.]airwallex@securesupportcloud[.]com`                | **High** | The sender's domain is not the official `airwallex.com`. This is a clear attempt to impersonate the legitimate company.     |
| **Social Engineering** | "Please verify immediately," "your account has been disabled"    | **High** | The email uses urgent and threatening language to create fear and pressure the recipient into clicking the link without thinking.       |
| **Suspicious Link** | A masked "Click here" hyperlink                                       | **High** | Masked hyperlinks are often used to hide the true, malicious destination URL. A hover-check would likely reveal a non-Airwallex domain. |
| **Technical Forgery** | (Hypothetical) Failed SPF/DKIM checks in the email header      | **High** | A full header analysis would likely provide technical proof that the email was not sent from an authorized server.             |

---

## 🧠 Foundational Concepts Q&A

This section contains answers to key questions about phishing and email security, making the project a useful reference guide.

<details>
<summary><strong>1. What is phishing?</strong></summary>
<br>
Phishing is a type of cyber attack where attackers impersonate legitimate organizations or individuals via email, text message, or other electronic communication to trick victims into revealing sensitive information. This can include login credentials, credit card numbers, or other personal data.
</details>

<details>
<summary><strong>2. How to identify a phishing email?</strong></summary>
<br>
You can identify a phishing email by looking for several red flags, including a sender's email address that is misspelled or uses a suspicious domain, urgent or threatening language, poor spelling and grammar, links where the displayed text does not match the actual URL destination, and unexpected attachments or requests for sensitive information.
</details>

<details>
<summary><strong>3. What is email spoofing?</strong></summary>
<br>
Email spoofing is the act of forging a sender's address to make an email appear as if it came from a legitimate source. Attackers use this technique to gain the recipient's trust and increase the likelihood that they will open the email and click on a malicious link.
</details>

<details>
<summary><strong>4. Why are phishing emails dangerous?</strong></summary>
<br>
Phishing emails are dangerous because they are the primary method for initiating a wide range of cyber attacks. If a victim falls for a phishing attempt, it can lead to identity theft, financial loss, installation of malware (like ransomware), and the compromise of entire corporate networks.
</details>

<details>
<summary><strong>5. How can you verify the sender's authenticity?</strong></summary>
<br>
You can verify a sender's authenticity by carefully inspecting the sender's email address, checking the email headers for security protocols like SPF and DKIM, and, if in doubt, contacting the sender through a separate, known-good communication channel (like their official website) to confirm they sent the email.
</details>

<details>
<summary><strong>6. What tools can analyze email headers?</strong></summary>
<br>
Several free online tools can analyze email headers, such as Google's Messageheader analyzer, MXToolbox, and G Suite Toolbox. These tools parse the raw header text and present it in a readable format, highlighting important information and potential security issues.
</details>

<details>
<summary><strong>7. What actions should be taken on suspected phishing emails?</strong></summary>
<br>
On suspected phishing emails, you should not click any links, download any attachments, or reply to the email. The best course of action is to report the email as "Phishing" or "Junk" using your email client's built-in features and then delete it.
</details>

<details>
<summary><strong>8. How do attackers use social engineering in phishing?</strong></summary>
<br>
Attackers use social engineering to manipulate human psychology. In phishing, they exploit emotions like fear, curiosity, and urgency to bypass a user's rational thinking. Examples include creating a fake invoice to incite curiosity or a false account suspension notice to create panic.
</details>

---

## 🏁 Conclusion & Key Learnings

This mini-project was a valuable, hands-on exercise in threat analysis. The key outcome was a heightened awareness of common phishing tactics and the development of skills needed to analyze suspicious emails, from surface-level inconsistencies to technical indicators found in the headers.

### Skills Demonstrated:
* Threat Detection & Analysis
* Understanding of Social Engineering Tactics
* Email Header Analysis
* Technical Documentation
