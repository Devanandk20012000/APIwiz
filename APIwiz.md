---


---

<h1 id="automating-gmail-drafts-from-google-sheets-using-make.com">Automating Gmail Drafts from Google Sheets using <a href="http://Make.com">Make.com</a></h1>
<h2 id="table-of-contents">Table of Contents</h2>
<ul>
<li><a href="#introduction">Introduction</a></li>
<li><a href="#system-requirements">System Requirements</a></li>
<li><a href="#security-measures">Security Measures</a></li>
<li><a href="#persona-storyline">Persona Storyline</a>
<ul>
<li><a href="#meet-devanand--sales-coordinator-at-all-jordan">Meet Devanand – Sales Coordinator at ALL-Jordan</a></li>
</ul>
</li>
<li><a href="#prerequisites">Prerequisites</a>
<ul>
<li><a href="#tools-you-will-need">Tools You will Need</a></li>
<li><a href="#what-to-prepare">What to Prepare</a></li>
</ul>
</li>
<li><a href="#real-world-templates">Real-World Templates</a></li>
<li><a href="#use-cases">Use Cases</a></li>
<li><a href="#advantages-and-applications">Advantages and Applications</a>
<ul>
<li><a href="#key-benefits">Key Benefits</a></li>
</ul>
</li>
<li><a href="#marketplace-reference">Marketplace Reference</a></li>
<li><a href="#saleo-guided-tour">Saleo Guided Tour</a>
<ul>
<li><a href="#what-the-tour-includes">What the Tour Includes</a></li>
<li><a href="#getting-stuck">Getting Stuck?</a></li>
<li><a href="#access-the-guided-tour">Access the Guided Tour</a></li>
<li><a href="#tip">Tip</a></li>
</ul>
</li>
<li><a href="#customization-options">Customization Options</a></li>
<li><a href="#troubleshooting-and-known-issues">Troubleshooting and Known Issues</a>
<ul>
<li><a href="#error-it-is-not-possible-to-use-restricted-scopes-with-customer-gmailcom-accounts">Error: “It is not possible to use restricted scopes with customer @gmail.com accounts”</a></li>
<li><a href="#other-common-issues">Other Common Issues</a></li>
</ul>
</li>
<li><a href="#frequently-asked-questions">Frequently Asked Questions</a></li>
<li><a href="#support">Support</a></li>
<li><a href="#glossary">Glossary</a></li>
<li><a href="#legal-notice">Legal Notice</a></li>
<li><a href="#copyright">Copyright</a></li>
</ul>
<hr>
<h2 id="introduction">Introduction</h2>
<p>Effective communication is a cornerstone of customer engagement, sales outreach, and operational follow-ups. However, manually composing personalised emails for every new lead or contact can be time-consuming, inconsistent, and subject to human error.</p>
<p>This user guide provides step-by-step instructions for configuring an automation workflow that connects <strong>Google Sheets</strong> and <strong>Gmail</strong> using <strong><a href="http://Make.com">Make.com</a></strong>. The objective is to automatically generate a Gmail draft message each time a new row is added to a specified Google Sheet.</p>
<p>This guide is intended for users of all backgrounds; whether you are a business professional, educator, freelancer, startup founder, or simply looking to automate your daily email workflows. If you have a basic understanding of web-based tools, you will be able to configure and benefit from this automation with ease.</p>
<hr>
<h2 id="system-requirements">System Requirements</h2>

<table>
<thead>
<tr>
<th>Component</th>
<th>Requirement</th>
</tr>
</thead>
<tbody>
<tr>
<td>Browser</td>
<td>Chrome, Firefox, Edge, Opera</td>
</tr>
<tr>
<td>Operating System</td>
<td>Windows 10+, macOS, Linux</td>
</tr>
<tr>
<td>Internet Connection</td>
<td>Stable broadband recommended</td>
</tr>
<tr>
<td><a href="http://Make.com">Make.com</a> Access</td>
<td>Free or Paid account</td>
</tr>
<tr>
<td>Google Workspace</td>
<td>Access to Gmail and Google Sheets</td>
</tr>
</tbody>
</table><hr>
<h2 id="security-measures">Security Measures</h2>
<ul>
<li>OAuth 2.0 is used for all Google account connections within <a href="http://Make.com">Make.com</a>.</li>
<li>Gmail and Sheets access is read/write only based on granted permissions.</li>
<li>No third-party has access to your credentials or email content.</li>
<li>You can revoke <a href="http://Make.com">Make.com</a> access anytime via your <a href="https://myaccount.google.com/permissions">Google Account Settings</a>.</li>
</ul>
<hr>
<h2 id="persona-storyline">Persona Storyline</h2>
<h3 id="meet-devanand-–-sales-coordinator-at-all-jordan">Meet Devanand – Sales Coordinator at ALL-Jordan</h3>
<p>Devanand handles dozens of new leads daily. He used to spend hours copying and pasting the same message over and over. It was tedious, error-prone, and prevented him from following up with warm leads quickly.</p>
<p>After implementing this Gmail automation:</p>
<ul>
<li>Each new row in his Google Sheet automatically creates a Gmail draft.</li>
<li>The draft is personalised with the recipient’s name, company, and industry.</li>
<li>Devanand just reviews the draft, customises if needed, and clicks send.</li>
</ul>
<blockquote>
<p>“This automation transformed my workflow. What used to take hours now takes minutes. I just reviewed the draft and hit send!”<br>
— <strong>Devanand</strong>, Sales Coordinator</p>
</blockquote>
<hr>
<h2 id="prerequisites">Prerequisites</h2>
<h3 id="tools-you-will-need">Tools You will Need</h3>

<table>
<thead>
<tr>
<th>Tool</th>
<th>Purpose</th>
<th>Link</th>
</tr>
</thead>
<tbody>
<tr>
<td>Google Account</td>
<td>Access Gmail &amp; Google Sheets</td>
<td><a href="https://accounts.google.com">accounts.google.com</a></td>
</tr>
<tr>
<td><a href="http://Make.com">Make.com</a> Account</td>
<td>Build and manage workflows</td>
<td><a href="https://www.make.com">make.com</a></td>
</tr>
</tbody>
</table><h3 id="what-to-prepare">What to Prepare</h3>
<ul>
<li>
<p>A Google Sheet with the following column headers:</p>
<ul>
<li><code>Name</code></li>
<li><code>Company</code></li>
<li><code>Email</code></li>
<li><code>Industry</code></li>
<li><code>Lead Status</code></li>
</ul>
</li>
<li>
<p>A Gmail template message like:</p>
</li>
</ul>
<p><strong>Subject</strong>:<br>
<code>Thanks for connecting, {{First Name}}! Let’s explore how we can help.</code></p>
<p><strong>Body</strong>:<br>
Hi {{First Name}},</p>
<p>Thank you for showing interest in our services. We noticed that you are part of the {{Industry}} sector, and we would love to explore how we can support your business needs.</p>
<p>If this is a good time, we would be happy to schedule a quick call or share more information tailored to your goals. Feel free to reply to this email at your convenience.</p>
<p>Looking forward to connecting with you!</p>
<p>Best regards,<br>
Devanand<br>
ALL-Jordan<br>
7012975405<br>
<a href="mailto:25381dev267@gmail.com">25381dev267@gmail.com</a></p>
<hr>
<h2 id="real-world-templates">Real-World Templates</h2>
<p>To help you get started instantly, use our ready-made Google Sheet template. It includes sample data and properly labeled columns that are compatible with the automation scenario described in this guide.</p>
<p><strong>Copy this template</strong>:<br>
<a href="https://docs.google.com/spreadsheets/d/1EmRP6TWzn2ApYBgxuUzJ5v6ggBLmUbtSpq62MIuJZhc/edit?usp=drive_link">Google Sheets – Email Automation Template</a></p>
<blockquote>
<p>💡 Tip: Make a copy in your own Google Drive before editing. Go to <code>File &gt; Make a Copy</code>.</p>
</blockquote>
<hr>
<h2 id="use-cases">Use Cases</h2>
<ul>
<li>Lead generation follow-up emails</li>
<li>Customer onboarding sequences</li>
<li>Reminder or appointment notifications</li>
<li>Internal team updates based on tasks</li>
<li>Event follow-ups or thank-you notes</li>
<li>Survey requests and feedback loops</li>
</ul>
<hr>
<h2 id="advantages-and-applications">Advantages and Applications</h2>
<h3 id="key-benefits">Key Benefits</h3>
<ul>
<li><strong>Save Time and Reduce Manual Work</strong></li>
<li><strong>Deliver Personalized Emails at Scale</strong></li>
<li><strong>Stay Professional and Consistent</strong></li>
<li><strong>Speed Up Lead Response Times</strong></li>
<li><strong>Enable Team Collaboration</strong></li>
<li><strong>Improve Tracking</strong></li>
</ul>
<hr>
<h2 id="marketplace-reference">Marketplace Reference</h2>
<p>This scenario is based on the <a href="http://Make.com">Make.com</a> template:</p>
<p>🔗 <a href="https://www.make.com/en/templates/5765-create-a-gmail-draft-message-from-a-new-google-sheets-row">Create a Gmail draft message from a new Google Sheets row</a></p>
<hr>
<h2 id="saleo-guided-tour">Saleo Guided Tour</h2>
<p>Saleo is a powerful in-app guidance tool that delivers real-time walkthroughs and interactive overlays on top of live software environments. It is used here to simulate the entire automation flow without requiring you to leave the <a href="http://Make.com">Make.com</a> platform or read long-form documentation separately.</p>
<hr>
<h3 id="what-the-tour-includes">What the Tour Includes</h3>
<p>The Saleo Guided Tour for this automation includes:</p>
<ul>
<li>
<p><strong>Page Linking</strong><br>
Automatically takes you to the relevant screen or module in <a href="http://Make.com">Make.com</a>.</p>
</li>
<li>
<p><strong>Interactive Tooltips</strong><br>
Short, informative prompts that explain what each button, input field, or selection does.</p>
</li>
<li>
<p><strong>Contextual Dialogue Boxes</strong><br>
Clear callouts offering best practices, warnings, or suggestions.</p>
</li>
<li>
<p><strong>Navigation Controls</strong><br>
You can always go <strong>Next</strong> or <strong>Back</strong> if needed. If you are stuck, use the <strong>Saleo navigation bar</strong> to jump to a specific point in the flow.</p>
</li>
</ul>
<hr>
<h3 id="getting-stuck">Getting Stuck?</h3>
<p>If at any point during the Saleo Tour:</p>
<ul>
<li>You close a window or refresh accidentally</li>
<li>The overlay disappears or doesn’t load</li>
<li>You lose your place in the sequence</li>
</ul>
<p>Use the <strong>Saleo navigation bar</strong> to restart the tour or jump to a specific chapter. You can also reload the page and the guide will resume where you left off.</p>
<hr>
<h3 id="access-the-guided-tour">Access the Guided Tour</h3>
<p>👉 <a href="https://tour-viewer.platform.saleo.io/f323a698-aac2-49b4-b9f3-b30dac1d29dc">https://tour-viewer.platform.saleo.io/f323a698-aac2-49b4-b9f3-b30dac1d29dc</a></p>
<hr>
<h3 id="tip">Tip</h3>
<p>We recommend opening the guided tour in a <strong>maximized browser window</strong> to avoid clipping of overlays, especially during module connections and popup authentications.</p>
<hr>
<h2 id="customization-options">Customization Options</h2>
<p>The automation can be further tailored to suit your needs:</p>
<ul>
<li><strong>Subject Line Personalization</strong>: Add variables like <code>Company</code>, <code>Industry</code>, or <code>Location</code></li>
<li><strong>Message Templates</strong>: Use different email templates based on lead status</li>
<li><strong>Scheduling</strong>: Run the automation at a fixed time daily using Make’s scheduling module</li>
<li><strong>Multiple Sheets</strong>: Extend the logic to multiple Google Sheets or tabs within the same workbook</li>
</ul>
<hr>
<h2 id="troubleshooting-and-known-issues">Troubleshooting and Known Issues</h2>
<h3 id="error-“it-is-not-possible-to-use-restricted-scopes-with-customer-gmail.com-accounts”">Error: “It is not possible to use restricted scopes with customer @gmail.com accounts”</h3>
<p>This error occurs when you try to authorize a Gmail module using a personal Gmail account with restricted API scopes.</p>
<p><strong>Solution</strong>:<br>
You need to create a custom OAuth app and enable the appropriate scopes for your Google project.</p>
<p><strong>Watch:</strong> <a href="https://youtu.be/yIr2IDM5yPY?si=Lml9KuxDwILto3CY">How to Fix Restricted Gmail Scopes in Make.com (YouTube)</a><br>
This video provides a step-by-step solution including setting up your own Google Cloud project, configuring OAuth consent, and enabling Gmail API scopes correctly.</p>
<h3 id="other-common-issues">Other Common Issues</h3>
<ul>
<li><strong>Modules Not Returning Data</strong>: Make sure your sheet has data and headers. Test individual modules by right-clicking and selecting “Run this module only”.</li>
<li><strong>Missing Mapping Options</strong>: Run the preceding module first to populate dynamic fields.</li>
<li><strong>Emails Not Sending</strong>: Check Gmail connection and verify you are not exceeding sending limits.</li>
<li><strong>No Auto-Save</strong>: Always press the Save button in <a href="http://Make.com">Make.com</a> — there is no auto-save.</li>
</ul>
<hr>
<h2 id="frequently-asked-questions">Frequently Asked Questions</h2>
<p><strong>Q: Can I use this with a company Gmail (Google Workspace)?</strong><br>
A: Yes. Google Workspace accounts fully support <a href="http://Make.com">Make.com</a> modules with no restricted scopes.</p>
<p><strong>Q: Can I use this with a free Gmail account (@gmail.com)?</strong><br>
A: You can, but some restricted scopes (like <code>send email</code>) may be blocked. See the <a href="#troubleshooting-and-known-issues">troubleshooting section</a> for a workaround using a custom OAuth app.</p>
<p><strong>Q: Can I customize the email for different lead types?</strong><br>
A: Absolutely. Add conditional logic or filters to send different templates based on columns like <code>Lead Type</code> or <code>Status</code>.</p>
<p><strong>Q: What happens if Make fails to send an email?</strong><br>
A: You can create an error route that logs failures to a secondary Google Sheet for review.</p>
<p><strong>Q: Is there a sending limit with Gmail?</strong><br>
A: Yes. Free Gmail accounts have a daily send limit (100/day), while Workspace accounts allow more. Use the Sleep module to avoid rapid fire sending.</p>
<p><strong>Q: Does <a href="http://Make.com">Make.com</a> auto-save my scenario?</strong><br>
A: No. Always click <strong>Save</strong> manually after editing.</p>
<hr>
<h2 id="support">Support</h2>
<ul>
<li><a href="https://www.make.com/en/help">Make Help Center</a></li>
<li><a href="https://support.google.com">Google Support</a></li>
<li>Make Community Forums for use-case discussions</li>
</ul>
<hr>
<h2 id="glossary">Glossary</h2>

<table>
<thead>
<tr>
<th>Term</th>
<th>Definition</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="http://Make.com">Make.com</a></td>
<td>A no-code automation platform used to connect apps and automate workflows</td>
</tr>
<tr>
<td>Scenario</td>
<td>A <a href="http://Make.com">Make.com</a> workflow consisting of modules linked in a logical flow</td>
</tr>
<tr>
<td>Module</td>
<td>An action or trigger in a Make scenario (e.g., send email, update sheet)</td>
</tr>
<tr>
<td>OAuth</td>
<td>Secure authorization protocol used to connect Make to Google services</td>
</tr>
<tr>
<td>Sleep Module</td>
<td>A delay tool in Make to pause actions for a set time</td>
</tr>
</tbody>
</table><hr>
<h2 id="legal-notice">Legal Notice</h2>
<p>All product names, logos, and trademarks are property of their respective owners. This documentation is provided for educational and instructional use only.</p>
<hr>
<h2 id="copyright">Copyright</h2>
<p>© 2025 ALL-Jordan<br>
You are permitted to use, modify, and distribute this guide for educational or business purposes, provided attribution is included.</p>

