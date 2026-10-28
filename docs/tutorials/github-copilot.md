---
title: GitHub Copilot in VS Code
parent: Tutorials
nav_order: 1
description: "Get free Copilot Student access and start using Copilot in Visual Studio Code."
last_modified_date: 2026-10-28
---

# GitHub Copilot in VS Code
{: .no_toc }

GitHub Copilot is an AI coding assistant. In VS Code it suggests code as you type, answers questions about your code in chat, and can make multi-file changes as an agent. Verified students get the Copilot Student plan for free.
{: .fs-6 .fw-300 }

1. TOC
{:toc}

---

{: .important }
Check your course's AI policy before you use Copilot on graded work. Many programming courses restrict it. See [Using AI responsibly](../responsible-use.md).

## 1. Get Copilot Student

1. Create a free account at [github.com](https://github.com/signup) if you don't have one.
2. Go to [GitHub Education benefits](https://github.com/settings/education/benefits) and apply as a student. Verify with your Rutgers email or proof of enrollment, such as a student ID, transcript, or class schedule. Approval can take a few days.
3. Once you're approved, return to the same page. Under **Free GitHub developer resources for students and teachers**, click **Learn more**, choose **Copilot Student**, and follow the prompts.

If only paid plans appear, don't buy anything. GitHub's advice is to wait a few days and try again, then contact GitHub Support if it still doesn't work ([GitHub docs](https://docs.github.com/en/copilot/how-tos/copilot-on-github/set-up-copilot/enable-copilot/set-up-for-students)). GitHub rechecks student eligibility every month.

{: .note }
While you wait, you can use **Copilot Free**, which anyone with a GitHub account gets automatically. It has a monthly limit on suggestions and chat ([plans](https://docs.github.com/en/copilot/get-started/plans)).

## 2. Set up VS Code

1. Install or update [Visual Studio Code](https://code.visualstudio.com/). Copilot is built into current versions, so you don't need to install an extension.
2. Hover over the Copilot icon in the Status Bar at the bottom of the window and select **Use AI Features**.
3. Sign in with your GitHub account. You can also run **GitHub Copilot: Sign in** from the Command Palette (⇧⌘P on Mac, Ctrl+Shift+P on Windows/Linux).

If your account doesn't have Copilot Student or a paid plan yet, VS Code signs you up for Copilot Free ([setup guide](https://code.visualstudio.com/docs/setup/copilot)).

## 3. Inline suggestions

As you type, Copilot shows suggested code in gray text, called ghost text.

- Press **Tab** to accept a suggestion or **Esc** to dismiss it.
- To accept one word at a time, press **⌘→** on Mac or **Ctrl+→** on Windows/Linux.
- **Next edit suggestions** predict the next change you're likely to make, even somewhere else in the file. An arrow appears in the gutter. Press **Tab** to jump to the edit, then **Tab** again to accept it.

More detail: [Inline suggestions in VS Code](https://code.visualstudio.com/docs/editing/ai-powered-suggestions).

## 4. Chat and agents

Open the Chat view with **⌃⌘I** on Mac or **Ctrl+Alt+I** on Windows/Linux. Choose how Copilot should work from the agent picker in the chat box:

| Agent | Use it to | Changes your files? |
|:------|:----------|:--------------------|
| **Ask** | Understand code, errors, or concepts | No |
| **Plan** | Research a larger change and get a step-by-step plan first | No |
| **Agent** | Build a feature, fix a bug, or create a project. It edits files and can run terminal commands. | Yes, and you review each change |

Tips:

- Type `#` in the chat box to attach a file, a folder, or other context, or drag a file into chat.
- Slash commands: `/explain` explains selected code, `/fix` proposes a fix, `/tests` writes tests, and `/init` creates project instructions so Copilot follows your project's conventions.
- For a quick change to the code you're looking at, use **inline chat**: select code and press **⌘I** on Mac or **Ctrl+I** on Windows/Linux. Choose **Keep** to accept the change or **Undo** to reject it.
- On Copilot Student, the model is chosen automatically (**Auto**).

{: .note }
Older guides, including an earlier version of this page, describe a separate **Edit mode** and a completions panel. VS Code deprecated Edit mode in version 1.110 and is removing it. Use **Agent** for edits instead ([release notes](https://code.visualstudio.com/updates/v1_116)).

## Keyboard shortcuts

| Action | Mac | Windows/Linux |
|:-------|:----|:--------------|
| Open the Chat view | ⌃⌘I | Ctrl+Alt+I |
| Start a new chat | ⌘N (in the Chat view) | Ctrl+N (in the Chat view) |
| Inline chat in the editor or terminal | ⌘I | Ctrl+I |
| Accept an inline suggestion | Tab | Tab |
| Dismiss an inline suggestion | Esc | Esc |
| Next / previous inline suggestion | ⌥] / ⌥[ | Alt+] / Alt+[ |
| Trigger an inline suggestion | ⌥\ | Alt+\ |

Sources: [VS Code AI cheat sheet](https://code.visualstudio.com/docs/agents/reference/ai-features-cheat-sheet) and [GitHub's Copilot shortcuts](https://docs.github.com/en/copilot/reference/keyboard-shortcuts).

## Troubleshooting

- **No Copilot icon in the Status Bar:** update VS Code to the latest version.
- **Copilot Student isn't offered yet:** check your status on the [education benefits page](https://github.com/settings/education/benefits). Activation can take several days after approval.
- **Copilot stopped responding:** check [GitHub Status](https://www.githubstatus.com/) for outages.

## Learn more

- [Copilot in VS Code quickstart](https://code.visualstudio.com/docs/agents/quickstart)
- [GitHub Copilot documentation](https://docs.github.com/en/copilot)
