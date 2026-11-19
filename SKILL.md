---
name: "excalidraw-explainers"
description: "Create, revise, or review editable Excalidraw explainers for a first-time reader. Use for visual journeys through complex processes or system changes, and for flowcharts, before-and-after comparisons, decision trees, timelines, and data charts."
---

# Excalidraw explainers

Make the board understandable without a narrator. Include everything the intended reader needs to answer their question, and nothing that does not help them answer it.

## 1. Decide what the reader needs to understand

- Write one sentence for yourself: “After seeing this, [audience] can explain [question] in their own words.” Use their terms and assume no project history unless the brief says otherwise. Use their own scenario or feedback when available.
- Check the source for the facts that make the story work: starting situation, actors, order, exact rule or failure, result, and exceptions that change the result. For a change, verify both the baseline and what the new version actually does. Separate what exists today, what is implemented but not connected, and what is proposed or unknown.
- Keep a detail on the main path if removing it changes the reader’s answer, gives them the wrong expectation, or leaves a jump they cannot explain. Put useful supporting detail in a nearby note, linked source, or second panel. Leave out adjacent workflows, internal names, duplicate labels, and edge cases that do not change the answer.

Ready to draw when you can state the answer plainly, trace each essential claim to evidence, and name any assumption or gap that changes the takeaway.

## 2. Choose the structure that answers the question

**Default to one visual journey for a complex explanation.** Use a journey when the reader needs to connect several steps, layers, or consequences. For a single decision, comparison, or takeaway, use the smallest diagram or chart that answers it.

1. Follow one named person, request, order, or job from the first recognizable event to the outcome. Lay out numbered stops along one reading path. Title each stop with what happens or the question the reader would ask next. Use clock times only when they matter; label invented times and values as illustrative.
2. At each stop, show what the person sees and the one behind-the-scenes action that explains it. Ask what must happen before the next stop. Draw the missing handoff, wait, decision, or failure path if omitting it would make the conclusion seem automatic. Introduce technical terms at the first moment the reader needs them.
3. Put each visual where it answers the next question: a flow for where the request goes, matched bars for what changes, a timeline or aligned small charts for when two things change at different times, or a cutaway for how parts fit. Use the same scenario, units, and time points across comparisons. Label the cause at the turning point, not only in the accompanying prose. Use categories or shared time markers for snapshots; don't imply continuous measurements you don't have.
4. End on the practical result and the assumption or tradeoff that could change it. Keep deeper implementation notes off the main path. If the reader says the board is hard to follow or has gaps, rebuild the reading path around their scenario before adding more text or more disconnected panels.

| Reader’s question | Default layout | Include |
| --- | --- | --- |
| What was the problem and what fixes it? | Aligned **Before / After** flows | Start both with the same real scenario. Highlight the first step that differs. End each with its practical consequence. |
| How does it work, and what do I do? | Flowchart or swimlanes | Trigger, actor + action, any handoff or wait, and outcome. Use swimlanes only if who does what would otherwise be unclear. |
| What happens if I choose X? | Decision tree | Put the actual question at the split. Label each branch with the answer or condition and show where it ends. |
| What connects to what? | System or concept diagram | Keep only the parts that explain the story. Label arrows with what moves or what one part does to another. If order matters, number the path. |
| What happened when? | Timeline | Label dates or relative order, mark the turning point, and specify whether timing is exact or approximate. |
| How much, compared to what? | Bar for comparisons; line for change over time; labeled values for one or two numbers | Show units, timeframe, and the basis for comparison (denominator or source if relevant). Use zero-based bars and consistent scales for comparisons. Mark estimates and missing values rather than turning them into zeroes. |

Keep stops in the same story visibly connected. Use separate panels for genuinely independent stories rather than shrinking everything to fit.

## 3. Write what happens, not what it’s called

- Use one concrete scenario from start to finish. Include timing or state when it changes the answer: “during the chat,” “before sending,” or “after payment clears,” not just “add member,” “review,” or “process.”
- Name the actor and action wherever they could be mistaken. Use the same names and terms throughout. Give each box one job. Put the extra sentence below the box if it explains the consequence rather than the action.
- Turn abstract steps into something the reader can see or do. If a person reviews, show what they see, what they can click, and what changes for each choice. If the screen is illustrative, label it “Example” or “Mockup,” and put any missing integration next to the affected step. Do not imply that an approval means an action already happened.
- Keep the timing, reason, and effect that explain the difference. If a reader is confused by a step, find the missing trigger, actor, evidence, rule, choice, or consequence. Redraw that part; swapping in shorter synonyms is not enough.

**Worked examples**

- **Chat:** “Change members” hides the problem. **Before:** Already chatting with Alice → try to add Sam during the chat → can’t add him here; start a new group chat. **After:** Already chatting with Alice → add Sam during the chat → Sam joins the same chat; earlier messages stay.
- **Email:** “Approve the workflow → review the action” mixes an unrelated process with an unclear instruction. **Before:** Ask Alice to email Jordan → Alice drafts it → no separate “Send this exact email?” prompt. **Proposed:** Alice drafts it and waits → show a mock card with **To**, **Subject**, **Message**, **Approve once**, and **Deny** → approval permits sending; denial leaves it unsent. If the API is ready but the card and pause are not, say so on the board.
- **Journey:** Follow Maya’s delivery from order placed → waits in the queue → driver picks it up → delivered → evening bill. At the quiet point, align two charts: orders waiting fall from 10 to 3, but rented vans stay at 2 until dispatch can return one. Label the return on the timeline: fewer orders do not lower the rental bill by themselves. Treat these as example counts, not measured traffic. Use the same pattern anywhere the user-visible change and its cost or capacity effect occur at different times.

## 4. Build an editable board

- Discover Excalidraw MCP tools with tool search; use the exposed canvas or editor to work with native text, shapes, and connectors. If the target is an existing board, inspect it first, update only the requested section, and verify unrelated content stayed intact. Avoid replacing the whole scene to change one panel.
- Set one reading direction per panel. Line up equivalent steps, use clear spacing, and route connectors without crossings where possible. Reserve color for meaning, pair it with text so it is not the only cue, and make the changed step or key result easiest to find. Use normal-size text, not footnote-size labels for essential facts.
- Keep the visual editable. Use a screenshot only as a preview, not as the board. If live editing is unavailable, produce a valid native `.excalidraw` file, verify it renders in Excalidraw or with a compatible renderer, and say the live board was not changed.

## 5. Test with the board alone, then hand it off

Read the render as if you just opened it and cannot see your notes. Fix it before delivery unless all of these pass:

- **Glance:** The title and first visible path tell the reader where to start and what question the board answers.
- **Walkthrough:** Follow every meaningful path. At each stop, you can answer “What just happened, what caused it, and what makes the next stop possible?” Point to the exact change in a comparison. For each chart, explain what the values measure and why they change at that point. If the answer is only in the chat reply, put it on the board.
- **Grounding:** Every factual arrow, branch, number, and status matches the source. A reader can distinguish the live behavior from a draft, a mockup, or an unverified step without opening the source.
- **Readability:** Inspect the actual render at the intended viewing size. No clipped text, ambiguous arrows, overlapping elements, or critical notes that only make sense with the spoken explanation. Remove boxes and text that do not help answer the question.
- **Delivery:** Confirm the saved scene contains the expected editable elements and opens at the start of the journey. Link the verified board when available and provide an editable `.excalidraw` export. Preview the key flow or turning-point chart in the handoff when useful, then give the takeaway and any important limitation without retelling the board.
