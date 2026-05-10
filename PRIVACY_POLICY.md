# Clear — Privacy Policy

**Effective date:** 10 May 2026
**Version:** 1.1
**Publisher:** Less Bound Pte. Ltd., 68 Circular Road, #02-01, Singapore 049422
**Contact:** [contact@less-bound.com](mailto:contact@less-bound.com)

---

## 1. Who we are and what this policy covers

Less Bound Pte. Ltd. ("**Less Bound**", "**we**", "**us**", or "**our**") operates the Clear mobile application ("**Clear**" or "the **Service**"). This Privacy Policy explains what personal data we collect about you when you use Clear, why we collect it, how we use and share it, and the rights you have over it.

By creating an account or using Clear, you agree to the practices described in this Privacy Policy. If you do not agree, please do not use the Service.

This policy applies to Clear on all platforms (Android, and — in due course — iOS). It does not apply to third-party websites or services we link to.

---

## 2. What Clear is for

Clear is a faith-, ethics-, and preference-based ingredient-label scanner. Users photograph a product label; we send the image to an AI service for analysis; the AI returns a CLEAR or AVOID verdict against the user's selected dietary rules (Halal, Vegetarian, Vegan, Pescatarian, Beef-Free).

**Clear does not detect food allergens or medical-condition triggers.** It is not designed for, and must not be relied on by, users with peanut, tree-nut, shellfish, soy, egg, gluten, lactose, or any other allergy or medically-restricted dietary requirement. See Section 12 (Important health and allergen disclaimer).

---

## 3. Data we collect

### 3.1 Information you give us

When you create an account and use Clear, we collect:

| Category | Details |
|---|---|
| Email address | Used to create your Firebase Authentication account and to contact you about the Service. |
| Password | Stored only as a hashed value by Google's Firebase Authentication service; we never see your plaintext password. |
| Dietary restrictions | The faith / ethics / preference categories you select (e.g. "Halal", "Vegan") and any custom-text restrictions you add (paid tiers only). |
| Preferred response language | The language code (e.g. "en", "ar", "hi") you choose for scan summaries. |
| Beta access codes | If you redeem a tester access code, we record that redemption against your account. |

### 3.2 Information generated when you use Clear

| Category | Details |
|---|---|
| Scan results | For each scan: the verdict (CLEAR / AVOID / NO_LABEL_DETECTED), the list of any flagged ingredients, the detected label language, the AI-generated summary, and a timestamp. |
| Subscription tier | "Free", "Traveler", "Guardian", or "Tester", and (for tester accounts) the expiry date of your beta access. |
| Scan count and reset dates | The number of scans you have performed in the current period, and the date the period resets. |
| Onboarding completion | A flag indicating whether you have finished the in-app onboarding. |

### 3.3 Information we do NOT store

- **The photos you take.** When you scan a label, the image is uploaded to our microservice, sent to Google's Vertex AI service for analysis, and discarded. We do not store your scan photos in our database, on our servers, or anywhere else after the scan completes.
- **Your location.** Clear does not request or use device location.
- **Your contacts, calendar, browsing history, or other apps.**
- **Your device's unique advertising identifier** beyond what Google AdMob collects directly when ads are shown (see Section 5).

### 3.4 Information collected automatically

When the Clear app contacts our microservice, our server logs record:

- Your Firebase user ID (so we can apply your scan quota correctly).
- Your device's IP address (for security and abuse prevention).
- The timestamp, restrictions list, and language of each scan request.
- Standard HTTP request metadata (user-agent, response time, response status).

These logs are retained for 30 days and then automatically deleted, except where required for security investigations or legal compliance.

---

## 4. How we use your data

We use your data only for the following purposes:

1. **To provide the Service.** Authenticating you, enforcing your scan quota, persisting your dietary restrictions, returning scan results, and showing your scan history.
2. **To process your scans.** Sending the captured image and your selected restrictions to a third-party AI service for analysis, then storing the result against your account.
3. **To enforce subscription tiers and limits.** Counting scans, resetting counters, and verifying tester access codes.
4. **To prevent abuse.** Detecting unusual usage patterns, multiple-account abuse, or attacks on our infrastructure.
5. **To show advertising** (free, traveler, and tester tiers only). We use Google AdMob to display banner and interstitial ads. AdMob's data practices are described in their [Privacy & Terms](https://policies.google.com/privacy).
6. **To communicate with you about the Service.** Account-related notices, security alerts, material changes to this policy or to the Terms of Service. We do not send marketing emails.
7. **To comply with law.** Where required by Singapore law or by valid legal process from another jurisdiction.
8. **To produce aggregated, de-identified insights and reports.** We may combine data across many users to produce statistics, trend analyses, and market-research reports — for example, aggregate summaries of which ingredient categories are most commonly flagged in a country, or which product types Halal-selecting users most often scan. These insights:
    - Contain **no information identifying any individual user**: account-level identifiers (Firebase UID, email, IP) are removed before aggregation.
    - Are produced using a minimum-group-size rule so that no published statistic can be tied back to a small number of users; the current threshold is at least 50 distinct users contributing to any reported figure.
    - May be published publicly, shared with industry partners (such as food manufacturers, retailers, regulators, and research organisations), and offered as part of Less Bound's commercial operations.

   You can opt out of having your (de-identified) activity contribute to this aggregation — see Section 11.

We do **not** sell personal data that identifies you as an individual, and we do not share identifying personal data with third parties for their own marketing purposes. Aggregated, de-identified insights as described in item 8 are not personal data once aggregated.

---

## 5. Third-party services we use

Clear is built on third-party platforms whose privacy practices apply when your data passes through them. We describe these by **category of service** below; the specific providers in each category as of the effective date of this policy are listed in [Appendix A](#appendix-a--service-providers-as-of-this-policys-effective-date) at the end of this document.

| Category | Purpose | Data shared |
|---|---|---|
| **Authentication services** | User account creation, password storage, sign-in | Email, hashed password, account metadata. We never see plaintext passwords. |
| **Managed database services** | Storing user profiles and scan history | Profile data (email, dietary restrictions, tier, scan count) and scan results (verdict, flagged ingredients, label language, timestamps) |
| **Server-side computing** | Hosting our scan-analysis backend | Scan request payloads (transient — discarded after processing) |
| **AI services** | Analysing ingredient label images | The captured image (transient — not retained by the AI provider), your restrictions list, your language preference |
| **Google AdMob** | Displaying advertisements (free, traveler, and tester tiers only) | Standard ad-serving signals: device advertising ID, IP-based approximate location, ad-interaction data. Subject to [Google's privacy policy](https://policies.google.com/privacy). |
| **In-app purchase verification** | Verifying purchases and managing subscription state | Purchase tokens, anonymised user IDs |

We do **not** share personal data with any third party for that party's own marketing purposes. The categories above describe data flowing through these services purely to provide Clear to you.

If we add a new category of third-party service (for example, an analytics SDK we don't currently use), we will update this section and notify you in-app before that service begins receiving your data. If we change which specific provider fulfils an existing category — for example, swapping one cloud-infrastructure provider for another — we will reflect that in [Appendix A](#appendix-a--service-providers-as-of-this-policys-effective-date) without a separate notification.

---

## 6. Where your data is stored

Different services run in different regions of our cloud infrastructure provider:

- **User profiles and scan history** are stored in the `asia-southeast1` (Singapore) region.
- **Our scan-analysis backend** runs in the `us-central1` (United States) region.
- **AI processing of scan images** runs in the `us-central1` (United States) region.
- **Authentication** is a globally-distributed service.

This means that when you scan a label, the image is transmitted from your location to a US-region service for AI analysis, then the result is returned and stored in Singapore. By using Clear you consent to this cross-border transfer.

For users in the European Economic Area (EEA) or the United Kingdom, our infrastructure providers rely on Standard Contractual Clauses or other lawful transfer mechanisms to process data outside the EEA / UK. The specific providers are named in [Appendix A](#appendix-a--service-providers-as-of-this-policys-effective-date), each of which publishes its own cross-border-transfer documentation.

---

## 7. How long we keep your data

| Data | Retention period |
|---|---|
| User account profile (email, restrictions, tier, etc.) | Until you request deletion (see Section 8). |
| Scan history | Until you request deletion. You can also delete individual scans from the History screen at any time. |
| Server access logs | 30 days, then automatically deleted. |
| Records required by law (e.g. tax records of subscription payments) | As long as Singapore law requires, then deleted. |

When you request account deletion, we mark your account as deleted immediately (so you can no longer sign in) and **permanently delete the underlying data within 30 days**. The 30-day window allows for accidental-deletion recovery and compatibility with our standard backup cycle. After 30 days the data is unrecoverable.

---

## 8. Your rights

You have the following rights over your personal data. To exercise any of them, email [contact@less-bound.com](mailto:contact@less-bound.com) from the email address associated with your Clear account.

| Right | What it means | How to exercise |
|---|---|---|
| **Access** | Get a copy of the data we hold about you. | Email us. We will respond within 30 days. |
| **Correction** | Have inaccurate data corrected. | You can edit your restrictions and language preference in the app's Settings; for other corrections, email us. |
| **Deletion** | Have your account and personal data permanently deleted. | Email us with the subject line "Delete my account." We will confirm within 7 days and complete deletion within 30 days. |
| **Export** | Receive your data in a machine-readable format. | Email us. We will provide a JSON export within 30 days. |
| **Object / restrict** | Ask us to stop or limit specific processing. | Email us with details. |
| **Withdraw consent** | Withdraw any consent you have given. | Email us. Note: withdrawing consent for processing necessary to provide the Service is equivalent to deleting your account. |
| **Complain** | Lodge a complaint with the Personal Data Protection Commission of Singapore. | [pdpc.gov.sg](https://www.pdpc.gov.sg/) |

If you are in the EEA / UK, you may also have additional rights under the GDPR / UK GDPR. We honour those rights for EEA / UK users and you can contact us in the same way.

---

## 9. Children

Clear is not directed to children under the age of 13, and we do not knowingly collect personal data from children under 13. In the European Economic Area, the United Kingdom, and certain other jurisdictions, the equivalent age is 16.

If you are a parent or guardian and believe your child has created a Clear account, please contact us at [contact@less-bound.com](mailto:contact@less-bound.com). We will delete the account and any associated data promptly.

---

## 10. Security

We protect your data using industry-standard practices:

- All network communication is over HTTPS / TLS.
- Passwords are hashed by Firebase Authentication; we never see plaintext passwords.
- Access to our infrastructure is restricted to authorised Less Bound personnel using two-factor authentication.
- We do not store scan photos at any layer.
- Firestore security rules restrict each user's data so it can only be read or written by that user (and by our backend service account for administrative operations like scan-count resets).

No security measure is perfect. If we become aware of a breach affecting your personal data, we will notify you and the Personal Data Protection Commission of Singapore as required by Singapore law.

---

## 11. Your control over aggregate-research use

Even though aggregated insights cannot be tied back to you, we offer an in-app opt-out for users who would prefer their (de-identified) usage patterns not contribute to our research and report dataset.

**Settings → Privacy → "Exclude my activity from aggregate research"**

When this toggle is on, your scan history, restriction selections, and other usage data continue to flow normally for the personal use of the app, but our aggregation pipeline skips your account when computing the statistics that feed our reports. Opting out has no effect on your access to the Service, the speed or accuracy of scans, the ads shown to you, or any other feature of Clear.

The opt-out applies prospectively. Statistics already published in past reports cannot be recalled, but those statistics are by definition aggregated and contain no information identifying you.

---

## 12. Cookies and tracking

Clear is a mobile app and does not use cookies. We do not currently use any analytics or behavioural-tracking SDKs. The only third-party SDKs that collect any device-level data are:

- **Google AdMob** (for displaying ads — see Section 5).
- The authentication and database SDKs that power the core service (see Section 5 and Appendix A).

If we add analytics or tracking in the future, we will update this policy and notify users in-app before enabling them.

---

## 13. Important health and allergen disclaimer

**Clear is an informational tool for faith-based, ethical, and preference-based dietary guidance only. It is not a medical device, not a clinical decision-making tool, and is not a substitute for medical labelling, certified-allergen-free product information, or professional medical advice.**

In particular:

- **Clear does not detect food allergens.** If you have a peanut allergy, tree-nut allergy, shellfish allergy, soy allergy, egg allergy, dairy/lactose allergy or intolerance, gluten/coeliac sensitivity, or any other allergy or medically-restricted dietary requirement, do **not** rely on Clear's verdicts.
- **Use certified-allergen-free product labelling and consult a licensed healthcare professional or registered dietitian** for any decision involving allergies, intolerances, or medical conditions.
- **Always verify ingredients directly on the product packaging.** AI-generated results may contain errors or omissions.

We disclaim, to the maximum extent permitted by Singapore law, any liability for harm arising from reliance on the Service for medical, allergy, or health-related decisions. See the Terms of Service for the full limitation of liability.

---

## 14. Changes to this policy

We may update this Privacy Policy from time to time — for example, when we add new features, integrate new third-party services, or to comply with new legal requirements.

When we make material changes, we will:

- Update the **Effective date** at the top of this document.
- Notify you in-app via a banner, and by email if the change materially expands how we collect or share your data.
- Where the change requires it under applicable law, ask you to renew your consent.

The current version of this policy is always available at [https://less-bound.com/clear/privacy](https://less-bound.com/clear/privacy) and from the in-app **Settings → Legal → Privacy Policy** link.

---

## 15. Contact us

For any privacy-related question, request, or complaint:

**Less Bound Pte. Ltd.**
68 Circular Road, #02-01
Singapore 049422
[contact@less-bound.com](mailto:contact@less-bound.com)

We aim to respond within 7 days for routine queries and within 30 days for formal data-rights requests.

---

## Appendix A — Service providers (as of this policy's effective date)

For transparency, the third-party platforms that fulfil the service categories in Section 5 as of **10 May 2026** are:

- **Google Cloud** — provides authentication, managed database, server-side computing, and AI processing services. Subject to [Google's Privacy Policy](https://policies.google.com/privacy) and Google Cloud's data-processing terms.
- **Google AdMob** — serves advertisements on free, traveler, and tester tiers. Subject to [Google's Privacy Policy](https://policies.google.com/privacy).
- **RevenueCat** — verifies in-app purchases and manages subscription state, when integrated. Subject to RevenueCat's [Privacy Policy](https://www.revenuecat.com/privacy).
- **Google Play (and, in due course, Apple App Store)** — distributes the app and processes payments for paid tiers. Subject to the relevant store's privacy policy.

We may change which provider fulfils a given category from time to time. Material changes — those that introduce a new category of data sharing, a new geographic region of processing, or a fundamentally different privacy posture — will trigger an update to the body of this policy and an in-app notification under Section 14. Routine same-category provider swaps will be reflected here in this appendix without a separate notification.

This appendix's "as of" date is updated whenever the provider list above changes.
