# PROVISIONAL PATENT APPLICATION

**Title:** ASYMMETRIC DUAL-LENS HEADS-UP DISPLAY SYSTEM WITH GAZE-DRIVEN AI RESPONSE SELECTION AND MODE-BASED CONTEXTUAL INTELLIGENCE

**Filing Type:** Provisional Application for Patent
**Applicant/Inventor:** Keith Walley, Emily Towns — InSight Technologies
**Date Prepared:** 2026-03-19
**Status:** DRAFT — For filing with USPTO under 35 U.S.C. § 111(b)

> *Note: This provisional application establishes a priority date. A corresponding non-provisional application must be filed within 12 months under 35 U.S.C. § 119(e) to claim benefit of this filing.*

---

## ABSTRACT

An augmented reality heads-up display (HUD) system comprising asymmetric dual-lens optics wherein a left lens presents a context-enriched view of the physical environment and a right lens presents an AI-generated intelligence panel. The system captures gaze direction and dwell duration via infrared eye tracking to enable hands-free, voice-optional interaction with AI-generated response cards queued in the right lens. A mode-based architecture routes environmental and document inputs through distinct AI inference pipelines — Scholar Mode for academic research workflows and Field Mode for physical-world assessment tasks — each generating structured response cards navigable by gaze dwell. The system further comprises a quote-clip-and-auto-citation subsystem, an idea-conflict detection subsystem, a write-first-source-later gap-filling subsystem, a vehicle identification subsystem, a property damage assessment subsystem, a style assessment subsystem, and a geospatial site-selection intelligence subsystem. Input is captured through a combination of infrared eye tracking, multi-microphone beamforming voice recognition, and optional physical remote input. Output is delivered through waveguide optics in the right lens and bone conduction audio.

---

## BACKGROUND OF THE INVENTION

### Field of the Invention

The present invention relates to augmented reality wearable computing devices, and more particularly to a dual-lens optical see-through HUD system that renders AI-generated contextual intelligence in response to gaze-based user interaction across domain-specific operational modes.

### Description of Related Art

Existing augmented reality head-mounted displays (HMDs) — including monocular clip-on units, symmetric binocular displays, and projected visor systems — have failed to deliver practical AI-augmented workflows for knowledge workers, field professionals, and researchers for several interconnected reasons.

**Symmetric lens waste.** Most commercial AR headsets present the same information plane to both eyes or treat both lenses as a single unified display surface. This symmetric architecture forces a tradeoff: either the overlay obscures the physical environment, or it is rendered too faint to be useful. No existing system assigns distinct, complementary roles to the two lenses based on their relationship to the user's attentional system.

**Absence of gaze as a primary input modality.** Existing systems treat gaze primarily as a cursor metaphor for pointing at static UI elements. No prior art system uses gaze dwell as a structured selection input for navigating a queue of AI-generated response cards tied to live contextual analysis of the user's environment or document.

**AI integration is post-hoc and generalized.** Where AI assistants have been integrated into wearable displays, they function as general-purpose chatbots invoked by voice command, returning undifferentiated text responses. No prior system routes environmental inputs through domain-specific AI inference pipelines that produce structured, prioritized, card-based output calibrated to the user's current operational mode.

**Knowledge worker workflows are unserved.** Existing AR systems are designed primarily for navigation, gaming, industrial maintenance, or telemedicine. No prior system provides an integrated workflow for academic researchers combining live document analysis, automatic citation generation, inter-source conflict detection, and retroactive source-gap identification in a wearable form factor.

**Field professional workflows are similarly unserved.** No prior system provides real-time vehicle identification, property damage flagging, style assessment, or geospatial site-selection intelligence via a wearable AR display operating from live visual input.

The present invention addresses all of the above deficiencies.

---

## SUMMARY OF THE INVENTION

The invention is an AI-augmented dual-lens HUD system and method characterized by:

1. An **asymmetric dual-lens optical architecture** in which a left lens presents an environmentally-grounded augmented view and a right lens presents an AI intelligence panel — physically, cognitively, and functionally distinct roles assigned to each eye.

2. A **gaze-driven dwell selection mechanism** in which infrared eye tracking captures gaze position and duration, and a progressive dwell ring animation provides visual confirmation of an impending selection, enabling fully hands-free navigation of AI response card queues.

3. A **mode-based AI routing architecture** in which the system operates in distinct intelligence modes — at minimum Scholar Mode and Field Mode — each activating a different AI inference pipeline, input sensor configuration, and right-lens card schema.

4. A **Scholar Mode subsystem** comprising: (a) real-time archival document context generation, (b) gaze-triggered quote clipping with automatic multi-format citation generation, (c) cross-source idea conflict detection with synthesis suggestion, and (d) write-first-source-later gap identification with retroactive citation recommendation.

5. A **Field Mode subsystem** comprising: (a) vehicle identification and intelligence retrieval via visual bounding-box detection, (b) physical damage flagging with insurance-grade severity assessment, (c) style assessment intelligence for retail and wardrobe contexts, and (d) geospatial neighborhood site-selection scoring.

6. A **right-lens card queue system** in which AI-generated response cards are ranked, stacked, and made individually selectable by gaze dwell, with queue position indicators rendered at the bottom of the right lens.

7. A **multimodal input pipeline** combining infrared eye tracking, beamforming microphone array voice recognition, and optional physical remote input, all fused into a single interaction event stream fed to the AI inference pipeline.

8. A **bone conduction audio output system** providing non-occlusive audio feedback confirming dwell selections, alerting to new card queue entries, and delivering voice responses from AI without blocking ambient environmental sound.

---

## DETAILED DESCRIPTION OF PREFERRED EMBODIMENTS

### I. System Architecture Overview

The InSight system comprises a wearable frame housing two distinct optical assemblies. The **left lens assembly** contains a waveguide panel configured to render minimal, environmentally-anchored overlays: bounding boxes, AR labels, gaze-focus highlights, and mode-indicator corners. The lens is designed to preserve the user's natural depth-of-field relationship with the physical world while adding context at the point of gaze.

The **right lens assembly** contains a higher-density waveguide panel configured to render the AI Intelligence Panel — a structured, scrollable stack of response cards generated by the system's AI inference engine. The right lens is the primary information surface of the system and is always subordinate to the left lens in terms of environmental grounding — it never presents raw environmental feed but always presents processed AI output.

A **central processing unit** (worn at or near the frame) handles sensor fusion, mode management, AI API communication, card rendering, and dwell event processing. The CPu communicates with cloud-based AI inference services over Wi-Fi 6 (802.11ax) and Bluetooth 5.3 for peripheral connectivity.

### II. Gaze Tracking and Dwell Selection

An **infrared eye tracking module** mounted on the interior of the frame projects IR light onto the corneal surface of each eye and captures the reflected pattern using dedicated IR image sensors. The resulting gaze vector is computed at a minimum rate of 60Hz, sufficient to distinguish fixation (sustained gaze on a single target) from saccade (rapid gaze movement between targets).

The system distinguishes three gaze states:
- **Saccade**: gaze velocity exceeds a threshold; no interaction triggered.
- **Fixation**: gaze velocity falls below threshold for a minimum dwell threshold (default: 800ms, user-configurable from 500ms to 1500ms); interaction preview triggered.
- **Confirmed Dwell**: fixation exceeds full dwell threshold; selection confirmed.

Upon entering fixation on an interactive element, a **dwell ring** is rendered around the fixation point in the appropriate lens. The dwell ring is a circular progress indicator — a stroke that sweeps from 0° to 360° over the dwell period — providing continuous visual feedback of selection progress. When the ring completes, the selection is confirmed and the ring disappears.

The dwell ring is rendered at sufficient opacity to be visible against both the physical environment (left lens) and the card panel (right lens) without obscuring the underlying content at fixation points.

A **gaze escape** mechansim allows the user to cancel a pending dwell by moving gaze off the target before the ring completes.

### III. Dual-Lens Asymmetric Display Architecture

#### Left Lens — World Intelligence Layer

The left lens renders information in three zones:
- **Corner Brackets**: Four corner-bracket overlays rendered at the periphery of the lens indicate the current active mode via color coding (Scholar Mode: green #10b981; Field Mode: orange #f97316). These serve as persistent, low-cognitive-load mode indicators.
- **Status Bar**: A centered, pill-shaped status bar at the upper portion of the left lens displays active system status (ACTIVE/STANDBY), current mode label, battery, and connectivity indicators.
- **Gaze Focus Highlights**: When the user fixates on text (Scholar Mode) or physical objects (Field Mode), the system renders a highlight underline or bounding box at the fixation target while gaze is sustained. This highlight confirms to the user that the system has registered the target and is processing it for AI inference.
- **AR Bounding Boxes (Field Mode)**: In Field Mode, the left lens renders labeled bounding boxes around detected objects (vehicles, damaged areas, retail items, buildings) with a primary label and status line.
- **Clip Confirmation Toast (Scholar Mode)**: Upon a confirmed Quote Clip dwell event, a toast notification appears at the lower center of the left lens confirming the clipped text and the citation format generated.

#### Right Lens — AI Intelligence Panel

The right lens renders the AI Intelligence Panel, which is organized as follows:
- **Panel Mode Label**: A small text label at the top of the panel indicates the current AI mode (e.g., "SCHOLAR ASSIST", "FIELD INTEL").
- **Card Stack**: AI response cards are stacked vertically with the highest-priority card at top. Each card contains a category tag (color-coded by card type), a primary text body, an optional citation or data line, and optional gaze-selectable action buttons.
- **Queue Dots**: At the bottom of the right lens, a row of small circular indicators represents the number and selection state of cards in the queue, analogous to a slide indicator. The current top card is indicated by a filled dot; remaining cards by outline dots.

Card types and their color coding:

| Card Type | Color | Use |
|---|---|---|
| Context / Document Analysis | Green (#10b981) | Scholar Mode — AI-generated document or passage context |
| Idea Connection / Conflict | Purple (#a78bfa) | Scholar Mode — inter-source relationships, conflicts |
| Citation / Quote | Amber (#f59e0b) | Scholar Mode — quote clip confirmation, citation formats |
| Source Discovery | Cyan (#06b6d4) | Scholar Mode — suggested related sources, gap fills |
| Vehicle Intelligence | Orange (#f97316) | Field Mode — vehicle scan results |
| Damage Assessment | Red (#ef4444) | Field Mode — damage detection and severity |
| Style Assessment | Purple (#a78bfa) | Field Mode — style and retail intelligence |
| Site Intelligence | Cyan (#06b6d4) | Field Mode — KC Field Intel / geospatial scoring |

### IV. Scholar Mode — Detailed Description

Scholar Mode is activated by the user via mode selection (tab, voice command, or physical remote). In Scholar Mode, the left lens renders a document or reading environment, and the right lens renders the Scholar Assist card panel.

Scholar Mode comprises four primary operational sub-modes:

#### IV.A — Archival Scan Sub-Mode

In Archival Scan, the system's optical input or camera feed captures text in the user's field of view (physical documents, screens, printed materials). As the user reads, the system tracks the gaze point and identifies the word, phrase, or sentence at fixation.

When the user's gaze dwells on a passage for the fixation threshold, the system sends the surrounding context window (the fixated passage plus adjacent sentences, up to a configurable token budget) to the AI inference pipeline. The pipeline returns:
- A **Document Context card** summarizing the meaning, historical context, or theoretical significance of the passage.
- An **Idea Connection card** if the passage relates to previously encountered material in the same session.
- A **Related Source card** if the AI identifies a bibliographic source likely to be relevant to the passage.

Cards are rendered in the right lens in ranked order. The user navigates cards by gaze dwell on individual cards or on the queue dots.

#### IV.B — Quote Clip and Auto-Citation Sub-Mode

In Quote Clip mode, the user fixates on a specific span of text. The system identifies the fixation target as a quotable passage. A dwell ring renders at the fixation point. Upon confirmed dwell, the system:

1. Clips the highlighted text span to a temporary quote buffer.
2. Identifies the source document (via OCR metadata, open-library lookup, or user-provided document tagging).
3. Constructs a formatted citation in all available citation styles (MLA, APA, Chicago, Bluebook).
4. Renders a **Citation Confirmation card** in the right lens showing the clipped text and all citation formats.
5. Renders a **Clip Confirmation toast** in the left lens confirming the clip action.

The clipped quote and citation are simultaneously pushed to the system's clip queue, accessible via a companion application on a connected device, and optionally appended to an active document in a paired writing application.

The Quote Clip subsystem is designed to support the academic "write first, source later" workflow (see IV.D) and to reduce the friction of manually constructing citations during reading and research.

#### IV.C — Idea Conflict Detection Sub-Mode

During an active research session, the system maintains a **session source graph** — a running record of authors, claims, and arguments encountered in documents or clipped quotes. When a new passage is analyzed, the AI inference pipeline compares the passage's core claim against the session source graph.

If a tension or direct contradiction is detected between the current passage and a previously encountered source, the system generates an **Idea Conflict card** in the right lens specifying:
- The nature of the tension (direct contradiction, definitional disagreement, methodological divergence, empirical conflict).
- The identity of the conflicting sources (Author A vs. Author B on claim X).
- A **Synthesis Suggestion card** proposing a scholarly bridge, acknowledgment, or resolution strategy with an associated suggested source.

The system further generates an **Argument Map card** summarizing the current state of the user's argument structure — unsupported claims, source conflicts, and missing counterarguments — rendered as a running inventory.

#### IV.D — Write First, Source Later Sub-Mode

In Write First mode, the system monitors the user's active document (via paired writing application or document camera feed). The system identifies **gap markers** — claims, assertions, or data references in the user's draft text that are not yet supported by a citation.

Gap markers are rendered as dashed underlines in the left-lens document view, color-coded in red to distinguish them from source-supported text.

For each gap marker, the system generates a **Source Discovery card** in the right lens recommending one or more specific bibliographic sources with match confidence scores. The user may confirm a source recommendation via gaze dwell, causing the system to append the formatted citation to the draft document at the appropriate location.

This subsystem inverts the conventional write-then-cite workflow, allowing the user to write freely and at speed without interrupting prose flow to locate citations, while ensuring all claims are eventually supported.

### V. Field Mode — Detailed Description

Field Mode routes live optical input through environmental AI inference pipelines optimized for physical-world assessment tasks. The left lens renders AR overlays anchored to detected objects, and the right lens renders Field Intel cards.

#### V.A — Vehicle Scan Sub-Mode

In Vehicle Scan, the system's camera continuously processes the optical field for vehicles. When a vehicle is detected, the system:

1. Renders an **AR Bounding Box** around the vehicle in the left lens with a "VEHICLE DETECTED" label and VIN scan status.
2. Resolves the vehicle's identity via VIN scan (if accessible) or visual classification (make, model, year, trim).
3. Queries a vehicle intelligence database for: manufacturer specifications, standard retail and wholesale pricing (book values), known recalls, common mechanical issues, and typical service needs for the detected year/model.
4. Renders a **Vehicle Intelligence card** in the right lens with all retrieved data fields.

This sub-mode is specifically designed for automotive sales and service contexts, enabling sales professionals to access comprehensive vehicle intelligence hands-free at the point of customer interaction.

#### V.B — Damage Flag Sub-Mode

In Damage Flag mode, the system processes optical input for physical damage indicators — surface deformation, discoloration, fracture patterns, and material discontinuities — on vehicles, structures, or other physical assets.

When damage is detected, the system:
1. Renders **AR Damage Overlays** in the left lens — labeled boxes or polygons at each damage site with severity and category labels (e.g., "PANEL DENT — MINOR", "STRUCTURAL DAMAGE — CRITICAL").
2. Generates a **Damage Assessment card** in the right lens providing: a damage category, estimated repair cost range, recommended repair method, and insurance-grade severity classification.

This sub-mode is designed for insurance adjusters, vehicle appraisers, property inspectors, and automotive service writers.

#### V.C — Style Assessment Sub-Mode

In Style Assist, the system analyzes visual input for clothing, accessories, and retail merchandise. When a style-relevant item is detected, the system generates a **Style Assessment card** in the right lens providing: item identification, brand and product information where identifiable, style category, complementary item suggestions, and retail pricing context.

This sub-mode is designed for retail sales professionals, personal stylists, and consumers making purchasing decisions.

#### V.D — Geospatial Site Intelligence Sub-Mode (KC Field Intel)

In KC Field Intel mode, the system fuses GPS location data, neighborhood demographic data, commercial activity data, and AI analysis to generate a **Site Intelligence card** for the user's current location or a gaze-fixated location.

The Site Intelligence card provides: a composite site score (0–100), sub-scores by category (foot traffic, demographic match, competitive density, growth trajectory, infrastructure quality), and a recommendation summary.

This sub-mode is designed for entrepreneurs, real-estate professionals, franchise developers, and small business operators evaluating potential locations for commercial activity.

The initial implementation covers Kansas City metro neighborhoods with the following representative scores:

| Neighborhood | Overall Score | Notes |
|---|---|---|
| Waldo / Brookside | 87/100 | High foot traffic, strong demographic fit |
| Crossroads / Midtown | 79/100 | High creative density, moderate infrastructure |

The KC Field Intel system is designed for extensibility to any metropolitan area via data integration partnerships.

### VI. Multimodal Input Architecture

The system accepts input from three modalities, all fused into a unified interaction event stream:

**Infrared Eye Tracking**: As described in Section II. Primary interaction modality for dwell selection.

**Beamforming Microphone Array**: Four microphones are distributed across the frame to implement spatial beamforming, isolating the user's voice from ambient noise. Voice commands include: mode switching ("Scholar Mode", "Field Mode"), card navigation ("next card", "dismiss", "save"), clip actions ("clip that", "cite this"), and open-ended AI queries ("what does this mean", "how old is this vehicle"). Recognized voice commands are processed locally for latency-sensitive commands (mode switch, dismiss) and sent to the AI inference pipeline for open-ended queries.

**Physical Remote Input**: An optional paired Bluetooth remote provides single-button confirmation (dwell confirm), scroll (card advance/retreat), and mode-toggle inputs for environments where gaze interaction is insufficient — high-vibration settings, users with nystagmus, or preference situations.

### VII. AI Inference Pipeline

The system communicates with a cloud-based AI inference service (default: Claude API, Anthropic) over Wi-Fi 6. The inference pipeline operates as follows:

1. **Context capture**: The system assembles a context package from the current mode's relevant inputs — document text at gaze point (Scholar), visual classification result (Field), GPS coordinates (KC Field Intel), session source graph (Scholar Idea Conflict), or draft document gap markers (Write First).
2. **Mode-specific prompting**: The context package is wrapped in a mode-specific system prompt that instructs the AI to return structured card-format output appropriate to the current sub-mode.
3. **Response parsing**: AI output is parsed into card objects with type, tag, body, citation/data, and actions fields.
4. **Card queue update**: Parsed cards are inserted into the right-lens card queue, sorted by relevance score, and rendered.
5. **Session graph update**: For Scholar Mode, entity, claim, and source references extracted from AI responses are appended to the session source graph for use in subsequent Idea Conflict queries.

Latency targets: card response within 1.2 seconds of dwell confirmation for standard queries; 800ms for cached/local queries.

### VIII. Audio Feedback System

Bone conduction transducers mounted on the frame at the zygomatic arch transmit audio directly to the cochlea via skull vibration, bypassing the ear canal. This preserves the user's ability to hear ambient environmental audio — critical for field professionals, researchers in libraries, and users in conversation.

Audio feedback events include:
- **Dwell progress tone**: Subtle rising tone during dwell ring fill.
- **Selection confirm**: Short confirm tone on dwell completion.
- **New card alert**: Soft notification tone when new cards enter the queue.
- **Voice query confirm**: Tone confirming that a voice command has been captured.
- **AI voice response**: For open-ended queries, the AI's text response is optionally rendered as synthesized speech via the bone conduction transducer.

---

## CLAIMS

*Note: The following claims are informal claims appropriate for a provisional patent application. These claims will be formalized, expanded, and organized into independent and dependent claim sets in the corresponding non-provisional application.*

**Claim 1 — Asymmetric Dual-Lens Architecture**
A wearable heads-up display system comprising: a left lens optical assembly configured to render environmentally-anchored augmented reality overlays in the user's field of view of the physical environment; a right lens optical assembly configured to render an AI-generated intelligence panel comprising a plurality of structured response cards; and a processing system configured to maintain distinct rendering pipelines for the left and right lens assemblies, wherein the left lens assembly is configured to present context from the physical environment and the right lens assembly is configured to present AI-processed output distinct from the physical environment.

**Claim 2 — Gaze Dwell Selection**
The system of Claim 1, further comprising: an infrared eye tracking module configured to continuously detect the user's gaze direction and gaze dwell duration; a dwell ring rendering module configured to render a progressive circular completion indicator at the user's gaze fixation point upon detection of a fixation event; and a selection event generator configured to generate a selection confirmation event when the gaze dwell duration at a fixation point exceeds a configured dwell threshold.

**Claim 3 — Response Card Queue Navigation by Gaze**
The system of Claim 2, wherein the AI intelligence panel rendered in the right lens comprises a plurality of response cards arranged in a prioritized queue, and wherein the user navigates the queue by directing gaze fixation to individual cards and confirming selection via gaze dwell, without requiring manual input.

**Claim 4 — Queue Position Indicator**
The system of Claim 3, further comprising a queue position indicator rendered in the right lens comprising a row of dot elements, each dot representing one response card, wherein the current top card is represented by a filled dot and remaining cards are represented by outline dots.

**Claim 5 — Mode-Based AI Routing Architecture**
The system of Claim 1, further comprising a mode management module configured to operate the system in a plurality of distinct operational modes, each mode comprising: a distinct input sensor configuration; a distinct AI inference prompt schema; and a distinct response card rendering schema; wherein switching modes reconfigures all three of the foregoing without requiring system restart.

**Claim 6 — Scholar Mode: Quote Clip and Auto-Citation**
The system of Claim 5, wherein one operational mode is a Scholar Mode comprising: a gaze-triggered text detection module configured to identify a text span at the user's gaze fixation point in a document; a dwell-confirmation quote clip module configured, upon dwell confirmation, to capture the identified text span to a quote buffer; a citation generation module configured to generate formatted citations for the captured text span in one or more citation styles selected from the group comprising MLA, APA, Chicago, and Bluebook; and a citation card rendering module configured to render a Citation Confirmation card in the right lens displaying the captured text and generated citations.

**Claim 7 — Scholar Mode: Idea Conflict Detection**
The system of Claim 6, further comprising: a session source graph module configured to maintain a graph data structure representing authors, claims, and arguments encountered during the current session; a conflict detection module configured to compare each newly analyzed passage against the session source graph and identify logical tensions, contradictions, or methodological divergences; and a conflict card rendering module configured to render an Idea Conflict card in the right lens specifying the nature of the conflict and the identities of the conflicting sources when a conflict is detected.

**Claim 8 — Scholar Mode: Write First, Source Later**
The system of Claim 5, wherein the Scholar Mode further comprises: a gap detection module configured to identify unsupported claims, assertions, or data references in the user's active document draft; a gap marker rendering module configured to render a visual indicator at each identified gap in the document view in the left lens; and a source recommendation module configured to generate Source Discovery cards in the right lens for each identified gap, each Source Discovery card comprising one or more suggested bibliographic sources and a match confidence score.

**Claim 9 — Field Mode: Vehicle Identification and Intelligence Retrieval**
The system of Claim 5, wherein one operational mode is a Field Mode comprising: a vehicle detection module configured to identify vehicles in the user's field of view via the system's optical input; an AR bounding box rendering module configured to render a labeled bounding box around a detected vehicle in the left lens; a vehicle identification module configured to resolve the detected vehicle's make, model, year, and trim level via visual classification or VIN scan; and a vehicle intelligence retrieval module configured to retrieve and render a Vehicle Intelligence card in the right lens comprising vehicle specifications, pricing, recall status, and service data.

**Claim 10 — Field Mode: Damage Assessment**
The system of Claim 9, further comprising: a damage detection module configured to identify physical damage indicators in the user's field of view via the system's optical input; a damage overlay rendering module configured to render labeled damage overlays at detected damage sites in the left lens; and a damage assessment card module configured to generate a Damage Assessment card in the right lens comprising damage category, severity classification, estimated repair cost range, and recommended repair method.

**Claim 11 — Field Mode: Geospatial Site Intelligence**
The system of Claim 5, wherein the Field Mode further comprises: a geospatial data fusion module configured to combine GPS location data, demographic data, commercial activity data, and AI analysis for the user's current or gaze-indicated location; and a site intelligence card module configured to render a Site Intelligence card in the right lens comprising a composite site score and sub-scores by category.

**Claim 12 — Multimodal Input Fusion**
The system of Claim 1, further comprising: a beamforming microphone array comprising a plurality of microphones distributed across the wearable frame configured to isolate the user's voice from ambient noise; a voice recognition module configured to recognize voice commands and open-ended AI queries; and an input fusion module configured to combine eye tracking events, voice recognition events, and optional physical remote input events into a unified interaction event stream delivered to the AI inference pipeline.

**Claim 13 — Bone Conduction Audio Output**
The system of Claim 1, further comprising: one or more bone conduction transducers mounted on the wearable frame configured to transmit audio to the user via skull vibration without occluding the ear canal, preserving the user's ability to perceive ambient environmental sound while receiving system audio feedback and AI voice responses.

**Claim 14 — Clip Confirmation Toast Notification**
The system of Claim 6, further comprising a toast notification module configured to render a transient confirmation notification in the left lens upon completion of a quote clip event, the notification comprising the clipped text and a citation format confirmation, positioned at the lower center of the left lens field of view so as not to occlude the primary document view.

**Claim 15 — Mode Color-Coded Corner Bracket System**
The system of Claim 5, further comprising a corner bracket rendering module configured to render four corner-bracket overlay elements at the periphery of the left lens, wherein the color of the corner brackets changes to reflect the currently active operational mode, providing continuous low-cognitive-load mode state awareness without requiring the user to shift gaze from the primary view area.

---

## BRIEF DESCRIPTION OF DRAWINGS

*(Drawings to be prepared for non-provisional filing. The following describes the drawing set.)*

- **FIG. 1** — System architecture diagram showing left lens, right lens, CPU unit, IR eye tracking module, microphone array, and bone conduction transducers.
- **FIG. 2** — Left lens view in Scholar Mode — Archival Scan sub-mode, showing document text, gaze highlight, corner brackets, and status bar.
- **FIG. 3** — Right lens view in Scholar Mode — Archival Scan sub-mode, showing Document Context card, Idea Connection card, and Related Source card with queue dots.
- **FIG. 4** — Dwell ring sequence diagram showing four stages: fixation detected, dwell ring at 25%, dwell ring at 75%, selection confirmed (ring complete, dismissed).
- **FIG. 5** — Left lens view in Scholar Mode — Quote Clip sub-mode, showing gaze-highlighted text span and clip confirmation toast.
- **FIG. 6** — Right lens view in Scholar Mode — Quote Clip sub-mode, showing Citation Confirmation card with multi-format citation display.
- **FIG. 7** — Right lens view in Scholar Mode — Idea Conflict sub-mode, showing Conflict Detected card, Synthesis Suggestion card, and Argument Map card.
- **FIG. 8** — Left lens view in Scholar Mode — Write First sub-mode, showing draft document text with gap markers rendered as dashed underlines.
- **FIG. 9** — Right lens view in Scholar Mode — Write First sub-mode, showing two Source Discovery cards with match confidence scores.
- **FIG. 10** — Left lens view in Field Mode — Vehicle Scan sub-mode, showing AR bounding box with vehicle label.
- **FIG. 11** — Right lens view in Field Mode — Vehicle Scan sub-mode, showing Vehicle Intelligence card with all data fields.
- **FIG. 12** — Left lens view in Field Mode — Damage Flag sub-mode, showing AR damage overlays with severity labels.
- **FIG. 13** — Right lens view in Field Mode — Site Intelligence sub-mode, showing composite score and sub-score breakdown.
- **FIG. 14** — Multimodal input fusion flow diagram showing eye tracking, voice, and remote input streams converging into the unified interaction event stream and AI inference pipeline.
- **FIG. 15** — System state diagram showing mode states (Scholar, Field), sub-mode states, and transition triggers.

---

## INVENTOR DECLARATION PLACEHOLDER

*The following declaration will be completed and signed by all inventors prior to non-provisional filing:*

I hereby declare that:
- I believe I am the original inventor (or joint inventor) of the subject matter claimed in this application.
- I have reviewed and understand the contents of this application.
- I acknowledge my duty to disclose to the USPTO all information known to me to be material to patentability as defined in 37 C.F.R. § 1.56.

**Inventor 1:** Keith Walley — InSight Technologies — Kansas City, Missouri
**Inventor 2:** Emily Towns — InSight Technologies — Kansas City, Missouri

---

*End of Provisional Patent Application Draft*
*Prepared: 2026-03-19 | Version: 1.0 DRAFT*
*For attorney review prior to USPTO filing*
