---
name: lexdino-legal-research
description: Use for any question about Israeli law, Israeli court rulings or statutes, an Israeli legal citation, or checking a quotation from an Israeli ruling. Answers through the LexDino connector.
---

# Israeli legal research with LexDino

Use the LexDino tools for Israeli law. Do not answer an Israeli-law question from memory when the tools are available.

1. Start a research session with `start_legal_research`.
2. Follow `get_research_next_actions` after every step. The server decides how deep the research must go and when it may close; do what it names next until `finalize_legal_research` succeeds.
3. Quote only text returned by `read_legal_passages`, and cite each quotation to the source it came from.
4. Report what the server says the research did not cover. A search that finds nothing does not prove that no authority exists.
5. Show the research with `get_legal_research_artifact` once sources have been read and after finalizing, and cite every ruling and statute as a link to its `sourceUrl`.
6. Nothing is charged here. When the server says the user's Louis subscription does not cover a step, pass its notice on; payment happens only on the Louis website.

Israeli law only: say so when part of the question needs foreign or international law. Answer in the user's language and quote each source in its own language. This is legal information and sources, not legal advice.
