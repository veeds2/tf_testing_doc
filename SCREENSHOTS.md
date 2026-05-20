# Screenshot Catalog

This file lists every screenshot referenced by the HR user guides. Drop the captured PNGs into the matching paths under `/images/<module>/` and they'll render automatically.

## How to capture

- **Format**: PNG preferred (JPG / GIF / WEBP also work)
- **Resolution**: capture at 2x (retina) so they look crisp on high-DPI displays. Mintlify auto-scales.
- **Width**: aim for ~1600px wide; anything smaller looks fuzzy
- **Crop**: tight to the relevant UI — don't include the browser chrome unless it's contextually important
- **Anonymize**: blur or replace any real customer names, emails, or PII before publishing
- **Dark/Light**: Mintlify supports both. If you want separate images, name them `<filename>-light.png` and `<filename>-dark.png` and update the MDX accordingly. Otherwise one neutral capture works fine.

## Master list (76 screenshots total)

### Workbooks (`/images/workbooks/`)

| Filename | What to capture |
|---|---|
| `01-project-overview.png` | Project Overview page with left-hand navigation showing Workbooks, Scenarios, Test Cases, etc. |
| `02-empty-workbooks.png` | Empty Workbooks tab with the central 'Upload Workbook' call-to-action |
| `03-upload-dialog.png` | Upload dialog with file selected and ready to upload, drag-and-drop area visible |
| `04-workbook-naming.png` | Upload dialog showing the Name field and the SF Module dropdown |
| `05-processing.png` | Workbook list with the new workbook in 'Processing…' state |
| `06-ready.png` | Workbook list with parsing complete: sheets/columns/questions count |
| `07-workbook-detail.png` | Workbook detail page with the Sheets tab open showing classified sheets |
| `08-iteration-filter.png` | Iteration filter chips at the top of a sheet: I1, I2, I3 with row counts |
| `09-deprecated-rows.png` | A sheet view with two rows shown in greyed-out, strikethrough style |
| `10-questions-tab.png` | Questions tab with multiple pending clarifications, priority-grouped |
| `11-clarification-card.png` | A single clarification card with recommendation, MC options, free-text fallback |
| `12-sheet-exclude.png` | Sheets list with Include/Exclude toggle visible on each row |
| `13-column-exclude.png` | Sheet view with column header menu open showing 'Exclude column' |
| `14-workbook-versions.png` | Workbook detail header with version dropdown (v1, v2 current, v3) |

### Scenarios & Categories (`/images/scenarios/`)

| Filename | What to capture |
|---|---|
| `01-scenarios-tab.png` | Scenarios tab with module groupings on left and category empty state on right |
| `02-empty-module.png` | Empty state for a module showing the central 'Generate Categories' CTA |
| `03-generating.png` | Module pane immediately after Generate click: 10 baseline categories + progress banner |
| `04-generated.png` | Module pane with ~28 categories total (baseline + AI), AI rows marked with badge |
| `05-category-actions.png` | Category row with action menu open: Edit, Demote, Link to cycles, Delete |
| `06-category-detail.png` | Category detail with scenarios and central 'Generate Scenarios' button |
| `07-refinement-chat.png` | Category detail with chat panel open and user refinement message |
| `08-refresh-menu.png` | Refresh dropdown showing 'Re-run AI suggestions' option |
| `09-link-to-cycles.png` | 'Link to cycles' picker showing project cycles selectable |

### Test Cases (`/images/test-cases/`)

| Filename | What to capture |
|---|---|
| `01-scenario-detail.png` | Scenario detail page with empty test cases section and 'Generate Test Cases' CTA |
| `02-generating.png` | Generation in progress with banner and first few proposed test cases appearing |
| `03-proposed-list.png` | Test cases list showing 12 proposed cases in 'Proposed' state |
| `04-test-case-detail.png` | Test case detail panel: steps, expected results, test data, AI rationale |
| `05-action-bar.png` | Test case action bar showing Approve, Edit, Reject buttons + feedback field |
| `06-bulk-approve.png` | Test cases list with 5 checkboxes ticked and 'Approve selected (5)' visible |
| `07-refinement-chat.png` | Chat panel open beside test cases list with AI's proposed changes |
| `08-edit-mode.png` | Test case in edit mode with all fields editable inline |

### Test Scripts (`/images/test-scripts/`)

| Filename | What to capture |
|---|---|
| `01-scripts-tab.png` | Test case detail with Scripts tab visible (empty on first open) |
| `02-generate-options.png` | Generate Script options panel: template, audience, detail level |
| `03-streaming.png` | Script being generated, streaming new steps in real time |
| `04-script-draft.png` | Completed script with 8 steps in Draft state, one step in inline-edit |
| `05-promote.png` | Script header showing Promote button and version dropdown |
| `06-template-editor.png` | Script template editor with pre-amble, step format, post-amble |

### Test Execution (`/images/test-execution/`)

| Filename | What to capture |
|---|---|
| `01-executions-tab.png` | Executions tab with 'My Executions' filter active showing assigned scripts |
| `02-execution-view.png` | Execution view opening on Step 1 of 8 with script header and step content |
| `03-step-detail.png` | A single execution step: action, test data table, expected result, status buttons |
| `04-attachments.png` | Step with two screenshots attached and a note about slow load time |
| `05-defect-form.png` | Defect form sliding in from right with auto-populated fields after Fail click |
| `06-mark-blocked.png` | Execution view at step 5 of 8 with 'Mark remaining as Blocked' option |
| `07-summary.png` | Execution summary screen with metric tiles and 'Move to next script' button |
| `08-dashboard.png` | Cycle Dashboard with progress charts, defect counts, tester velocity tiles |
| `09-new-execution.png` | Execution detail header with 'New Execution' button creating version 2 |

### Defects (`/images/defects/`)

| Filename | What to capture |
|---|---|
| `01-defects-tab.png` | Defects tab with filter bar and list color-coded by severity |
| `02-defect-detail.png` | Defect detail with header, reproduction steps, AI analysis, activity feed |
| `03-ai-analysis.png` | AI Analysis panel: root cause hypothesis, similar defects, workbook reference |
| `04-triage-controls.png` | Defect header with assignee dropdown showing team members + defect loads |
| `05-resolve.png` | Status change menu with Resolved option and auto-notify recipients |
| `06-verify-fix.png` | Resolved defect with 'Verify fix — re-run script' button prominent |
| `07-bulk-triage.png` | Bulk action confirmation dialog showing 12 defects about to be reassigned |
| `08-routing-rule.png` | Defect routing rule editor with condition builder and assignment fields |

### FactorBot (`/images/factorbot/`)

| Filename | What to capture |
|---|---|
| `01-bot-icon.png` | TestFactors page with FactorBot chat icon in bottom-right corner |
| `02-bot-open.png` | FactorBot side panel open showing chat input and welcome message |
| `03-typing.png` | Chat input with a question being typed |
| `04-answer.png` | FactorBot response with inline citations and a follow-up offer |
| `05-citation.png` | Citation click opening source test case in side-by-side view |
| `06-history.png` | FactorBot side panel with conversation history list on the left |

### Knowledge Wiki (`/images/knowledge-wiki/`)

| Filename | What to capture |
|---|---|
| `01-knowledge-home.png` | Knowledge tab home: recent pages, documents, 'Most cited facts' widget |
| `02-new-page.png` | Blank wiki page editor with title and content area |
| `03-page-editing.png` | Page editor with rich text formatting toolbar visible at top |
| `04-save-tags.png` | Save dialog with tag inputs: SF Module, Topic, Scope |
| `05-upload-docs.png` | Upload dialog with two PDFs in queue and a tag input |
| `06-open-questions.png` | Open Questions tab with 4 questions, each linking to the gap |
| `07-promote-rule.png` | Answer form with 'Apply as rule' checkbox and scope selector |
| `08-search.png` | Search results showing 3 wiki pages and 1 PDF matching a query |

### Memberships & Access (`/images/memberships/`)

| Filename | What to capture |
|---|---|
| `01-project-members.png` | Project Settings page with Members tab showing members + pending invitations |
| `02-add-member.png` | Add Member panel with email and role fields and Invite button |
| `03-invite-confirmation.png` | Confirmation toast: 'Member added' or 'Invitation sent' |
| `04-change-role.png` | Member row with role dropdown open showing all valid role options |
| `05-remove-member.png` | Member row with action menu open showing Remove option in red |
| `06-pending-invitations.png` | Pending invitations list with Resend/Revoke/Copy-link actions |
| `07-org-members.png` | Org Settings with Members tab showing org-scope memberships |
| `08-people-panel.png` | People panel showing one user's full access tree with assigned/unassigned scopes |

### Settings (`/images/settings/`)

| Filename | What to capture |
|---|---|
| `01-entry-points.png` | Project sidebar with the gear/Settings icon at bottom-left |
| `02-tabs.png` | Project Settings page with tab strip across the top |
| `03-autosave.png` | A settings field mid-edit with 'Saving…' spinner; another with 'Saved' checkmark |
| `04-inheritance.png` | Two fields side by side: one with 'Inherited from' badge, one with 'Set at this scope' |
| `05-logo-cropper.png` | Logo upload with cropper open allowing zoom, pan, rotation |
| `06-color-preset.png` | Color preset swatch grid with one selected and surrounding UI re-themed |
| `07-defect-routing.png` | Defect Routing tab with three rules listed and 'Add rule' button |

---

## Workflow recommendation

For a fast first pass, capture screenshots in this order:

1. **Quickstart pages** that new users hit first — just 3 screenshots (Workbooks empty state, Generate Categories CTA, Execution view) covers the most-viewed paths
2. **Workbooks + Scenarios + Test Execution** — these get the most traffic
3. **Defects + Test Cases + Memberships** — admin/triage workflows
4. **Settings + FactorBot + Knowledge Wiki + Test Scripts** — power users and reference

You don't have to capture all 76 at once. Mintlify renders missing images gracefully (shows a placeholder); pages still work without them.

## After dropping screenshots in

1. Commit them: `git add images/ && git commit -m "docs: add screenshots for <module>"`
2. Push: `git push`
3. Mintlify auto-deploys the new images within ~60 seconds
4. Spot-check the live site to confirm they render
