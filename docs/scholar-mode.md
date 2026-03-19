# Scholar Mode

Scholar Mode is InSight's research and academic workflow assistant. It overlays AI intelligence on top of documents, books, and written materials the user is reading or writing.

## Visual Identity

- Color: Emerald green (`#10b981`)
- Corner brackets: Green-tinted
- Background: Deep green-black gradient

## Scenarios

### 1. Archival Scan
**Use case:** Reading primary source documents (e.g., 1923 Federal Reserve Bulletin)

- Left lens shows the document with gaze-highlighted passages
- Right lens surfaces:
  - **Document Context** — historical background on the source
  - **Idea Connection** — links the passage to the user's own prior writing
  - **Related Source** — suggests a secondary source with relevance score and citation

### 2. Quote Clip
**Use case:** Capturing quotations with automatic citation generation

- Left lens shows the source text (e.g., Rousseau's *Social Contract*)
- Gaze-highlighted passage is ready to clip
- Right lens surfaces:
  - **Clip & Cite panel** — shows the quote with formatted citation (MLA, APA, Chicago, Bluebook)
  - **Dwell / Clip button** — confirms the clip and syncs to citation library
  - **Idea Connection** — suggests where in the user's paper the quote belongs
  - **Citation Formats Ready** — all formats auto-generated

**Interaction:** Dwell on "Clip" button to confirm. Clipped quote highlights amber; a confirmation toast appears.

### 3. Idea Connect
**Use case:** Detecting argument conflicts and synthesis opportunities across sources

- Left lens shows the current reading (e.g., Locke's *Second Treatise*)
- Right lens surfaces:
  - **Conflict Detected** — flags tension between current source and prior citations in the user's paper
  - **Synthesis Suggestion** — recommends a bridging source (e.g., Berlin's "Two Concepts of Liberty")
  - **Argument Map** — summary of unsupported claims, source conflicts, and missing counterarguments

### 4. Write First
**Use case:** Drafting freely, with gap detection and source suggestions added afterward

- Left lens shows the user's in-progress draft with gap markers on unsupported claims
- Right lens surfaces:
  - **Gap 1 / Gap 2** — identifies each unsupported claim with a suggested source and match score
  - **Strengthen Argument** — proposes statistics or data points to ground the argument

## Queue System

Progress dots at the bottom of each lens track how many items are in the current action queue and which is active.
