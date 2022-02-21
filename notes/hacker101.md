# Hacker101

A [tutorial](https://www.hacker101.com/start-here) from HackerOne (They have an [Youtube channel](https://www.youtube.com/c/HackerOneTV)!)

## Mindset

- When assessing an application, find every bit of functionality you can. Once you have a rough list of all the bits of the application, consider this: if I was an attacker, what would my goal be?

- You will never find every bug, especially under time pressure, so you need to prioritize them - Just think about "What keeps you up at night?"

## Reporting

You should include these fields in your report in order to share your findings:

- Title (e.g. "Reflected Cross-Site Scripting in profiles")
- Severity (Here's a list of suggested levels of severity)
  - Informational - Issue has no real impact
  - Low - The business impact is minimal
  - Medium - Potential to cause harm to users, but not revealing data
  - High - Potential to reveal user data or aids in exploitation of other vulnerabilities
  - Critical - High risk of personal/confidential data exposure, general system compromise and other severe impact to the business
- Description: Brief description of what the vulnerability is
- Reproduction steps: Brief description of how to reproduce the bug; preferably with a small proof of concept
- Impact: What can be done with the vulnerability?
- Mitigation: How is it fixed?
- Affected assets: Generally a list of affected URLs
