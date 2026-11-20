---
epoch: 1795073312812
mode: agent
backendId: claude
sessionId: "99dd62a8-92a2-4619-a0cc-9c628d003fe5"
topic: "can u make a theorem template like Law and Formula ?"
model: '{"baseModelId":"haiku","effort":"medium"}'
tags:
  - copilot-conversation
usage: '{"usedTokens":39713,"contextWindow":1000000,"inputTokens":2,"outputTokens":2,"cacheReadTokens":39330,"cacheWriteTokens":379,"updatedAt":1795073328684}'
---

**user**: can u make a theorem template like [[Law]] and [[Formula]] ?
<!-- copilot-message {"notes":["Templates/Law.md","Templates/Formula.md"]} -->
[Timestamp: 2026/11/19 12:58:32]

**ai**: I made a Theorem template at `Templates/Theorem.md`, modeled on [[Law]] and [[Formula]].

It has the same frontmatter layout (`date`, `course`, `tags: theorem`) and these sections:

- **Statement**: the theorem in words
- **Conditions**: the hypotheses it needs
- **Formal Statement**: a LaTeX math block, like the one in [[Formula]]
- **Proof Idea**
- **Examples**
- **Uses**
- **Related**

I picked these sections based on what a theorem note usually needs. If you want the proof section to be a full proof rather than an idea, or want a different set of headings, tell me and I'll change it.
<!-- copilot-message {"tools":["Read (read): Templates/Law.md","Read (read): Templates/Formula.md","Glob (read)","Write (edit): Templates/Theorem.md","Edit (edit): Templates/Theorem.md"]} -->
[Timestamp: 2026/11/19 12:58:32]