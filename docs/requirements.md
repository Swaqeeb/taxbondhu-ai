# TaxBondhu AI — Product Requirements

Created: 11 October 2026 | Project Day 1
Status: Planning; tax rules and calculations await validation.

## Purpose
Help ordinary Bangladeshi taxpayers prepare understandable,
reliable, and affordable personal income tax returns.

## Initial Scope
- Assessment Year: 2026–27
- Income Year: 2025–26
- First synthetic test case: salaried taxpayer with one employer
- Screen for other income and relevant filing obligations
- Flag unsupported situations instead of producing an incomplete return

## User Experience
- Bangla and English
- Simple questions, one at a time
- Relevant follow-up questions and document requests
- Mobile-friendly, accessible interface
- Progress indicator and save-and-resume
- Remember confirmed information and allow corrections
- Explain unfamiliar terms and why information is needed
- Never treat an unanswered question as “No” or zero

## Documents and Verification
- Use synthetic documents during initial development
- Extract values and preserve references to their source
- Require confirmation before extracted values enter calculations
- Flag missing, uncertain, duplicate, or conflicting information
- Request additional evidence only when relevant

## Tax Calculations
- Use verified official NBR rules for the selected assessment year
- Maintain a deterministic, version-controlled Python rule engine
- Calculate supported liabilities, deductions, rebates, and credits
- Verify eligibility; never assume an exemption applies
- Use Decimal for money and verified rounding rules
- Trace every result to confirmed inputs and rule sources

## Accuracy Controls
- Automated calculation, boundary, and regression tests
- Independently checked expected results
- Cross-check income, investments, payments, and declarations
- Comprehensive final audit
- Professional review for complex or ambiguous cases
- Aim for zero known calculation errors and zero unverified submissions
- Never guarantee an error-free return

## Return Preparation and Filing
- Prepare a reviewed summary mapped to official return fields
- Guide the user through the official NBR e-Return process
- Assisted online form filling remains a planned feature
- Verify NBR permission and technical feasibility before implementation
- Direct submission requires an authorized integration
- Approval to fill a form is separate from approval to submit
- Require explicit approval of the final return before submission
- Material changes invalidate earlier approval

## Privacy and Security
- Obtain consent for document processing and external AI services
- Protect sensitive data with encryption and access controls
- Implement authentication before multi-user access
- Define secure storage, retention, and document deletion
- Keep real financial records, identifiers, and secrets out of GitHub
- Avoid sensitive data in logs
- Treat uploaded document contents as untrusted input

## Development Phases
1. Personal prototype using synthetic data
2. Accuracy testing and independent professional validation
3. Private beta with consenting users
4. Public website
5. Android application
6. Expanded support for freelance, rental, and business income

## Learning and Portfolio
- Develop Python, SQL, AI, web, FinTech, and security skills
- Maintain documentation, test results, and milestones
- Track each session by project day and calendar date
- Explain each development step and wait for confirmation

## Open Dependencies
- Complete verification of AY 2026–27 rules and official forms
- Define supported salary components and document formats
- Arrange independent tax-professional validation
- Clarify NBR permission for third-party online form filling