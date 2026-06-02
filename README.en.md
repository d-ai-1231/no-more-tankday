# no-more-tankday

### An AI skillpack that catches marketing disasters before they launch

> Campaigns are created with good intent. But the public decides what they mean.
> This skillpack helps you find the blind spots before the public does.

---

## What this is

This is **not** a content generation tool.

It is a **QA gate** that reviews marketing outputs against Korean cultural, historical, and social contexts before they go live. Think of it as a pre-flight checklist for Korean market campaigns.

---

## What it checks

- Campaign names
- Product names
- Launch dates and event dates
- Main and sub copy
- Hashtags
- Visual descriptions
- Storyboard flow
- **Combination risks** (date + name + copy together)

The real danger is rarely in a single word. It's in the combination.

---

## Risk levels

| Level | Meaning | Action |
|-------|---------|--------|
| **Low** | No issue found | Proceed |
| **Medium** | Possible misinterpretation | Revise recommended |
| **High** | Public backlash likely | Block launch until fixed |
| **Critical** | Boycott / media firestorm possible | Stop, escalate to PR/legal/execs |

---

## Real-time issue checking

**This skillpack does not fetch live data.**

If your agent has access to search tools, it can also check for today's news and trending issues.

| Tool | Notes |
|------|-------|
| Tavily API | Web + news, recommended |
| Brave Search API | 2,000 free queries/month |
| Generic web search | Naver News, Daum News, etc. |

Without search tools, only static (historical/cultural) risks are reviewed.

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
