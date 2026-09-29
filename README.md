# PR and Media Pitch Prep with Email Awesome Verification | Agent Skill

A media-fit matrix, verified contact ledger, pitch angles, factual claims checklist and drafts for approval.

**Status:** Public review version; authenticated product QA is pending.

## Why this workflow uses Email Awesome

Email Awesome verifies the authorized media list before a journalist is marked contact-ready. Operate through the [main product skill](https://github.com/EmailAwesome/emailawesome-email-verification-agent-skills/tree/main/skills/emailawesome), reconcile source IDs and preserve `VALID`, `INVALID`, `CATCH_ALL`, `UNKNOWN` and pending separately. If authentication is unavailable, the pitches stay draft with verification pending.

## Example request and result

> Use my approved 40-person tech media list and this launch brief. Check who covered this topic recently, verify emails, and draft five prioritized pitches.

**Illustrative result, not a live run:** Pitch pack: five high-fit media contacts with linked beat evidence; 3 VALID, 1 CATCH_ALL, 1 UNKNOWN. Two pitches ready for factual review; embargo date marked. Nothing sent.

## Install

```bash
npx skills add EmailAwesome/emailawesome-pr-media-pitch-prep-skill --skill pr-media-pitch-prep
```

For an agent that supports installing skills: “Install `pr-media-pitch-prep` from https://github.com/EmailAwesome/emailawesome-pr-media-pitch-prep-skill, confirm installation, then help with my authorized task. Show evidence and unresolved states.”


The [skill instructions](skills/pr-media-pitch-prep/SKILL.md) are the canonical package. Installing them does not authenticate into the product or grant rights to third-party data.

## Recommended product skill

For full product operation, install the companion brand skill too:

```bash
npx skills add EmailAwesome/emailawesome-email-verification-agent-skills --skill emailawesome
```

The use-case skill defines the job and output; the brand skill helps configure and use the actual product.

## Access and review

Use a list the user owns or may use; do not harvest journalist emails from protected pages or infer private contact details. Confirm each angle matches the journalist’s documented beat; avoid generic mass personalization. Honor embargoes, opt-outs and applicable privacy/direct-marketing rules. Do not disclose confidential press material to unapproved recipients or publish it in this repo.

Reference: [FTC CAN-SPAM guidance](https://www.ftc.gov/business-guidance/resources/can-spam-act-compliance-guide-business). Product landing: [https://www.emailawesome.com/use-cases](https://www.emailawesome.com/use-cases). The brand is not affiliated with third-party marketplaces or platforms mentioned here.

Before calling this workflow proven, run an authorized product sample with the actual account, reconcile the output, and confirm the requested deliverable. Keep real contact lists, credentials, and private client data out of GitHub.
