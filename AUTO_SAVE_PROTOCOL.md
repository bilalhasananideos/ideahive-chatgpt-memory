# ChatGPT Memory — Mandatory Save and Handoff Protocol

## Source of truth
The local `chatgpt/` folder inside the IdeaHive Studio working directory is the primary working copy. This dedicated repository is a separate GitHub mirror for anonymous ChatGPT read access.

## After each meaningful completed task
1. Save research in the correct ChatGPT-specific file/folder.
2. Update `CURRENT_STATUS.md` with the date, completed work, unfinished work, exact next action and relevant paths.
3. Update `LATEST_HANDOFF.md` and create a dated handoff in `handoffs/` when a checkpoint or chat switch requires it.
4. Read the saved file back and verify the contents before saying it is saved.

## Keep these states separate
- **Local save:** verified only after the local file has been written and read back.
- **GitHub backup:** verified only after the intended commit is pushed and the remote branch/commit or raw file is checked.

A local save does not mean GitHub backup succeeded.

## No-login limitation
Anonymous access to a public GitHub repository is read-only. ChatGPT can read public raw files, but cannot commit or push anonymously. For write-back, either use an explicitly connected/authenticated GitHub integration or have the owner run the reviewed Git commands locally.

## Public-repository safety
Before the first push and every later addition, inspect staged files. Never publish passwords, tokens, API keys, cookies, browser profiles, identity documents, private financial/medical information, or confidential material the owner has not approved for public access.

## Verification wording
- Say `local save verified` only after read-back.
- Say `GitHub backup verified` only after confirming the remote commit/file.
- Otherwise say `draft prepared`, `staged locally`, or `not yet pushed` as appropriate.

## Handoff requirements
Every dated handoff must include: project objective, ChatGPT-only completed work, exact checkpoint, pending work, exact next action, relevant file paths, restrictions, local-save status and GitHub-backup status.
