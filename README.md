# Grill Me

`grill-me` is an open-source Codex skill that prevents premature project execution.

It asks focused, adaptive questions, converts the answers into a concrete project brief, and waits for explicit approval before beginning any implementation or external action.

## What it does

- Asks one to three high-leverage questions at a time.
- Uses read-only inspection to make questions more informed.
- Avoids asking for information that is already known or immaterial.
- Proposes sensible defaults when the user is unsure.
- Produces a compact confirmation brief.
- Opens the execution gate only after explicit approval.
- Reopens the gate when a material scope change appears.

## Install

Clone or copy this repository into your Codex skills directory:

```bash
git clone https://github.com/Anni1996/grill-me.git ~/.codex/skills/grill-me
```

Restart Codex if the skill does not appear immediately.

## Use

Invoke it explicitly:

```text
Use $grill-me for this project. I want to launch a landing page for my new service.
```

It can also be selected automatically when you ask Codex to question you and confirm requirements before starting work.

## Design principle

The skill treats the initial request as the beginning of discovery, not approval of a final brief. It permits read-only research before confirmation, but blocks deliverable creation and state-changing actions until the user explicitly approves the summarized agreement.

## Contributing

Issues and pull requests are welcome. Please keep changes focused on decision quality, scope clarity, and a crisp confirmation gate rather than adding generic project-management ceremony.

## License

[MIT](LICENSE)
