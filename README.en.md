# no-more-tankday

### Catch marketing disasters before they launch

Campaigns are created with good intent.
The public decides what they mean.

This skillpack finds the dangerous combinations before the public does.

---

## What this is

Not a content generator. A **pre-launch QA gate** for Korean market campaigns.

It reviews campaign names, product names, launch dates, copy, visuals, hashtags, and storyboards against Korean cultural, historical, and social context. The real danger is rarely a single word — it's the combination.

---

## Risk levels

| Level | Meaning | Action |
|-------|---------|--------|
| **Low** | No issue | Proceed |
| **Medium** | Possible misread | Revise |
| **High** | Backlash likely | Block until fixed |
| **Critical** | Boycott / firestorm | Stop, escalate |

---

## Real-time issue checking

This skillpack does **not** fetch live data.

If your agent has search tools (Tavily, Brave Search, etc.), it can also check today's news and trending issues. Without them, only static historical/cultural risks are reviewed.

---

## Install (30 seconds)

```bash
git clone https://github.com/d-ai-1231/no-more-tankday.git
cp -r no-more-tankday/skills/marketing-cultural-risk ./skills/
```

## Use (copy-paste)

Add this file to your QA agent prompt:

```
agents/final_qa_prompt.md
```

See [integration_guide.md](docs/integration_guide.md) for three usage modes.

---

## License

MIT
