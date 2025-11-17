---
id: getting-started
title: Quick Start Guide
description: Get Velu AI connected to your documentation repository, ingest key context sources, and ship your first automated documentation update.
sidebar_label: Quick Start
---

This guide helps new teams bring Velu AI online and publish their first AI-assisted documentation update. It draws on the Velu AI Product Requirements Document (v1.0, updated November 14, 2026) and the current onboarding flow.

## 1. Prerequisites

- **Velu AI account:** Confirm you have an invitation or sign-up access for your organization.
- **GitHub account:** Required to authenticate Velu AI against the documentation repository Velu will update.
- **Connector credentials:** Ensure you can authorize Velu AI to read from your primary context sources (e.g., Google Drive, Slack, Linear, Confluence, Notion).
- **Governance owner:** Identify who will approve the first set of AI-proposed documentation changes.

## 2. Sign up and launch onboarding

1. Register or log in with your Velu AI credentials.
2. Complete the guided onboarding wizard. During this flow you will:
   - **Provision the GitHub integration** to connect the documentation repository that Velu AI will update via pull requests.
   - **Select context sources** such as Google Drive so Velu can ingest specs, release notes, meeting summaries, and other artifacts referenced in the PRD.
3. Confirm role-based access defaults so reviewers are ready to approve proposed updates.

## 3. Connect core context sources

After the initial wizard, add or verify the ingestion feeds that fuel Velu AI’s "documentation brain":

- **Slack**: Capture feature discussions, support escalations, and feedback threads.
- **Linear or Jira**: Pull product spec changes and release tickets marked as P1 in the PRD.
- **Confluence, Notion, or other doc hubs**: Sync existing knowledge bases so Velu can detect stale content.
- **Google Drive**: Index shared docs, slide decks, and transcripts that inform product knowledge.

These connectors help Velu AI reach the automation targets defined in the PRD (e.g., <5 % stale docs, 70% automation coverage, 24-hour update latency).

## 4. Configure documentation publishing

1. From **Settings → Publishing**, confirm the GitHub repository Velu AI linked during onboarding.
2. Choose whether Velu should create pull requests on a staging branch or directly against your main documentation branch.
3. Set your approval policy (e.g., require technical writer sign-off until AI confidence levels rise).

Velu AI tracks diffs and edit history so you can review, roll back, or audit changes as needed.

## 5. Prime Velu AI with context

- Run an initial synchronization to build the context graph from the connected sources.
- Review the dashboard for any high-confidence stale content alerts. Use these to validate Velu’s understanding before the first publish.

## 6. Draft your first article with Velu AI

1. In Slack, invoke `/velu update docs` or open the “Ask Velu” chat inside the app.
2. Prompt Velu AI to **write a new article or update an existing guide**. Velu will automatically search the connected context sources (e.g., PRDs, tickets, Drive docs) to ground the draft.
3. Inspect the proposed content for accuracy, tone, and adherence to your style rules.

## 7. Review and publish via pull request

1. When satisfied, approve the suggested update. Velu AI will create a GitHub pull request against the configured documentation repository.
2. Review the diff, add comments if adjustments are needed, and merge once approved.
3. Track post-merge metrics: automation coverage, freshness of key docs, and help-center task coverage.

## 8. What’s next?

- Expand ingestion to additional sources (Zendesk, video transcripts) to improve coverage.
- Calibrate governance controls (confidence thresholds, audit logs) in preparation for higher automation.
- Explore roadmap features such as the Chrome capture extension and personalized documentation experiences planned for later phases.

By following this quick start sequence, teams can move from signup to a merged, AI-authored documentation update while honoring the risk mitigations and success metrics defined in the Velu AI PRD.
