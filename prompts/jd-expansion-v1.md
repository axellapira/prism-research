# JD Expansion Prompt v1

**Frozen** as of repository commit. Do not edit. New versions go in
`jd-expansion-v2.md`, etc.

**Model:** `claude-opus-4-7`
**Temperature:** 0
**System prompt:** none
**Tools:** none
**Max output tokens:** 600

The following user message is sent verbatim, with `{query}` substituted for
the PSB query string:

```
You will receive a short natural-language query that a recruiter typed into
a people-search tool. Your task is to expand the query into a realistic
1-paragraph job description that another recruiter would write for the role
the query is targeting.

Constraints:
- Output ONLY the job description paragraph. No preamble, no headers, no
  bullet points, no closing notes. One paragraph of plain prose.
- 4 to 7 sentences.
- Do NOT add hard requirements that were not in or strongly implied by the
  query. If the query says "5+ years," include 5+ years; if it does not
  specify experience, do not invent a number.
- Do NOT add a salary band, benefits, or company-marketing language. The
  paragraph should read as a job-posting description of duties and
  qualifications, not a recruiting pitch.
- Preserve every constraint mentioned in the query (location, seniority,
  skills, company type, education, etc.) exactly as expressed.
- Use neutral, professional tone. No exclamation marks, no "rockstar /
  ninja" framing, no superlatives.

Query:
{query}

Job description paragraph:
```
