Privacy Policy for QRResearchr
Last updated: October 14, 2026
This Privacy Policy explains how QRResearchr ("the Application", "we", "us", or "our") handles user information when you use our mobile application. We are committed to protecting your privacy and ensuring transparency regarding any device permissions and data interactions.
1. Summary of Core Privacy Principles
   Zero Personal Information Collection: We do not collect, store, sell, or transmit any personally identifiable information (such as your name, email, phone number, physical address, contacts, or photos).
   No Account Required: You can use all core features of QRResearchr without creating an account or logging in.
   On-Device Camera Processing: Camera frames are processed strictly in-memory on your physical device to decode QR codes and barcodes. No photos, videos, or image buffers are ever saved or uploaded.
   Local Data Storage: Your scan history and domain blacklist remain exclusively on your local device storage.
   Zero Third-Party Advertising: We do not display third-party advertisements or integrate tracking SDKs.
2. Device Permissions & How They Are Used
   QRResearchr requests the minimum necessary permissions required for core utility functionality:
   A. Camera Access (android.permission.CAMERA)
   Purpose: Allows the application to access your device's camera hardware to scan and decode barcodes and QR codes in real-time.
   Handling: The camera stream is passed directly to the on-device Google ML Kit Barcode Scanning API. Camera frames are processed transiently in volatile memory (RAM) and immediately discarded.
   What we do NOT do: We do not take photos, record audio/video, access your device photo gallery, or transmit image streams over any network.
   B. Network Access (android.permission.INTERNET)
   Purpose: Used exclusively to perform automated security and threat analysis on scanned URLs when requested.
   Handling: When a scanned QR code contains a web address (URL), the application performs network operations to check SSL/TLS certificate validity, verify HTTP/HTTPS protocols, detect raw IP endpoints, and resolve redirect chains (e.g., expanding short links).
   What we do NOT do: We do not associate URL lookups with your device identifier or user profile.
3. Data Storage & Retention
   Scan History: When you scan a QR code, the text content, timestamp, and security risk score are stored locally on your device within an encrypted Android Room SQLite database.
   Domain Blacklist: Domains you manually choose to block or flag are stored strictly on your local device.
   Data Deletion: You have full control over your stored data. You can delete individual items or purge your entire scan history at any time from within the Application's History tab. Uninstalling the Application permanently removes all locally stored data.
4. Third-Party Services & Libraries
   The Application utilizes established, vetted open-source libraries and platform frameworks:
   Google ML Kit Barcode Scanning: Provides high-efficiency, on-device barcode parsing.
   Android Jetpack Libraries (CameraX, Compose, Room): Core operating system components developed and maintained by Google.
   The Application does not include third-party marketing SDKs, tracking pixels, or cross-app analytics trackers (such as Facebook SDK, AppsFlyer, or Google AdMob).
5. Children's Privacy (COPPA Compliance)
   QRResearchr is a general-purpose security and utility tool. We do not knowingly collect or solicit personal data from children under the age of 13. Because our Application does not collect personal information from any user, we adhere strictly to the Children's Online Privacy Protection Act (COPPA) and Google Play Families Policy requirements.
6. Security Safeguards
   We implement industry-standard security measures within the Application's design:
   Network communications for URL security analysis enforce encrypted HTTPS protocols.
   Discovered URLs are rendered with defensive defanging (e.g., hxxps://...) to prevent accidental tap execution of malicious scripts.
   Local application databases are isolated within Android's protected application sandbox.
7. Changes to This Privacy Policy
   We may update this Privacy Policy periodically to reflect improvements in application functionality or regulatory requirements. Any modifications will be updated on this page with a revised "Last updated" date.
8. Contact Information
   If you have questions, feedback, or concerns regarding this Privacy Policy or the security practices of QRResearchr, please contact us at:
   Email: student.smihayesi@gmail.com
   Developer: QRResearchr Developer Team