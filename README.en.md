# no-more-tankday

**An AI agent skillpack for pre-launch marketing risk review in the Korean market.**

---

## What this is

This is **not** a content generation tool. It is a **QA gate** for marketing outputs.

It helps detect cultural, historical, social, linguistic, and real-time issue risks in marketing campaigns before they go live in Korea.

---

## What it checks

- Campaign names
- Product names
- Launch dates and event dates
- Main and sub copy
- Hashtags
- Visual descriptions
- Storyboard flow
- Combination risks (date + name + copy)
- Real-time social issues

---

## How it works

The skillpack uses structured rules to evaluate marketing inputs against known Korean historical dates, sensitive expressions, and cultural contexts.

It assigns a risk level:

| Level | Meaning |
|-------|---------|
| **Low** | No significant risk. Proceed. |
| **Medium** | Possible misinterpretation. Recommend revision. |
| **High** | Likely public backlash. Block launch until revised. |
| **Critical** | Boycott, media coverage, or community backlash likely. Stop and escalate. |

---

## Real-time issue checking

**This skillpack does not fetch live data.**

If your agent environment has access to search tools, real-time issue checking can be performed at the final approval stage.

### Supported search tools

| Tool | Purpose |
|------|---------|
| Tavily API | Web + news search (recommended) |
| Brave Search API | Web + news search, 2,000 free queries/month |
| Generic web search | Naver News, Daum News, etc. |

Without search tools, only static (historical/cultural) risks are reviewed.

---

## Installation

```bash
git clone https://github.com/d-ai-1231/no-more-tankday.git
cp -r no-more-tankday/skills/marketing-cultural-risk ./skills/
```

## Usage

Add the contents of `agents/final_qa_prompt.md` to your QA agent prompt.

See [integration_guide.md](docs/integration_guide.md) for detailed setup options.

---

## License

MIT
