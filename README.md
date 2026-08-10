Topic: CO1 
Security Features in Real-World Applications

1. Identify any five real-world applications or online services that involve communication, authentication, or transactions. For each application, investigate and identify:

The security feature/service required, such as confidentiality, integrity, authentication, authorization, availability
The security mechanism used to provide the identified security feature.
The security protocol or technology used to implement the mechanism.
Briefly explain how the mechanism/protocol provides the identified security feature.

Present your findings in the following format:

| Application           | Security Feature             | Security Mechanism     | Protocol / Technology         | How it provides security                            |
| ---------------       | ----------------             | ------------------     | ----------------------        | --------------------------------------------------|
| Gmail                 | Authentication               | Password + MFA         | OAuth                         | Verifies the identity of the user                   |
| Online banking        | Confidentiality              | Encryption             | HTTPS/TLS                     | Protects data transmitted between client and server |
| Adhaar                | Authentication               | Biometric verification | OTP + Fingerprints/ Iris scan | Verifies identity through unique physical traits|
| College Result portal | Integrity                    | Hashing/ Checksum      | HTTPS/TLS                     | Ensures marks are not tampered with in transit     |
| Netflix               | Availability                 | Load balancing, CDN    | Content delivery network      | Ensures reliable performance under high traffic  |
| Instagram             | Authentication               | Password + OTP         | OAut HTTPS                    | Verifies the identity before granting the account access|
| Uber/Ola              | Authentication               | OTP                    | SMS OTP/ HTTPS                | Verifies the driver and rider identity befor the trip |


2. For any five real-world applications, investigate the security controls used to protect users and data. Classify the controls based on whether they provide Confidentiality, Integrity, or Availability, and determine how these controls help in preventing, detecting, and recovering from security attacks. Mention the mechanisms and protocols involved.

|Application     |Security control              | CIA          | Preventing               | Dectecting      | Recovering   | Mechanism/Protocol          |
|--------------- |------------------------------|--------------|--------------------------|-----------------|--------------|-----------------------------|
|Online banking  |Encryption + OTP                |Confidentiality|	Stops anyone other than users from reading your data or logging in without OTP|	Alerts if login is tried from a new device| Allows to freeze account/reset password if hacked|	SSL/TLS, HTTPS, OTP, 2FA|
|Gmail           | Spam/Phishing filters + Digital Signatures | Integrity | Blocks fake/malicious emails before they reach inbox | Flags suspicious sender addresses and links | Allows to report phishing, which improves future filtering | DKIM, SPF, DMARC |
| Amazon         | Firewalls + Load Balancers   | Availability | Blocks malicious traffic (like DDoS attacks) from crashing the site | Amazon's systems constantly monitor traffic patterns. If they suddenly see traffic spike 100x normal which is way more than a regular sale, the system flags it as suspicious. This could mean an attack is happening. | Redirects traffic to backup servers to keep site running | Firewall, DDoS protection, Load Balancing | 
Instagram | Two-Factor Authentication + Hashing (passwords)	| Confidentiality + Integrity | Even if the password leaks in a data breach, the hacker still cannot login without the 2FA code sent to the user's personal phone/email. This stops account takeover before it happens. | Detects login attempts from unknown locations | Allows to  recover account via email/phone verification | 2FA, Password Hashing (bcrypt), HTTPS | 

