# MuseumLog Privacy Policy

**Effective date:** July 21, 2026
**Last updated:** July 25, 2026

This Privacy Policy explains how MuseumLog collects, uses, shares, and protects information when you use the MuseumLog mobile application (the "App").

**Data controller:** Alex Zhang, operator and data controller for MuseumLog, based in California, United States. Contact: museumlog.app@gmail.com.

**Where the App is offered:** the App's beta is offered in the **United States**, in the countries of the **European Union / European Economic Area**, in the **United Kingdom**, and in **Switzerland**. Section 9 describes your rights under the GDPR, the UK GDPR, and the Swiss Federal Act on Data Protection (FADP), and the legal bases we rely on.

If you do not agree with this policy, do not use the App.

---

## 1. Summary (plain language)

- We collect your **account information** (email, name, avatar, language preference) when you sign up.
- You can use core features **without creating a named account**; in that case we create an anonymous account identifier on your device.
- When you scan an artwork, **your photo is sent to third-party AI providers** (Anthropic, OpenAI, Google Cloud) to identify the artwork. This is the core function of the App.
- We use your **location** (only while you use the App, and only if you grant permission) to find museums near you.
- Photos you attach to your artwork log are stored on our servers. **Photo storage URLs are not currently access-restricted — treat logged photos as potentially accessible to anyone with the link.**
- We store the content you create: artwork logs, personal notes, collections, favorites, and learning progress.
- **Product analytics are opt-in.** If — and only if — you agree, we collect anonymous usage events (which screens and features you use) to improve the App. Declining changes nothing, and you can turn it off anytime in Profile → Privacy & Data.
- We do **not** sell your personal information.
- You can delete your account and data in the App (Profile → Settings → Account) or by contacting us (see Section 10).
- The beta is for **adults (18+)** only.

---

## 2. Information we collect

### 2.1 Information you provide

- **Account information.** When you sign up with email and password, we collect your email address, a display name you choose, and your password (stored by our authentication provider in hashed form — we never see or store your plaintext password). If you sign in with **Apple** or **Google**, we receive your name and email address from that provider, subject to the choices you make in their consent screens (Apple lets you hide your email).
- **Profile information.** An optional avatar photo, your display name, and your preferred language (one of: English, Spanish, French, German, Italian, Japanese, Portuguese, Chinese).
- **Artwork photos.** Photos you take with the camera or select from your photo library to identify and log artworks, including optional label/placard photos.
- **User content.** Artwork log entries (title, artist, year, medium, description, visit date), free-text personal notes, collections, and favorites.
- **Communications.** Anything you send us by email or support channels.
- **Feedback board posts.** The titles and descriptions you post to the in-app community feedback board.

### 2.2 Information collected automatically

- **Anonymous account identifier.** If you use scanning features before creating a full account, we create an anonymous authentication identifier for you. Content you create is tied to that identifier. If you later create a full account, that identity and its content persist under your account.
- **Location data (with your permission).** With your consent, we access your device's approximate location while the App is in use, to find museums and art venues near you. We do not track your location in the background.
- **Photo metadata (EXIF).** Photos you take or import may contain embedded metadata, including GPS coordinates and capture date. We read this metadata to infer where and when you saw an artwork, and we record the location associated with your artwork log along with how it was obtained (e.g., photo metadata, current device location, or your visit session).
- **Usage counters.** We keep daily counts of your AI-powered requests (scans, content generation) to enforce fair-use limits and control costs. These counters are tied to your account identifier.
- **Learning and interaction data.** Your progress in Learn features (lessons completed, review queue) and an append-only log of in-app interactions (e.g., which artworks you viewed) used to personalize recommendations.
- **Device and session data.** Authentication session tokens are stored securely on your device (see Section 7). Standard technical data (such as IP address) is processed transiently by our hosting and infrastructure providers as part of operating the service.

### 2.3 Product analytics (opt-in)

With your **opt-in consent** — asked once during onboarding and changeable anytime in Profile → Privacy & Data — we collect product-analytics events through **PostHog** to understand how the App is used and where it can improve. If you decline (or simply never agree), no analytics events are collected or transmitted, and the App works identically.

When you have opted in, analytics events include: which screens and features you use (for example, each onboarding step you reach), feature interactions (such as votes on the feedback board), the text of feedback-board posts you submit, app version and build, platform and device model, event timestamps, and a random analytics identifier. Analytics events are **not** linked to your name or email, and never include your artwork photos, personal notes, or device location. Your IP address is processed transiently by PostHog to receive events (and may be used to infer an approximate region). Steps you take during onboarding **before** answering the consent question are held only in the App's memory on your device and are transmitted (in order) solely if you then opt in; if you decline or close the App, they are discarded and never leave the device.

We do not use third-party advertising SDKs and we do not collect data for cross-app tracking.

---

## 3. How we use your information

- **To provide the App's core features:** identifying artworks from your photos, saving your artwork log, syncing across sessions, showing your collections and favorites, and generating art-history content about artworks you log.
- **To find museums near you** when you use nearby-discovery features.
- **To personalize** Learn content and recommendations based on your logged artworks and interactions.
- **To localize** the App and generated content into your preferred language.
- **To enforce fair-use limits** on AI-powered features and protect the service from abuse.
- **To maintain security,** debug problems, and operate the service.
- **To communicate with you** about your account (e.g., email confirmation, password reset).

We do not use your personal information for third-party advertising, and we do not sell it.

---

## 4. AI processing and third-party service providers

Artwork recognition and content generation are the core function of the App and depend on third-party AI providers. Before your first scan, the App shows a disclosure and asks for your permission; nothing is transmitted to AI providers until you agree, and declining simply leaves the photo unscanned on your device. **When you scan an artwork, the photo you submit (a cropped scan image) is transmitted to one or more of the following providers for processing:**

| Provider | Purpose | Data sent |
| --- | --- | --- |
| **Anthropic** (Claude models) | Artwork recognition from images; generation and translation of art-history content; Learn content | Your scan image; artwork/artist text and context from your logs |
| **OpenAI** (GPT models) | Artwork interpretation from images | Your scan image |
| **Google Cloud (Vertex AI)** | Image embeddings used to match your scan against known artworks | Your scan image |

Scan images are transmitted to these providers either directly within the processing request or via short-lived signed links to a private, access-controlled storage area. We do not send your name, email, or account details to AI providers with your images.

AI-generated descriptions of artworks are produced from retrieved sources (such as Wikipedia and museum databases) and may be stored and shown to you and, for shared canonical artworks, to other users.

We also use these non-AI service providers and data sources:

| Provider | Purpose | Data sent |
| --- | --- | --- |
| **Supabase** | Database, authentication, file storage, and serverless functions (our backend) | Account data, user content, photos, usage counters |
| **PostHog** | Opt-in product analytics (Section 2.3) | Usage events, feedback post text, app/device info, random analytics id — only after you opt in; never photos, notes, location, name, or email |
| **Geoapify** | Finding museums and art venues near you | Your approximate device coordinates |
| **OpenStreetMap (Overpass API)** | Fallback nearby-venue lookup | Your approximate device coordinates |
| **Apple Maps Server API** | Fallback nearby-venue lookup | Your approximate device coordinates |
| **Wikipedia / Wikimedia / Wikidata** | Retrieving factual information and public images about artworks and artists | Artwork/artist names only — no personal data |
| **Art Institute of Chicago API** and other museum open-data sources | Artwork reference data and images | Artwork queries only — no personal data |
| **Apple / Google sign-in** | Authentication, if you choose those sign-in methods | Handled under Apple's and Google's own privacy policies |

Each provider processes data under its own privacy policy. We share only what is needed for the feature you are using.

---

## 5. How your information is shared

We share personal information only:

- **With the service providers listed in Section 4**, to operate the App.
- **If required by law**, such as in response to a valid legal request.
- **In a business transfer**, such as a merger or acquisition, in which case this policy will continue to apply to previously collected data.
- **With your direction**, if you explicitly share content.
- **Feedback board.** If you post to the in-app community feedback board, the text of your post is visible to all signed-in users of the App. Posts are displayed **without your name or profile**; internally each post remains linked to your account for moderation, fair-use limits, and handling of reports.

**Important note on photos:** artwork photos attached to your log are stored in a storage bucket whose URLs are publicly readable. This means anyone who obtains a photo's URL can view that photo without logging in. Photo URLs are long and randomized, but you should not attach photos you would not want to be publicly accessible.

We do not sell personal information and have not sold personal information in the preceding 12 months. We do not "share" personal information for cross-context behavioral advertising as defined by California law.

---

## 6. Data retention

- **Account and content data** is retained while your account exists.
- **Scan crop images** submitted for recognition are stored short-term in a private bucket for processing and matching.
- **Usage counters** are kept as daily aggregates.
- **If your account is deleted,** your profile, artwork logs, photos' database records, notes, collections, favorites, learning data, interaction logs, and usage counters are deleted (our database is configured to cascade-delete user data when the account is removed). Backups may persist for a limited period before being overwritten in the ordinary course.

To request deletion, see Section 10.

---

## 7. Security

- All traffic between the App and our servers uses TLS encryption.
- Authentication sessions on your device are stored in the operating system's secure storage (iOS Keychain).
- Our database enforces row-level security: your private data is readable and writable only by your authenticated account.
- Passwords are handled and hashed by our authentication provider; we never store plaintext passwords.
- AI request logs record request outcomes, not the content of your prompts or images.

No system is perfectly secure. If we learn of a breach affecting your personal data, we will notify you as required by applicable law.

---

## 8. Your choices and controls

- **Camera, photo library, and location permissions** are optional and controlled in your device settings. Core scanning requires camera or photo access; nearby discovery requires location. The rest of the App works without them.
- **Photo metadata:** you can disable location tagging in your device camera settings if you don't want GPS embedded in your photos.
- **Language:** set in-app; stored on your profile.
- **Sign out** at any time; anonymous accounts are not silently recreated after an intentional sign-out.

---

## 9. Your privacy rights

Depending on where you live, you may have rights to access, correct, delete, or export your personal data, to object to or restrict certain processing, and to withdraw consent.

### 9.1 European Union / EEA (GDPR)

If you are in the EU/EEA, the data controller is **Alex Zhang, operator and data controller for MuseumLog** (contact details in Section 14). We rely on the following legal bases for each processing purpose:

| Processing purpose | Legal basis |
| --- | --- |
| Creating and operating your account, syncing your data | Performance of a contract |
| Recognizing an artwork from a photo you submit (including sending the photo to the AI providers in Section 4) | Performance of a contract |
| Storing your artwork log, notes, photos, collections, and favorites | Performance of a contract |
| Finding museums near you when you use nearby discovery (with your device location permission) | Performance of a contract — the feature runs only when you invoke it and have granted the permission |
| Reading photo metadata (EXIF location and date) to tag your own log entries | Performance of a contract |
| Personalizing Learn content from your in-app activity | Performance of a contract |
| Security, abuse prevention, and fair-use limits | Legitimate interests (protecting the service and all users; assessment available on request) |
| Essential operational logging | Legitimate interests |
| Optional product analytics (Section 2.3) | Consent — asked during onboarding, off unless you agree, withdrawable anytime via the permanent toggle in Profile → Privacy & Data |
| Responding to support and rights requests; legal compliance | Contract / legal obligation |

You have the right to **access**, **rectify**, **erase**, **restrict**, and **port** your personal data, to **object** to processing based on legitimate interests, and to **withdraw consent** at any time (withdrawing is as easy as granting: device permissions can be revoked in iOS Settings — a shortcut is in Profile → Privacy & Data). Withdrawal does not affect processing that already happened.

You also have the right to **lodge a complaint with a supervisory authority**, in particular in the EU/EEA country where you live or work. A list of authorities is at edpb.europa.eu.

We are assessing the appointment of an **EU representative under GDPR Article 27** and a **UK representative under UK GDPR Article 27**; if appointed, the representatives' names and contact details will be published here.

### 9.2 United Kingdom (UK GDPR)

If you are in the United Kingdom, the same rights and legal bases described in Section 9.1 apply under the **UK GDPR** and the Data Protection Act 2018, with Alex Zhang as controller. You may lodge a complaint with the **Information Commissioner's Office (ICO)** — ico.org.uk. Transfers of your data to the United States are protected as described in Section 12, including the UK Addendum / UK extension mechanisms.

### 9.3 Switzerland (FADP)

If you are in Switzerland, we process your personal data in accordance with the Swiss **Federal Act on Data Protection (FADP)**. You have equivalent rights of access, rectification, erasure, and objection, exercisable via the contact in Section 14, and you may contact the **Federal Data Protection and Information Commissioner (FDPIC)** — edoeb.admin.ch. Transfers abroad rely on the safeguards in Section 12 as recognized for Switzerland.

### 9.4 California (CCPA/CPRA)

You have the right to know, delete, correct, and to opt out of sale/sharing. We do not sell or share personal information as defined by the CPRA. We do not discriminate against you for exercising rights.

### 9.5 Other jurisdictions

We will honor applicable rights requests.

To exercise any right, contact museumlog.app@gmail.com. We may need to verify your identity (e.g., confirming control of the account email) before acting on a request. We will respond without undue delay and within the time required by applicable law (for GDPR requests, within one month, extendable for complex requests with notice).

---

## 10. Account deletion

You may delete your account and associated data at any time using **Delete Account** in the App (Profile → Settings → Account), or by emailing museumlog.app@gmail.com from your account email with the subject "Delete my account." Deletion removes your profile and user content as described in Section 6.

---

## 11. Children's privacy

The App is not directed to children, and **during the beta program you must be at least 18 years old to use it** (see the Terms of Service and Beta Program Terms). We do not knowingly collect personal information from anyone under 18. If you believe someone under 18 has provided us personal information, contact museumlog.app@gmail.com and we will delete it.

---

## 12. International data transfers

Our servers and most of our service providers are located in the **United States** (our primary database is hosted in the AWS us-east-1 region). If you use the App from the EU/EEA, the United Kingdom, or Switzerland, your personal data is transferred to and processed in the United States.

For these transfers we rely on the safeguards recognized under Chapter V of the GDPR for each provider: certification under the **EU-U.S. Data Privacy Framework** where the provider is certified, and the European Commission's **Standard Contractual Clauses** incorporated in our data processing agreement with the provider otherwise. For the **United Kingdom** we rely on the corresponding UK mechanisms (the UK Extension to the Data Privacy Framework where the provider is certified for it, or the UK International Data Transfer Addendum to the SCCs); for **Switzerland**, on the Swiss recognition of these mechanisms (including the Swiss-U.S. extension of the Data Privacy Framework where applicable) with the adaptations required by the FDPIC. The per-provider mechanism is listed below and kept current; you can request details at museumlog.app@gmail.com.

| Provider | Role | Transfer safeguard |
| --- | --- | --- |
| Supabase (hosting, database, storage, auth) | Processor | Data processing agreement incorporating the EU Standard Contractual Clauses |
| Anthropic | Processor | Data processing addendum incorporating the EU Standard Contractual Clauses; Anthropic does not train models on API data |
| OpenAI | Processor | Data processing addendum incorporating the EU Standard Contractual Clauses; OpenAI does not train models on API data by default |
| Google Cloud (Vertex AI) | Processor | Certified under the EU-U.S. Data Privacy Framework; Cloud Data Processing Addendum with EU Standard Contractual Clauses |
| Geoapify | Processor | EU-established provider (Geoapify GmbH, Germany) with EU hosting — no third-country transfer by us |
| PostHog (opt-in analytics only) | Processor | Data processing agreement incorporating the EU Standard Contractual Clauses (US hosting) |

Requests to Wikipedia, Wikidata, and museum open-data APIs contain artwork queries only, not your personal data.

---

## 13. Changes to this policy

We may update this policy from time to time. Material changes will be communicated in the App or by email before they take effect. The "Last updated" date at the top reflects the latest revision. Continued use after changes take effect constitutes acceptance.

---

## 14. Contact

Alex Zhang, operator and data controller for MuseumLog
museumlog.app@gmail.com

EU representative (GDPR Article 27) and UK representative (UK GDPR Article 27): appointment in progress; details will be published here.
