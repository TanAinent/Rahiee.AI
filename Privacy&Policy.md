# Rahiee.AI Privacy Policy

**Effective date:** 1 November 2025  
**Last updated:** 11 November 2025  

Rahiee.AI ("the App") is provided by **TanAiNent** ("we", "us", "our") as a commercial HR management platform. This Privacy Policy explains what personal information we collect, how we use it, with whom it may be shared, and the choices available to you. By installing or using the App you confirm that you have read and understood this Policy.

---

## 1. Scope

This Policy covers information processed through:

- The Rahiee.AI Android and iOS applications.
- The web-based admin console.
- Backend services hosted primarily on Supabase (PostgreSQL, storage, authentication), Firebase Cloud Messaging, and other integrated third-party providers listed below.

It applies to administrators, HR managers, and employees who use Rahiee.AI within their organization.

---

## 2. Information We Collect

We collect and process the following categories of data:

### 2.1 Account & Profile Data
- **Full name** - used for product personalization and app functionality (linked to identity, used for tracking)
- **Email address** - used for app functionality and product personalization (linked to identity, used for tracking)
- **Phone number** - used for app functionality and product personalization (linked to identity, used for tracking)
- **Physical address** - used for product personalization (linked to identity, used for tracking)
- Employee ID, department, job title
- Authentication credentials (hashed passwords, OAuth tokens)
- Administrative roles, access permissions, and employment status

### 2.2 HR & Scheduling Data
- Work schedules, assignments, shifts, calendar events
- Leave requests, approvals, exchange requests, attendance records
- Notes added by supervisors (e.g., reasons for schedule changes or attendance overrides)

### 2.3 Attendance Evidence
- **Camera images / Photos or Videos** - captured at check‑in and check‑out for identity verification and uniform compliance (linked to identity, used for tracking, used for app functionality)
- **Precise geolocation data** - GPS coordinates, address approximation, timestamps associated with attendance events to confirm on-site presence (linked to identity, used for tracking, used for app functionality)
- Device metadata (uniform detection scores, ML model confidence, device model, OS version)

### 2.4 Usage & Diagnostic Data
- **Device ID** - used for app functionality and other purposes including analytics (linked to identity)
- App crash logs, performance metrics, debounced API calls, analytics events (pages/screens viewed, time on screen)
- Push notification tokens, IP address, network status
- Notifications sent, read receipts, and interaction history

### 2.5 Optional Integrations
- Files uploaded to Supabase storage (e.g., policy documents, employee assets)
- Data exchanged via APIs or RPCs (e.g., `get_schedules_with_attendance_status`, `get_realtime_dashboard_stats`)

We do **not** knowingly collect sensitive personal information beyond what is required for HR operations. If your organization uploads such data, it is responsible for ensuring a lawful basis and notifying affected users.

---

## 3. How We Use Information

We process personal data to:

1. **Provide core HR features** – create and manage schedules, record attendance, process leave/exchange requests, and display dashboard analytics
2. **Authenticate users** – manage secure login with Supabase Auth, role-based access, session management
3. **Verify attendance** – validate check-ins via camera capture, ML inference, GPS coordinates, and schedule alignment
4. **Notify users** – send push/email/SMS notifications for schedule changes, approvals, or urgent messages via Firebase Cloud Messaging or similar channels
5. **Improve reliability** – monitor performance, debug issues, enforce debouncing and race-condition safeguards, and enhance user experience
6. **Product personalization** – customize the app experience based on user role, preferences, and organizational structure
7. **Comply with legal obligations** – maintain audit trails, respond to lawful requests, maintain tax/attendance records where required

Processing is based on contractual necessity (delivering HR services to your organization), legitimate interests (security, optimization), and, when required, consent (e.g., camera and location permissions).

---

## 4. Data Used to Track You

The following data **may be used to track you** across apps and websites owned by other companies for analytics and service improvement purposes:

- **Precise location** - to analyze attendance patterns and optimize scheduling
- **Contact information** (name, email, phone, physical address) - to identify users across sessions and provide personalized experiences
- **User content** (photos/videos) - attendance verification images may be used to improve ML models and attendance accuracy
- **Device ID** - to maintain consistent user sessions and analytics

You can limit tracking by:
- Disabling location services when not checking in/out
- Opting out of analytics in Settings (where available)
- Using your device's "Ask App Not to Track" feature (iOS 14.5+)

---

## 5. Sharing & Third-Party Processing

We limit sharing to what is necessary to operate the App:

| Recipient | Purpose | Key Safeguards |
|-----------|---------|----------------|
| **Supabase** (PostgreSQL, Storage, Auth, Edge Functions) | Hosting databases, files, RPC execution | Compliant with SOC 2, GDPR-ready controls |
| **Firebase Cloud Messaging / Google Play Services** | Push notifications, device tokens | Follows Google privacy and security policies |
| **Google Analytics for Firebase / Crashlytics** (if enabled) | Usage analytics, crash reporting | Aggregated telemetry; you may disable via settings |
| **Payment / Payroll integrations** (optional) | Payroll calculations if configured | Subject to separate agreements |
| **TanAiNent support staff** | Troubleshooting, customer support | Staff bound by confidentiality commitments |
| **Law enforcement or regulators** | Legal compliance | Only upon lawful request and minimal disclosure |

We do **not** sell personal data. Third parties are contractually obligated to protect information, use it solely for our instructions, and delete it upon request.

---

## 6. Data Retention

- **Account data**: retained while the employer maintains a contract with TanAiNent plus up to 180 days for backup and audit, unless a longer period is mandated by law
- **Attendance records & schedules**: stored as long as required by employment law or client policy (typically 3–7 years)
- **Camera images & ML metadata**: retained for 90 days by default (configurable by the client) then deleted unless linked to an active investigation
- **Logs & analytics data**: anonymized and retained up to 24 months

You may request deletion of user-provided data by emailing **rahieeislam@gmail.com**. We may retain limited information if required for legal compliance, dispute resolution, or security.

---

## 7. Your Rights & Privacy Choices

Depending on your jurisdiction and employer policies, you may have the right to:

- Access, correct, or update your profile information
- Request deletion of your data (subject to HR/legal retention requirements)
- Restrict or object to certain processing (e.g., marketing communications, analytics)
- Port your data to another service
- Opt out of cross-app tracking (iOS: Settings → Privacy → Tracking)
- Revoke location or camera permissions (device settings)

**User Privacy Choices:**
- You can manage notification preferences in-app via Settings → Notifications
- Control location tracking via device settings
- Request data export or deletion by contacting your HR administrator or emailing **rahieeislam@gmail.com**

Employees should first contact their HR administrator. We support admin-led deletion or export via Supabase, or you can email **rahieeislam@gmail.com** with details. We respond within 30 days.

---

## 8. Security

We implement administrative, technical, and physical safeguards:

- TLS encryption in transit, AES-256 at rest (Supabase managed)
- Role-based access control and fine-grained policies (Row Level Security) across schedules, attendance, and notifications
- Logging, alerting, and periodic security reviews
- Secure development practices (static analysis, linting, code reviews)
- Minimum privilege service accounts; secrets stored via environment variables and Supabase config

No system is completely secure; in case of a breach we will notify affected organizations and authorities in accordance with applicable law.

---

## 9. Children's Privacy

Rahiee.AI is intended for adult workplace users (18+). We do not knowingly collect data from individuals under 16 (or lower age permitted by local law). If we learn that a minor's data has been submitted, we will delete it promptly. Parents or guardians should contact **rahieeislam@gmail.com** if they believe their child's data has been provided.

---

## 10. International Transfers

Data may be stored on Supabase or Firebase infrastructure located in the United States or European Union. When transferring data across regions, we rely on appropriate safeguards (e.g., Standard Contractual Clauses, DPAs). Employer administrators may configure region-specific storage where available.

---

## 11. Permissions & In-App Controls

When you install the App, you may be prompted to grant:

- **Camera** – required for attendance image capture and uniform verification
- **Location (Precise)** – used to verify check-in/out locations; precise location is stored only with attendance records
- **Notifications** – to deliver schedule updates and approvals
- **Storage** – for caching, uploading attachments

You can revoke permissions via device settings:
- **iOS**: Settings → Rahiee.AI → [Permission Type]
- **Android**: Settings → Apps → Rahiee.AI → Permissions

**Important:** Some features may not function without required permissions. For example, attendance check-in requires both camera and location access.

---

## 12. Marketing Communications

We may send administrative or marketing emails (e.g., new feature announcements) to organization administrators or users who opt in. You can unsubscribe via the email footer or by contacting us.

---

## 13. Changes to This Policy

We may update this Policy to reflect product changes or legal requirements. We will notify administrators via in-app alerts or email, and update the "Last updated" date. Material changes become effective 30 days after notice unless required sooner by law. Continued use of Rahiee.AI after updates constitutes acceptance.

Previous versions of this Policy are available upon request.

---

## 14. Contact Us

For privacy questions, data access or deletion requests, or security concerns, contact:

**TanAiNent – Rahiee.AI Privacy Team**  
**Email:** rahieeislam@gmail.com  
**Privacy Policy URL:** [Your URL here]  
**User Privacy Choices URL:** [Your URL here] *(if applicable)*

If we do not resolve your concern, you may have the right to contact your local data protection authority.

---

## 15. Additional Disclosures for App Stores

### Apple App Store Compliance
- Rahiee.AI complies with Apple's App Store Review Guidelines and App Tracking Transparency framework
- We provide in-app access to this Policy via Settings → Privacy Policy
- Data safety labels in App Store Connect reflect the collection categories outlined above
- Seven data types are collected: Email Address, Device ID, Precise Location, Photos or Videos, Phone Number, Physical Address, Name

### Google Play Store Compliance
- Rahiee.AI complies with Google Play User Data Policies, including limited use of sensitive permissions (camera, location)
- Biometric, camera, or location data is used solely for attendance verification and is not shared for advertising
- We provide in-app access to this Policy via Settings → Privacy Policy
- Data safety labels in Play Console reflect the collection categories outlined above

### Data Collection Summary
All collected data types serve specific purposes:

| Data Type | Primary Purpose | Tracking | Linked to Identity |
|-----------|----------------|----------|-------------------|
| Name | Product Personalization, App Functionality | Yes | Yes |
| Email Address | App Functionality, Product Personalization | Yes | Yes |
| Phone Number | App Functionality, Product Personalization | Yes | Yes |
| Physical Address | Product Personalization | Yes | Yes |
| Precise Location | App Functionality (attendance verification) | Yes | Yes |
| Photos/Videos | App Functionality (attendance verification) | Yes | Yes |
| Device ID | App Functionality, Analytics | No | Yes |

---

## 16. California Privacy Rights (CCPA)

California residents have specific rights under the California Consumer Privacy Act:

- **Right to Know:** Request disclosure of personal information collected, used, or shared
- **Right to Delete:** Request deletion of personal information (subject to exceptions)
- **Right to Opt-Out:** Opt out of "sale" of personal information (we do not sell data)
- **Right to Non-Discrimination:** Equal service regardless of privacy choices

To exercise these rights, contact **rahieeislam@gmail.com** with "California Privacy Request" in the subject line.

---

## 17. European Privacy Rights (GDPR)

For users in the European Economic Area, United Kingdom, or Switzerland:

- **Legal basis for processing:** Contract performance, legitimate interests, consent
- **Data transfers:** Standard Contractual Clauses or adequacy decisions
- **Right to lodge complaint:** Contact your local supervisory authority
- **Data Protection Officer:** Available at rahieeislam@gmail.com for GDPR inquiries

---

By installing or using Rahiee.AI, you acknowledge that you have read and understood this Privacy Policy.

---

*Last reviewed: 11 November 2025*  
*Version: 2.0*
