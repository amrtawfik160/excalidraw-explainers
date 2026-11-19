---
name: "excalidraw-explainers"
description: "Create, revise, or review editable Excalidraw visuals that explain a topic to a first-time reader. Use for Excalidraw flowcharts, before-and-after comparisons, decision trees, timelines, system diagrams, data charts, and visual walkthroughs."
---

# Excalidraw explainers

Make the board understandable without a narrator. Include everything the intended reader needs to answer their question, and nothing that does not help them answer it.

## 1. Decide what the reader needs to understand

- Write one sentence for yourself: “After seeing this, [audience] can explain [question] in their own words.” Use their terms and assume no project history unless the brief says otherwise. Use their own scenario or feedback when available.
- Check the source for the facts that make the story work: starting situation, actors, order, exact rule or failure, result, and exceptions that change the result. For a change, verify both the baseline and what the new version actually does. Separate what exists today, what is implemented but not connected, and what is proposed or unknown.
- Keep a detail on the main path if removing it changes the reader’s answer, gives them the wrong expectation, or leaves a jump they cannot explain. Put useful supporting detail in a nearby note, linked source, or second panel. Leave out adjacent workflows, internal names, duplicate labels, and edge cases that do not change the answer.

Ready to draw when you can state the answer plainly, trace each essential claim to evidence, and name any assumption or gap that changes the takeaway.

## 2. Choose the structure that answers the question

| Reader’s question | Default layout | Include |
| --- | --- | --- |
| What was the problem and what fixes it? | Aligned **Before / After** flows | Start both with the same real scenario. Highlight the first step that differs. End each with its practical consequence. |
| How does it work, and what do I do? | Flowchart or swimlanes | Trigger, actor + action, any handoff or wait, and outcome. Use swimlanes only if who does what would otherwise be unclear. |
| What happens if I choose X? | Decision tree | Put the actual question at the split. Label each branch with the answer or condition and show where it ends. |
| What connects to what? | System or concept diagram | Keep only the parts that explain the story. Label arrows with what moves or what one part does to another. If order matters, number the path. |
| What happened when? | Timeline | Label dates or relative order, mark the turning point, and specify whether timing is exact or approximate. |
| How much, compared to what? | Bar for comparisons; line for change over time; labeled values for one or two numbers | Show units, timeframe, and the basis for comparison (denominator or source if relevant). Use zero-based bars and consistent scales for comparisons. Mark estimates and missing values rather than turning them into zeroes. |

Give each panel a title that states its point or asks the question it answers. Split independent stories into panels instead of shrinking everything to fit.

## 3. Write what happens, not what it’s called

- Use one concrete scenario from start to finish. Include timing or state when it changes the answer: “during the chat,” “before sending,” or “after payment clears,” not just “add member,” “review,” or “process.”
- Name the actor and action wherever they could be mistaken. Use the same names and terms throughout. Give each box one job. Put the extra sentence below the box if it explains the consequence rather than the action.
- Turn abstract steps into something the reader can see or do. If a person reviews, show what they see, what they can click, and what changes for each choice. If the screen is illustrative, label it “Example” or “Mockup,” and put any missing integration next to the affected step. Do not imply that an approval means an action already happened.
- Keep the timing, reason, and effect that explain the difference. If a reader is confused by a step, find the missing trigger, actor, evidence, rule, choice, or consequence. Redraw that part; swapping in shorter synonyms is not enough.

**Worked examples**

- **Chat:** “Change members” hides the problem. **Before:** Already chatting with Alice → try to add Sam during the chat → can’t add him here; start a new group chat. **After:** Already chatting with Alice → add Sam during the chat → Sam joins the same chat; earlier messages stay.
- **Email:** “Approve the workflow → review the action” mixes an unrelated process with an unclear instruction. **Before:** Ask Alice to email Jordan → Alice drafts it → no separate “Send this exact email?” prompt. **Proposed:** Alice drafts it and waits → show a mock card with **To**, **Subject**, **Message**, **Approve once**, and **Deny** → approval permits sending; denial leaves it unsent. If the API is ready but the card and pause are not, say so on the board.
- **Non-software:** For two pickup options, draw **Order ready → how will you collect it?** with **Walk in → show your order number at the counter** and **Curbside → text your parking spot and wait in the car**. Add hours only if they change which option someone can use. For real instructions, verify both routes first.

## 4. Build an editable board

- Discover Excalidraw MCP tools with tool search; use the exposed canvas or editor to work with native text, shapes, and connectors. If the target is an existing board, inspect it first, update only the requested section, and verify unrelated content stayed intact. Avoid replacing the whole scene to change one panel.
- Set one reading direction per panel. Line up equivalent steps, use clear spacing, and route connectors without crossings where possible. Reserve color for meaning, pair it with text so it is not the only cue, and make the changed step or key result easiest to find. Use normal-size text, not footnote-size labels for essential facts.
- Keep the visual editable. Use a screenshot only as a preview, not as the board. If live editing is unavailable, produce a valid native `.excalidraw` file, verify it renders in Excalidraw or with a compatible renderer, and say the live board was not changed.

## 5. Test with the board alone, then hand it off

Read the render as if you just opened it and cannot see your notes. Fix it before delivery unless all of these pass:

- **Glance:** The title and first visible path tell the reader where to start and what question the board answers.
- **Walkthrough:** Follow every meaningful path. You can say who acts, when, what they see or choose, and what happens at the end. For a comparison, you can point to the exact step that changed and why it matters. For a chart, you can tell what each plotted value means and how it can be compared.
- **Grounding:** Every factual arrow, branch, number, and status matches the source. A reader can distinguish the live behavior from a draft, a mockup, or an unverified step without opening the source.
- **Readability:** Inspect the actual render at the intended viewing size. No clipped text, ambiguous arrows, overlapping elements, or critical notes that only make sense with the spoken explanation. Remove boxes and text that do not help answer the question.
- **Delivery:** Confirm the saved scene contains the expected editable elements. Link the verified board when available and provide an editable `.excalidraw` export. In the handoff, state the main takeaway and any important limitation without repeating the entire diagram.
