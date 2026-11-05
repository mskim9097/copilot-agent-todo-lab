# TaskFlow – GitHub Copilot Cloud Agent Lab

A small browser-based starter application for a BCIT COMP 4976 hands-on lab on AI-assisted software development. TaskFlow uses HTML5, CSS3, vanilla JavaScript, and browser localStorage. No installation, dependencies, build tools, backend, or external resources are required.

## Learning objectives

- Fork a GitHub repository.
- Delegate debugging tasks to GitHub Copilot Cloud Agent.
- Write clear natural-language prompts.
- Review agent-generated code changes.
- Validate the modified application through manual testing.

## Running the application

1. Download the repository ZIP.
2. Extract it to a local folder.
3. Open `index.html` directly in Google Chrome or Microsoft Edge.
4. Add tasks using **Add Task** or Enter. Use each checkbox to mark a task completed or incomplete.

## Project files

```text
copilot-agent-todo-lab/
├── index.html
├── style.css
├── script.js
└── README.md
```

## Lab challenge

This starter contains two functional defects to correct:

- Completed status should persist after refreshing, along with task descriptions.
- Empty and whitespace-only tasks should be rejected.

Use GitHub Copilot Cloud Agent to investigate and correct these problems. Describe the expected behavior in your prompts, inspect the proposed changes, and test the application before accepting them.

## Manual testing checklist

Use a fresh browser profile or a new copy of the project in a different folder if you need an empty list. The application uses the localStorage key `taskflow-comp4976-tasks`.

- Open `index.html` directly and confirm the layout and empty state display correctly.
- Add “Review COMP 4976 notes” using the button, then add another description using Enter. Both appear immediately and the counter increases.
- Check and uncheck a task. Its checkbox and strikethrough styling should update together.
- Mark a task complete, then refresh. The task should remain completed. Repeat with multiple tasks.
- Submit an empty input, several spaces, and other whitespace pasted into the text field (for example, a tab). No blank row should be added and the counter should not increase.
- Enter text containing `<b>example</b>`. It should appear literally, without HTML formatting.
- Navigate with Tab, submit with Enter, and toggle a focused checkbox with Space. Check visible focus indicators.
- Resize to a narrow mobile viewport. Confirm the input, button, and long task descriptions fit without horizontal scrolling.
- Repeat in Chrome and Edge, including refreshing and reopening the file in the same browser profile.

## Browser storage notes

Tasks are saved in this browser profile, not synchronized between browsers or devices. Clearing browser data removes saved tasks; private browsing may remove them when the private session closes. Storage for `file://` URLs is browser-dependent. Moving or renaming the file or changing profiles may give it a different storage area. School-managed browser policies can also block localStorage. Keep the extracted project in the same location and test the actual classroom browser before the lab. If storage is unavailable, the app shows a message and remains usable for the current session.

No repository publication or account connection is required to run TaskFlow locally.
