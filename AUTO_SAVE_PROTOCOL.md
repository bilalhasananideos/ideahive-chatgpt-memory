# ChatGPT Mandatory Proactive Auto-Save Protocol

## 1. Automatic trigger

The assistant must initiate this protocol after every meaningful completed task, without waiting for the user to say "save".

Meaningful work includes:
- Completed research or analysis.
- Important findings or evidence.
- Strategic conclusions and decisions.
- Completed deliverables.
- Changes to the project plan or workflow.

Minor conversation and temporary brainstorming do not automatically require permanent saving.

## 2. Assistant responsibilities

After meaningful work:

1. Identify what should be preserved.
2. Select the appropriate ChatGPT research file.
3. Prepare the complete updated content.
4. Update CURRENT_STATUS.md.
5. Record completed work, unfinished work and the exact next action.
6. Update or create a dated handoff when appropriate.
7. Provide exact Terminal commands for local saving.
8. Ask for command output and verify the saved content.

The assistant must initiate this process without being reminded.

## 3. Local saving

The original local ChatGPT memory is the primary working copy.

ChatGPT must not claim it has directly written to the user's Mac unless it actually has authorized filesystem write access.

When direct access is unavailable, it must provide complete file content and exact Terminal commands.

## 4. GitHub backup

GitHub backup is separate from local saving.

The assistant must:
- Review files before publication.
- Check for confidential information.
- Prepare exact Git commands.
- Ask for approval before publishing.
- Verify the remote commit after push.

Never claim a GitHub backup succeeded without verification.

## 5. Save states

Use these exact distinctions:

- Draft prepared: content written in the response.
- Local save pending: user has not executed the command.
- Local save verified: file was read back successfully.
- GitHub backup pending: local changes are not remotely confirmed.
- GitHub backup verified: remote commit/file has been confirmed.

## 6. Incomplete work

Never mark unfinished research as completed.

Record:
- Current progress.
- Missing evidence.
- Remaining tasks.
- Exact next action.

## 7. Chat switching

Before switching chats:
- Update CURRENT_STATUS.md.
- Create a dated handoff.
- Update the latest handoff pointer.
- Provide a continuation prompt.

END OF PROTOCOL
