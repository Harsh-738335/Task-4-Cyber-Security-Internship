🔐 Task 4: Password Security & Authentication Analysis
📌 Objective

The objective of this task is to understand how passwords are stored, analyzed, attacked, and protected using secure authentication mechanisms. This task focuses on password hashing, common attack techniques, and modern defenses like Multi-Factor Authentication (MFA).

🛠 Tools Used

Primary Tools: Hashcat, John the Ripper

Alternative Tools: Online Hash Identifiers

📖 Understanding Password Storage
Hashing vs Encryption

Hashing is a one-way process used to securely store passwords.

Encryption is a two-way process and is not recommended for password storage.

Conclusion:
Passwords should always be stored using cryptographic hash functions, not encryption.

🔍 Identification of Hash Types
Hash Type	Length	Description
MD5	32 characters	Fast but insecure
SHA-1	40 characters	Vulnerable to collisions
bcrypt	60 characters	Secure and slow

Example MD5 hash:

password123 → 482c811da5d5b4bc6d497ffa98491e38

🔐 Password Hash Generation

Passwords were converted into hashes using common hashing algorithms such as MD5 and SHA-1 to demonstrate how plain-text passwords are stored securely.

Example:

Plain Password: admin123
MD5 Hash: 0192023a7bbd73250516f069df18b500

⚔️ Password Cracking Techniques
Dictionary Attack

Uses common password lists (e.g., rockyou.txt)

Effective against weak passwords

Brute Force Attack

Tries all possible combinations

Time-consuming but guaranteed over time

Observation:
Weak passwords are cracked within seconds using dictionary attacks.

❌ Why Weak Passwords Fail

Short length

Predictable patterns

Commonly used words

Reused across platforms

Examples of weak passwords:

123456
password
admin

🔑 Multi-Factor Authentication (MFA)
What is MFA?

MFA requires more than one authentication factor:

Password

OTP / Authenticator App

Biometric verification

Importance of MFA

Prevents unauthorized access even if passwords are compromised

Adds an additional security layer

✅ Recommendations for Strong Authentication

Use bcrypt or Argon2 for password hashing

Enforce minimum password length (12–16 characters)

Enable Multi-Factor Authentication

Implement account lockout and rate limiting

Avoid password reuse

Educate users about password security

🎯 Final Outcome

Understanding of password storage mechanisms

Knowledge of password attacks and defenses

Awareness of modern authentication best practices
