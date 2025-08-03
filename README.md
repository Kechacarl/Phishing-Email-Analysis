# Phishing-Email-Analysis
investigating a given phishing email to reveal the risks involved 

# Phishing Email Analysis Report
Summary of Findings
This email exhibits multiple classic phishing indicators. The sender is impersonating a legitimate entity and is attempting to elicit a response that involves a financial transaction and the download of a malicious file.

Technical Analysis (Email Headers)

The email headers provide clear evidence of spoofing and failed security checks.

Sender Address: The email claims to be from "Bill" at billjobs@microapple.com. This domain microapple.com is a clear attempt to impersonate both Microsoft and Apple, a common tactic in phishing scams. The Return-Path also points to this same fraudulent address.

Reply-To Address: The Reply-To address is negeja3921@pashter.com, which is completely different from the sender's address. This is a major red flag, as it indicates the scammer wants replies to go to a different, likely disposable, email account.

SPF Authentication Failure: The Received-SPF header explicitly states spf=fail. This means the server that sent the email (93.99.104.210) was not authorized to send mail on behalf of the microapple.com domain, confirming the email is forged.

Originating IP: The email was received from localhost at the IP address 93.99.104.210, which resolves to emkei.cz. Emkei.cz is a known online service for creating fake emails, which is a strong indicator that this is a simulated attack.

Return-Path: <billjobs@microapple.com>
Received-SPF: fail (google.com: domain of billjobs@microapple.com does not designate 93.99.104.210 as permitted sender)
Received: from localhost (emkei.cz. [93.99.104.210])
Reply-To: negeja3921@pashter.com
From: "Bill" <billjobs@microapple.com>

Content Analysis (Email Body & Attachment)

The content of the email and its attachment are designed to manipulate the recipient into taking a specific action.

Social Engineering: The email uses a high-stakes, urgent scenario involving "abducted CoCanDians" and the "President’s daughter" to create a sense of panic and urgency. This is a classic tactic to bypass rational thinking.

Call to Action: The sender demands "1 Billion CoCanDs" in cash, with the promise that they will "safely bring back your citizens" in a "spaceship" with "autonomous bots". The request is absurd, which is a sign of a fraudulent request.

Lack of Personalization: The email starts with a generic "Hi TheMajorOnEarth," rather than a specific name, which is a common feature of mass-sent phishing emails.

Attachment: The email contains a PDF attachment named "PuzzleToCoCanDa.pdf". The body of the email instructs the user to "solve the puzzle" for the "next steps". This attachment is a malicious payload that is likely designed to deliver malware or other threats when opened. The email also contains a "hint" for the puzzle: "Don't Trust Your Eyes".

Call for Action (For Organizational Employees)

If you receive an email of this nature, please take the following steps immediately to protect yourself and the organization:

Do Not Engage: Do not reply to the email, click any links, or open any attachments, regardless of how convincing the message may seem. The attachment is likely malicious and could infect your computer or the company network.

Isolate: Delete the email from your inbox and, if possible, from your "deleted" or "trash" folder.

Report Immediately: Forward the full email, including its headers, to the organization's IT or security department. Do not simply forward the body of the email; use the "Forward as attachment" or "Show original" feature to capture all technical details.

Confirm Authenticity: If the email claims to be from a known colleague or a legitimate business partner, do not trust the email address provided. Instead, use an alternative, trusted communication channel (e.g., phone call, corporate messaging platform) to independently verify the request.

Stay Vigilant: Remain aware of other similar messages and report them to the security team. Phishing campaigns often target multiple employees at once.
