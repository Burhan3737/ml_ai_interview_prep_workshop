# Facilitator Guide: Mock Non-Coding Technical Interviews

Your private answer key. Do not share with students.

For mostly first- and second-year CS, AI and Data Science students. One student at a time, round robin, about 9 to 10 minutes each. No scores: you give verbal feedback only.

---

## 1. Contents

1. [Contents](#1-contents)
2. [The idea](#2-the-idea)
3. [Run sheet for one student](#3-run-sheet-for-one-student)
4. [How to play the interviewer](#4-how-to-play-the-interviewer)
5. [What to look for](#5-what-to-look-for)
6. [Feedback script](#6-feedback-script)
7. [Question cards](#7-question-cards): [Algorithms and data structures](#algorithms-and-data-structures-cards) · [Systems and software](#systems-and-software-cards) · [Data and databases](#data-and-databases-cards) · [AI and ML](#ai-and-ml-cards) · [Scenarios](#scenarios-cards) · [Your experience](#your-experience-cards)
8. [Tips for students](#8-tips-for-students)
9. [Feedback notes sheet](#9-feedback-notes-sheet)
10. [Sources](#10-sources)

**Question index** (36 questions: 6 tracks × 6, matching the 6 rows of the board)

- **Algorithms and data structures:** [A1 Undo and redo](#a1--undo-and-redo) · [A2 Live leaderboard](#a2--live-leaderboard) · [A3 Fastest route](#a3--fastest-route) · [A4 Search autocomplete](#a4--search-autocomplete) · [A5 Meeting rooms](#a5--meeting-rooms) · [A6 Duplicate files](#a6--duplicate-files)
- **Systems and software:** [S1 Chat app](#s1--chat-app) · [S2 8-second page load](#s2--8-second-page-load) · [S3 Ticket site crashes](#s3--ticket-site-crashes) · [S4 Simultaneous edits](#s4--simultaneous-edits) · [S5 URL shortener](#s5--url-shortener) · [S6 Parking garage](#s6--parking-garage)
- **Data and databases:** [D1 University database](#d1--university-database) · [D2 Sign-ups down 20%](#d2--sign-ups-down-20) · [D3 20 GB log, 8 GB RAM](#d3--20-gb-log-8-gb-ram) · [D4 Missing values](#d4--missing-values) · [D5 Messy merge](#d5--messy-merge) · [D6 SQL or NoSQL?](#d6--sql-or-nosql)
- **AI and ML:** [M1 Cats vs dogs](#m1--cats-vs-dogs) · [M2 Spam filter](#m2--spam-filter) · [M3 "99% accurate"](#m3--99-accurate) · [M4 Movies for new users](#m4--movies-for-new-users) · [M5 98% train, 60% new](#m5--98-train-60-new) · [M6 Handbook chatbot](#m6--handbook-chatbot)
- **Scenarios:** [SC1 Ship with a bug?](#sc1--ship-with-a-bug) · [SC2 No tests, no docs](#sc2--no-tests-no-docs) · [SC3 Broke the site](#sc3--broke-the-site) · [SC4 Won't make deadline](#sc4--wont-make-deadline) · [SC5 Rewrite it?](#sc5--rewrite-it) · [SC6 Unsafe passwords](#sc6--unsafe-passwords)
- **Your experience:** [E1 Hardest bug you fixed](#e1--hardest-bug-you-fixed) · [E2 A technical decision](#e2--a-technical-decision) · [E3 Hard to learn](#e3--hard-to-learn) · [E4 Code feedback](#e4--code-feedback) · [E5 Do it differently](#e5--do-it-differently) · [E6 Vague brief](#e6--vague-brief)

---

## 2. The idea

> "The technical interview is not only about whether you can solve the problem. It's about how you approach it and try to solve it."

That is the line on the mindset slide. It comes from your original words:

> "The technical interview is not about can you solve the problem they give to you, it is about how you approach & try to solve the problem. Ask clarifying questions, state your assumptions, talk aloud about different options. Listen to the interviewers, explain your decisions. Be curious, don't pretend to know things if you don't."

The slide turns this into five habits:

1. **Clarify the problem:** ask questions, then state and check your assumptions.
2. **Think out loud:** compare two or three options and their trade-offs.
3. **Explain your decisions:** say why you chose it; listen to what the interviewer tells you, and use it.
4. **Start simple, then improve and check it:** get a basic version, improve it, then test it against edge cases.
5. **Be honest about what you don't know:** say so, then reason from what you do know.

Every question is open and deliberately under-specified. Nobody is expected to have memorised anything, and there is no single right answer to find. What you are watching is the approach: does the student clarify before diving in, think out loud about more than one option, explain their choices and use what you tell them, get something simple working before improving and checking it, and stay honest about what they don't know. The hidden details on each card exist to reward students who ask. The optional change partway through exists to see whether they listen and adapt. A student who reasons out loud to a sensible answer beats one who gives a polished answer in silence, and your feedback should make that obvious to them. There are no scores; you give verbal feedback only.

---

## 3. Run sheet for one student

About 9 to 10 minutes. Have this guide, the printed [feedback notes sheet](#9-feedback-notes-sheet) and a pen ready.

**Before the first student:** go to the Question board slide and click **Clear used marks**. Marks are saved in the browser, so last session's greyed-out questions will still be there otherwise. The board shows all 36 questions in 6 rows, one track per row: Algorithms, Systems & software, Data & databases, AI & ML, Scenarios and Your experience. Greyed-out cards are already used; **Clear used marks** is the only reset. Pick a track filter if you want to limit the draw (there are no year levels).

**The flow:** briefing slides → draw → 1 minute to think → 3 minutes to answer out loud → feedback → next student.

### What to say on each slide (about 1.5 minutes in total)

The deck has 7 slides.

| Slide | Say |
|---|---|
| 1 · Welcome | "Hi, what's your name? This is a practice interview. One random problem, a minute to think, three minutes to talk me through it, then feedback." |
| 2 · Mindset | Read the quote, or say: "I'm not only checking whether you solve it. I'm watching how you approach it and try to solve it." |
| 3 · Five habits | "Clarify the problem, think out loud, explain your decisions, start simple then improve and check it, and be honest about what you don't know. That's the whole game." |
| 4 · How this works | "You get one minute to think, then three minutes to answer out loud. Ask me questions whenever you like. I'll answer them, but I won't give hints. I might change something halfway through. That's on purpose." |
| 5 · When you're stuck | "If you're stuck, say so and say what you'd try. 'I don't know, but I'd guess…' is a good answer. Bluffing isn't." |
| 6 · Question board | Let the student draw. Read the question aloud once. Click **Start**: the timer runs 1 minute of thinking time, then moves straight into 3 minutes of answer time. |
| 7 · Takeaways | Use at the end of feedback, then click **Next student** (clears the name, goes back to slide 1). |

### Running the interview

**Think (1 minute, timed on screen).** The student plans quietly. Say nothing. If they ask you a question now, answer it as below. If they are ready early, **Skip to answer** moves the timer on.

**Answer (3 minutes, timed on screen).** The student talks it through out loud.
- **Answer only what they ask.** Reveal a hidden detail **only** when their question touches it. Keep answers short and factual. See [How to play the interviewer](#4-how-to-play-the-interviewer).
- **Give no hints.** Don't prompt, nudge or rescue, even if they go quiet or get stuck. The briefing slides told them how to approach a problem and what to do when stuck; whether they follow that is part of what you are watching.
- **Optional: introduce the change** from the card, in one sentence, at about the halfway point (around 1.5 minutes in): "Let me change something…". It is a new constraint, not a hint, to see whether they listen. Then watch: do they acknowledge it, rethink, and say what changes and what stays?
- Take notes as you go. Write down one exact phrase they said that was good. You will quote it.

**After the 3 minutes, only if time allows.** Use the card's stretch prompt, or one follow-up such as "Why that one?". Skip this if you are running behind.

**Feedback (about 3 minutes).** See [Feedback script](#6-feedback-script). One strength, one habit, an example, then they redo that part for about a minute.

**Reset (under 30 seconds).**
- On the board: click **Mark done and close** to grey out the question. **Esc or Close does not mark it.** Only skip marking if you want to reuse the question.
- Go to Takeaways, click **Next student**. Finish your notes on the sheet while the next student walks up.

### How many per hour

Per student: about 1.5 minutes of slides, half a minute to draw and read, 1 minute thinking, 3 minutes answering, about 3 minutes of feedback and under half a minute to reset. That is roughly 9 to 10 minutes each, so **about 6 students per hour**, realistically 5 if you run over or use stretch prompts. To fit more, show slides 1 to 5 once to the whole room at the start and go straight to the board for each student. That saves about 1.5 minutes each and gets you to about 7 per hour.

---

## 4. How to play the interviewer

- **Hold back details until asked.** The question is vague on purpose. Do not volunteer numbers, users or constraints. Asking for them is habit 1, clarify the problem.
- **Answering a question is not a hint.** The student may ask you questions at any time during the answer. When they do, answer honestly and briefly, in one sentence, using the card's **Hidden details**. If a question is not covered on the card, make up a sensible answer and stay consistent with it. "I don't know, what would you assume?" is also fine, and invites an assumption. The line is simple: you respond to what they asked, and only that. A hint is anything you offer that they didn't ask for: a nudge, a leading question, a suggested direction, or a correction they didn't request.
- **Give no hints.** Do not rescue a stuck student, and do not prompt a silent one. If they go quiet, let the silence run; the briefing slides told them to say what they are thinking and what they'd try. Note what happened and use it in feedback.
- **Let assumptions stand.** If they state an assumption and check it ("Is that fair?"), answer from the hidden details: that is a question. If they don't check it, let it stand. A reasonable assumption is fine even if it differs from the card.
- **Never reveal "the answer".** Not during, not after. In feedback, talk about the approach, not the solution. If they ask "What's the right answer?", say: "There isn't one. I'd have liked to hear you compare X with Y."
- **Be warm and neutral.** Don't signal right or wrong with your face. Early-year students read every reaction. A friendly "Okay, go on" works for everything.
- **The change is optional, and calm.** If you use it, introduce it as a normal part of the conversation, not a trap: "Say the data no longer fits in memory. What changes?" It is a new constraint, not a hint: it tells them nothing about the solution, it tests whether they listen.
- **After the 3 minutes, only if time allows,** use the stretch prompt, or one follow-up: "Why that one?", "What's the downside of that?" or "What would make you change your mind?". If you suspect a bluff, ask "How would that work, roughly?" If it falls apart, don't push. Mention it in feedback.

---

## 5. What to look for

There are no scores. Use these descriptions to decide what to praise and which one habit to suggest working on. Calibrate for first and second years: a student who shows most of the habits some of the time is doing well. Strong does not need professional polish.

### 1. Clarify the problem

**Strong looks like**
- Asks two or three focused questions about users, scale or the goal before starting, and visibly uses the answers.
- States assumptions as assumptions, then checks them, or says what would change if they were wrong.
- Sounds like: "Who's using this? Roughly how many?" / "Is it slow for every user or just some? Because that changes where I'd look." / "I'll assume a meeting that ends at 10:00 doesn't clash with one that starts at 10:00. Is that fair?"

**Weak looks like**
- Dives straight in and asks nothing, or asks one generic question and ignores the answer.
- Assumptions stay hidden; you only find them in what they build.
- Sounds like: "Okay, so I'd build an app that…" / "How big is it?" (then ignores the answer) / (silently assumes everything fits in memory)

### 2. Think out loud

**Strong looks like**
- Talks through two or three options, with at least one trade-off each, then picks one.
- Narrates pauses, so you can follow the thinking.
- Sounds like: "A sorted list makes the search fast but every insert slow. A hash map is fast to update but can't give me a rank." / "I'm thinking about whether this fits in memory…"

**Weak looks like**
- Long silences, or only one idea.
- Mentions a second idea but doesn't compare it.
- Sounds like: "I'd use machine learning." / "Or you could use a tree, I guess."

### 3. Explain your decisions

**Strong looks like**
- Says why for each choice, tied to what matters in this problem.
- Uses what you tell them: when you answer a question or introduce the change, says what it changes and what stays.
- Sounds like: "Since we need rank as well as the top 10, I'd use a sorted structure." / "If there are a billion distinct IPs, the dictionary won't fit, so I'd split the file by IP first." / "That kills option A. B still works because…"

**Weak looks like**
- Choices with no reasons, or thin ones.
- Ignores your answers, or acknowledges the change but carries on with the original plan.
- Sounds like: "Okay. So yeah, I'd still do that." / "Because it's the best one."

### 4. Start simple, then improve and check it

**Strong looks like**
- Gets a basic version on the table first, even a slow one, and says what is wrong with it.
- Improves it step by step, explaining what each step fixes.
- Checks the result against an example and edge cases: empty or huge input, ties, two users at once.
- Sounds like: "The simple way is to compare every pair. That's billions of pairs, so I'd group by size first." / "Let me check that: what if two meetings start at exactly the same time?"

**Weak looks like**
- Jumps to the most complicated solution and can't explain how it works, or stops at the first idea.
- Never tests the idea; declares it done.
- Sounds like: "You'd use a distributed system with AI." / "Yeah, that should work." (no check)

### 5. Be honest about what you don't know

**Strong looks like**
- Says plainly when they don't know something, then reasons from what they do know.
- Says what they would check or look up.
- Sounds like: "I don't know the name of that algorithm, but I'd always expand the quickest route so far." / "I'm not sure how WebSockets work exactly, but I think…"

**Weak looks like**
- Bluffs with buzzwords, or says "I don't know" and stops.
- Sounds like: "You'd just use a neural network and blockchain." / "I haven't done that in class." (stops)

---

## 6. Feedback script

About 3 minutes. Same order every time. No scores.

1. **One specific strength, with a quote (30 s).** "When you said '[their words]', that was exactly the right move, because…"
2. **One habit to work on (20 s).** Only one. Pick the habit that was weakest, or the one that would have helped most on this problem. "The habit I'd work on is [habit]." For example: clarify the problem, think out loud, explain your decisions, start simple then improve and check it, or be honest about what you don't know.
3. **What it would have sounded like here (30 s).** Give a concrete line for this problem. "For example, at the start you could have asked, 'Is it slow on every visit, or just the first?'" or "You could have said, 'The simple version compares every pair; let me improve that.'"
4. **The redo (about 1 min).** "Let's rewind to [the start / the moment I changed the requirement]. Try it again with that habit." Let them do it. Then: "Hear the difference?"
5. **Close (20 s).** Frame it as practice, and point to the takeaways slide: "That's exactly what this is for. Keep practising that one habit."

**Encouraging phrasings for early-year students**
- "You don't need to know the answer. You did the hard part, which is thinking out loud."
- "Saying 'I don't know' and then reasoning anyway is a strength. Interviewers want to see it."
- "That pause was fine. Next time, just say what you're thinking during it."
- "Starting with the simple version was the right call. Next time, check it on an edge case before you move on."
- "Your second go was clearly better. That's the skill improving in two minutes."
- "You're a first year. Doing this at all puts you ahead."
- "You had good ideas. The fix is to say them before you decide, so I can see them."

**Avoid:** listing every weakness, giving the "answer", comparing to other students by name, any score or grade, or "good job" without a specific reason.

---

## 7. Question cards

Hidden details are reveal-only-if-asked: answering a question the student asked is not a hint. There are no rescue prompts, because you give no hints. **The change partway through is optional:** a new constraint, not a hint, to see whether they listen; use it at about the halfway point of the 3-minute answer. **Stretch prompts are for after the 3 minutes, only if time allows.** Technical notes are for you, to judge what the student says, not to teach in the session. Each card's **Source:** line names a public report showing the question, or a close variant, being asked in real interviews; it is for you, not the student.

**Calibrating for Year 1 and 2.** Every card names the core CS ideas a good answer reaches, but students don't need the formal names. "Two stacks" for undo, "sort them by start time" for meeting rooms or "check the sizes first" for duplicate files is real reasoning, and it earns the same credit as the textbook term. Each card's **What a strong approach sounds like** gives a reasonable early-year answer and a strong one. A reasonable early-year answer is a good result. Give feedback on the five habits, not the vocabulary.

## Algorithms and data structures cards

### A1 · Undo and redo

*Algorithms and data structures · Design*

**Q:** How would you implement undo and redo in a text editor?

**Source:** Glassdoor (ION Group), ION Group Interview Question: How can we implement the undo and redo functions in MS Word, which data structures are used there? https://clear.glassdoor.nl/Interview/How-can-we-implement-the-undo-and-redo-functions-in-MS-Word-which-data-structures-are-used-there-QTN_8415349.htm. Candidate-reported interview question asking how to implement undo/redo in MS Word and which data structures to use (seen in search results; page blocks direct access).

**What it really tests:** clarifying what counts as one "step", thinking out loud about options, using a new constraint (memory), checking an edge case (redo after a new edit). Core ideas: two stacks (undo and redo), storing operations rather than whole copies (command pattern), clearing the redo stack when a new edit is made.

**Hidden details**
- A plain-text editor (no images or formatting), single user.
- Typing a word should undo as one step, not one letter at a time.
- Users expect at least 100 undo steps.
- Typical documents are small (under 100 KB).
- Undo history doesn't need to survive closing the file.

**Good clarifying questions:** What counts as one undo step: a keystroke, a word, a paste? How many steps back? How big are documents? Does history survive a restart? One user or several?

**Reasonable assumptions:** Last-in, first-out order. Edits are insert, delete and replace. Memory is not a problem for small files.

**Options to explore**
- Save a full copy of the document after every step: very simple; memory is O(document size × steps).
- Store each edit as an operation that knows how to reverse itself ("inserted 'cat' at 120", undo = delete 3 characters at 120): tiny memory per step; each type of edit needs an inverse.
- Store diffs between versions: compact; more work to compute.
- Two stacks: undo pops from the undo stack, reverses the edit and pushes it onto redo; redo does the opposite. Push and pop are O(1).

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Documents can now be 50 MB log files." Good adaptation: full copies become 5 GB for 100 steps, so switch to storing operations or diffs; keep the stacks; maybe cap the history length.

**What a strong approach sounds like:** asks what a step is → notices undo is "most recent first" → two stacks → stores operations rather than copies → handles redo after a new edit. *Reasonable early-year:* "a list of past versions, take the last one off", plus "and another list for redo". *Strong:* two stacks of reversible operations, clears redo on a new edit, groups typing into words, caps the history.

**Warning signs:** never thinking about redo. Not noticing what happens to redo after a new edit. A queue (first-in, first-out) without noticing the order is wrong.

**Stretch prompt (after the 3 minutes, if time allows):** "You undo twice, then type something new. What should redo do now, and why?"

**Technical notes for you**
- The standard design is two stacks. Undo: pop from undo, apply the inverse, push to redo. Redo: pop from redo, re-apply, push to undo.
- A new edit after undoing must clear the redo stack; otherwise redo would re-apply edits to a document that has changed under them.
- The command pattern stores each action as an object with `execute()` and `undo()` methods. It is the textbook design for undo.
- Snapshots cost O(n) memory per step; operations cost O(size of the change).
- Grouping rapid keystrokes into one step (coalescing) is what real editors do. Some editors (Vim, Emacs) keep an undo *tree* instead of discarding redo history.

---

### A2 · Live leaderboard

*Algorithms and data structures · Design*

**Q:** A game has 5 million players whose scores change all the time. How would you keep track of the top 10 so it can be shown instantly?

**Source:** Hello Interview (community questions) (Meta, Google, Airbnb, PayPal), Design an Online Game Leaderboard. https://www.hellointerview.com/community/questions/realtime-game-leaderboard/cm4t0qbr9004988ilmum8jm06. Real-time leaderboard showing global top rankings and a user's own rank, reported as asked at these companies.

**What it really tests:** clarifying how often scores change compared with how often the top 10 is viewed, starting simple (re-sort everything) and improving it, checking the design against an awkward case (a top-10 player's score goes down). Core ideas: the cost of re-sorting 5 million scores, a min-heap of size 10, why the heap breaks when a top-10 score drops, a sorted structure (sorted set or balanced tree) that stays in order as scores change, and update frequency vs read frequency.

**Hidden details**
- About 2,000 score updates per second at peak.
- The top 10 is shown on every player's home screen: about 50,000 views per second at peak.
- Scores can go down as well as up: losing a match costs points.
- Ties: the player who reached the score first ranks higher.
- One global board. All 5 million scores fit easily in memory on one server.
- The top 10 may be up to a second out of date.

**Good clarifying questions:** How often do scores change? How often is the top 10 viewed? Can scores go down? How are ties broken? One global board or several? How up to date must the top 10 be?

**Reasonable assumptions:** Views far outnumber updates. Each player has one current score. The scores fit in memory (5 million numbers is tiny).

**Options to explore**
- Re-sort all 5 million scores on every view (or `ORDER BY score LIMIT 10` on every request): simple and always correct; O(n log n) per view, far too slow at 50,000 views a second.
- Work out the top 10 once a second and cache it: views become instant; still a pass over 5 million scores every second, and the list can be a second old.
- Min-heap of size 10 (the smallest of the top 10 at the root): when a score beats the root, replace the root, O(log 10); showing the top 10 just reads 10 items. Very cheap, and it's right as long as scores only go up.
- The heap's weakness: if a top-10 player's score drops, they may no longer belong, but the heap doesn't know who is 11th, so it has to scan all 5 million again. A player already in the heap whose score rises must also be updated in place, not added twice.
- Sorted structure of every player (balanced binary search tree, skip list, or a Redis sorted set) plus a map from player to current score: an update removes the old entry and inserts the new one, O(log n); the top 10 is the first 10 entries; drops are handled naturally.
- Update vs read frequency: if updates were rare, sorting on each update would be fine; if views were rare, sorting on each view would be fine. Here both are frequent, so both need to be cheap.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Each country now also wants its own top 10." Good adaptation: keep one structure (heap or sorted set) per country as well as the global one, and update both on each score change; each update costs twice as much but is still O(log n).

**What a strong approach sounds like:** asks how often scores change and are viewed, and whether they can drop → rejects re-sorting 5 million on every view → keeps only the best 10 in a min-heap → checks it: "what if someone in the top 10 loses points?" → sees the heap doesn't know who is 11th → moves to a sorted structure of all players, or explains when the heap is good enough. *Reasonable early-year:* "don't sort every time; keep a list of the best 10, and when a new score beats the lowest one, swap it in", plus noticing that a drop is a problem. *Strong:* min-heap with O(log 10) updates, the drop problem spotted and explained, a sorted set or balanced tree with O(log n) updates and the top 10 read off one end, the choice tied to the update and view rates.

**Warning signs:** sorting all 5 million on every view without noticing the cost. Never asking whether scores can go down, or assuming the heap still works when they do. Adding the same player to the top 10 twice. Ignoring ties.

**Stretch prompt (after the 3 minutes, if time allows):** "A player who isn't in the top 10 wants to see their own rank, like 'You are #48,213'. How would you work that out without counting everyone above them one by one?" (a tree where each node knows the size of its subtree, or Redis `ZREVRANK`, both O(log n)). If there is still time: "Exact rank only matters for the top 1,000; 'top 12%' is fine for everyone else. Does that make it easier?" (count players per score range and add up the ranges above).

**Technical notes for you**
- Sorting 5 million items is O(n log n), about 10^8 operations; a single pass to find the top 10 is O(n). Either is fine once a second, not 50,000 times a second.
- A min-heap of size k keeps the top k: if a new score is bigger than the root, replace the root and sift down, O(log k). It cannot handle a top-k member's score decreasing without knowing the (k+1)th score, which needs a full O(n) rescan. A common workaround keeps a larger buffer (say the top 100) and rebuilds when it runs low.
- Updating a player already in the heap needs a map from player to heap position (an indexed heap); otherwise the same player can appear twice.
- A balanced BST (red-black or AVL) or skip list ordered by (score, time reached), plus a hash map from player to current score: update = delete old entry + insert new, O(log n); the top 10 is a walk from the high end, O(log n + 10).
- Redis sorted sets (`ZADD`, `ZREVRANGE key 0 9`) implement exactly this with a skip list plus a hash table. For the stretch, rank needs subtree sizes (an order-statistic tree) or skip-list spans (`ZREVRANK`), giving O(log n); approximate rank from a histogram of scores is common in real games.

---

### A3 · Fastest route

*Algorithms and data structures · Problem*

**Q:** How would a maps app find the fastest route between two places?

**Source:** PracHub (Palantir), Find Shortest Paths in Road Network. https://prachub.com/interview-questions/find-shortest-paths-in-road-network. Palantir SWE onsite: find the shortest route between two cities in a road network, first by road count, then by distance.

**What it really tests:** clarifying "fastest", explaining how they represent the problem (a graph), starting simple (BFS) and improving it, using new information (live traffic). Core ideas: roads as a weighted graph, edge weights as travel time, Dijkstra's algorithm, A* with a distance heuristic, and why BFS only works when every edge costs the same.

**Hidden details**
- Driving only, within one country.
- The road network has about 20 million intersections.
- Each road segment has a length and a typical speed; live traffic data is available.
- The answer must come back in under a second.
- "Fastest" means shortest travel time, not shortest distance.

**Good clarifying questions:** Fastest or shortest? Driving, walking or public transport? How big is the map? How quickly must it answer? Does traffic count? One-way streets?

**Reasonable assumptions:** Travel times are never negative. One-way streets mean a directed graph. Traffic changes over time.

**Options to explore**
- Try every route: impossible; the number of paths grows exponentially.
- BFS (explore by number of hops): finds the route with fewest roads; wrong when roads take different times.
- Dijkstra: always expands the closest unexplored point using a priority queue; correct for non-negative weights; O((V + E) log V); explores in all directions.
- A*: Dijkstra plus a guess of remaining time (straight-line distance ÷ top speed), so it heads towards the goal; much faster in practice; same answer if the guess never overestimates.
- Precompute shortcuts between important junctions: very fast queries; heavy preprocessing.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "A motorway just closed because of an accident." Good adaptation: the edge weight becomes very large (or the edge is removed), re-run the search; notes that precomputed shortcuts would need updating, which is why real systems separate structure from live weights.

**What a strong approach sounds like:** pins down "fastest" → models roads as a graph with travel-time weights → explains why BFS isn't enough → Dijkstra with a priority queue → A* to speed it up → handles live changes. *Reasonable early-year:* "intersections are nodes, roads are edges, always extend the quickest route so far". *Strong:* names Dijkstra and A*, explains the heuristic, gives complexity, notes scale.

**Warning signs:** "Just check all routes." Treating distance and time as the same. "Use AI" with no mechanism.

**Stretch prompt (after the 3 minutes, if time allows):** "Dijkstra explores in every direction. How could you make it search towards the destination?"

**Technical notes for you**
- BFS gives the fewest edges, which equals the fastest route only if every edge has the same weight.
- Dijkstra (1959) is correct for non-negative weights; with a binary heap it runs in O((V + E) log V).
- A* (Hart, Nilsson and Raphael, 1968) adds a heuristic h(n); if h never overestimates (admissible), A* still finds the optimal route.
- For time-based weights, straight-line distance ÷ maximum speed is an admissible heuristic.
- Production routing uses preprocessing such as contraction hierarchies to answer continent-scale queries in milliseconds.

---

### A4 · Search autocomplete

*Algorithms and data structures · Design*

**Q:** As someone types into a search box, how would you quickly find the saved search terms that start with what they've typed so far?

**Source:** PracHub (Microsoft), Design a typeahead search service. https://prachub.com/interview-questions/design-a-typeahead-search-service. Microsoft SWE technical screen: design a search autocomplete system (prefix matching, ranking).

**What it really tests:** clarifying what "start with" means (capital letters, spaces) and how fast it must be, starting with a simple scan and improving it, explaining a memory vs speed trade-off. Core ideas: the cost of scanning every term on each keystroke, a sorted list where all terms with the same prefix sit together and binary search finds the start of that block, a trie (prefix tree), memory vs speed, and normalising case and spacing the same way when storing and when matching.

**Hidden details**
- About 1 million saved search terms, about 20 characters long on average.
- Show up to 10 matches; for now, any 10 will do, in any order.
- Matches must appear within 50 ms of each keystroke, and many people type at once.
- Capital letters don't matter: "Pyt" should match "python tutorial". Spaces at the start are ignored.
- The list of saved terms is rebuilt once a night; it doesn't change while people are typing.
- English only. The server has a few GB of memory to spare.

**Good clarifying questions:** How many saved terms are there? How fast must matches appear? Do capital letters matter? What about extra spaces? Must the term start with the text, or can the text appear anywhere in it? How many matches should be shown? How often does the list change? How much memory is there?

**Reasonable assumptions:** The terms fit in memory. Lookups happen far more often than changes to the list. Terms are stored in lowercase.

**Options to explore**
- Scan every term and check whether it starts with the typed text: simple and correct; about 1 million checks per keystroke, too slow with many people typing.
- Sorted list plus binary search: sorted alphabetically, all terms with the same prefix sit next to each other, like words in a dictionary. Binary search finds the first one in about 20 comparisons (O(log n)); then read forward until the prefix stops matching, up to 10. Compact; adding a term means shifting the list, which is fine with a nightly rebuild.
- Trie (prefix tree): each node is a letter; walk down one node per typed character, O(length of the prefix), and every match lies below that node. Each new keystroke can continue from where the last one stopped. Fast, but uses much more memory than a plain list (a node per character, each with links to its children).
- Memory vs speed: the sorted list is small and already fast enough here; the trie is faster per keystroke and fits prefixes naturally but costs memory; a compressed trie (radix tree) merges single-child chains to save some of it.
- Case and normalisation: lowercase and trim both the stored terms and the typed text in the same way; otherwise "Python" is missed, or stored twice as "Python" and "python".

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Users in France and Germany now search too, so terms contain accents like 'é' and 'ü'." Good adaptation: decides whether "cafe" should match "café", normalises both sides the same way (lowercase, perhaps strip accents), and notes that the sorted list and the trie both still work once the text is normalised.

**What a strong approach sounds like:** asks how many terms, how fast, and whether capitals matter → starts with a scan and names its cost → sorts the list so matches sit together and uses binary search to jump to them → or a trie, walking one letter at a time → weighs memory against speed → normalises case on both sides → checks an edge case (one letter typed, or no matches). *Reasonable early-year:* "keep the terms in alphabetical order and jump to where those letters start, like looking up a word in a dictionary", or "a tree where each branch is a letter". *Strong:* binary search for the prefix range with O(log n), a trie with O(prefix length), the memory trade-off, normalisation applied identically to stored and typed text, capped results.

**Warning signs:** `LIKE '%text%'` on a database on every keystroke without thinking about cost (and it matches anywhere, not just the start). "Use a hash map" with no idea how a prefix would be looked up. Forgetting about capital letters. Returning all 50,000 matches for a single letter.

**Stretch prompt (after the 3 minutes, if time allows):** "Each term now has a count of how often it was searched. How would you show the 5 most popular matches first?" (sort the matching range by count, or store the top 5 at each trie node, trading memory for speed). If there is still time: "How would you still suggest 'python' when someone types 'pyhton'?" (edit distance, much more expensive than a prefix lookup), or "Should we ask the server on every keystroke?" (wait briefly after typing stops, cache popular prefixes).

**Technical notes for you**
- A full scan costs O(n × L) per keystroke, where L is the prefix length.
- In a sorted array, two binary searches (for the prefix, and for the prefix followed by the highest possible character) give the range of matching terms in O(L log n).
- A trie lookup for a prefix of length L is O(L), independent of the number of terms; listing the matches then costs time proportional to how many are returned, which is why capping at 10 matters.
- Raw text here is about 20 MB (1 million × 20 characters). A naive trie with a 26-slot array of child links per node can take many times that; storing children in a small map, or a radix tree, reduces it.
- Normalisation must be applied identically when building and when querying: lowercasing (Unicode case folding, e.g. Python's `str.casefold()`), trimming, and for accent-insensitive matching, Unicode decomposition (NFD) and removing the accent marks.
- For the stretch: storing the top k completions at each trie node gives instant ranked answers at the cost of memory and updates; fuzzy matching for typos usually uses edit (Levenshtein) distance.

---

### A5 · Meeting rooms

*Algorithms and data structures · Problem*

**Q:** You have a list of all of today's meetings, each with a start and end time. What is the smallest number of meeting rooms needed so no two meetings clash, and how would you work it out?

**Source:** PracHub (Google), Compute minimum number of rooms needed. https://prachub.com/interview-questions/compute-minimum-number-of-rooms-needed. Google SWE technical screen: given meetings with start/end times, return the minimum number of rooms needed.

**What it really tests:** clarifying what counts as a clash (does a meeting ending at 10:00 clash with one starting at 10:00?), starting simple and improving it, checking edge cases. Core ideas: sorting meetings by start time, a min-heap of end times (the room that frees up soonest), or a sweep over sorted start and end events; O(n log n); the answer equals the largest number of meetings happening at the same moment.

**Hidden details**
- About 200 meetings today in one building, between 08:00 and 20:00.
- A meeting ending at 10:00 and one starting at 10:00 can use the same room.
- All rooms are the same; any meeting fits in any room.
- The list is not sorted: it's in the order people booked.
- Only the number of rooms is needed, not which meeting goes where.

**Good clarifying questions:** Does a meeting that ends at 10:00 clash with one that starts at 10:00? Is the list sorted? How many meetings? Are all rooms the same? Do you want just the number, or the actual room for each meeting? Can a meeting run past midnight?

**Reasonable assumptions:** Every meeting starts before it ends. Times are whole minutes. Rooms are interchangeable.

**Options to explore**
- Try every way of putting meetings into rooms: correct; the number of ways explodes.
- For each meeting's start time, count how many meetings are running at that moment; the largest count is the answer: simple and correct; O(n²), fine for 200 meetings.
- Sort by start time and give each meeting any room whose last meeting has ended, opening a new room only if none is free: correct; O(n × rooms) if you check every room each time.
- Same idea, but keep each room's end time in a min-heap: the top of the heap is the room that frees up first. If it's free by this meeting's start, reuse it (pop, then push the new end time); otherwise push a new room. The heap's size at the end is the answer. O(n log n).
- Sweep: sort all start times and all end times; walk through them in time order, +1 at a start and −1 at an end, and keep the maximum. O(n log n). At equal times, process ends before starts, since back-to-back meetings can share.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "The building only has 4 rooms. How would you find which meetings can't get one?" Good adaptation: the same sweep or heap shows the moments when more than 4 meetings overlap; when no room is free, that meeting is flagged; notes that which meeting to bump (booked last? shortest? least important?) is a policy question to ask about, not an algorithm question.

**What a strong approach sounds like:** asks about back-to-back meetings → draws a small timeline example → notices the answer is "the most meetings at once" → sorts → uses a heap or a sweep → checks edge cases (back-to-back, identical start times, one meeting, an empty list). *Reasonable early-year:* "sort them by start time, and for each meeting reuse a room that's already free, otherwise open a new one". *Strong:* min-heap of end times or a start/end sweep, O(n log n), explains why the answer can't be smaller than the busiest moment, handles ties.

**Warning signs:** assuming the list is already sorted. Counting only the meetings that overlap the first one. Getting back-to-back meetings wrong without asking. Counting overlapping *pairs* and calling that the answer.

**Stretch prompt (after the 3 minutes, if time allows):** "Why can the answer never be smaller than the number of meetings running at the busiest moment? Does your method ever use more?"

**Technical notes for you**
- This is the classic interval-partitioning problem (LeetCode 253, "Meeting Rooms II").
- Lower bound: if k meetings are running at the busiest moment, at least k rooms are needed. The greedy method (sort by start, reuse a room that has freed up) never opens a (k+1)th room, so it is optimal.
- Heap version: sorting costs O(n log n); each meeting then does at most one pop and one push at O(log n) each. Memory is O(number of rooms).
- Sweep version: two sorted arrays and two pointers, or a list of (time, +1/−1) events. With half-open intervals [start, end), an end at 10:00 must be processed before a start at 10:00.
- Checking every start against every meeting is O(n²): fine for 200 meetings, too slow for 10 million.

---

### A6 · Duplicate files

*Algorithms and data structures · Problem*

**Q:** A hard drive has 500,000 files, and many are duplicates. How would you find them efficiently?

**Source:** Glassdoor (Dropbox), Dropbox Interview Question: Detect duplicate files uploaded to Dropbox. https://www.glassdoor.ca/Interview/Detect-duplicate-files-uploaded-to-Dropbox-QTN_1866037.htm. Candidate-reported Dropbox question on detecting duplicate files; LeetCode Discuss 'Dropbox | Phone Screen | Find Duplicate File in System' (https://leetcode.com/discuss/interview-experience/307373/) corroborates (seen in search results; page blocks direct access).

**What it really tests:** clarifying what "duplicate" means, starting simple (compare every pair) and improving it, honesty about hashing. Core ideas: group by size first, then hash only the files that share a size, understand hash collisions, confirm with a byte-by-byte comparison.

**Hidden details**
- "Duplicate" means identical content, even if the name or folder differs.
- About 2 TB in total: many small documents and a few thousand large videos.
- File names are unreliable: copies are renamed, different files share names.
- The tool should report, not delete.
- It runs once on a laptop; an hour is acceptable.

**Good clarifying questions:** Identical content or similar-looking? Delete or report? How big are the files in total? Do names or dates help? How long can it run?

**Reasonable assumptions:** Reading the disk is the slow part. Most files have a unique size.

**Options to explore**
- Compare every pair byte by byte: correct; n(n−1)/2 ≈ 125 billion pairs.
- Compare names or dates: fast; wrong both ways.
- Group by size, then hash (for example SHA-256) only files in groups with more than one file, and group by hash: reads far less data; hashing is O(file size).
- Hash just the first few KB before the full hash: avoids reading whole large files that differ early.
- Byte-by-byte comparison of files whose hashes match: removes any doubt about collisions.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "The drive is on a slow network share, so reading every byte is very expensive." Good adaptation: leans harder on size grouping, adds a partial hash of the first block, and only fully reads files that still match.

**What a strong approach sounds like:** defines "duplicate" → notices pairwise comparison is too much → uses cheap checks first (size) → hashes only candidates → confirms → reports for a human. *Reasonable early-year:* "files with different sizes can't be the same, so only compare same-sized ones". *Strong:* size, then partial hash, then full hash, then byte compare, with the cost of each step.

**Warning signs:** comparing every pair without noticing the scale. Trusting names. Claiming hashes can never collide, or that collisions make hashing useless.

**Stretch prompt (after the 3 minutes, if time allows):** "Two different files could have the same hash. How likely is that, and what would you do about it?"

**Technical notes for you**
- All pairs of 500,000 is about 1.25 × 10^11 comparisons. Grouping by size or hash turns this into near-linear work.
- Identical bytes always give identical hashes; different bytes almost always give different hashes. With SHA-256, an accidental collision is practically impossible; MD5 collisions can be created deliberately.
- Grouping by size first avoids hashing most files, since unique sizes cannot have duplicates.
- Tools such as fdupes use this pipeline: size, partial hash, full hash, then byte-by-byte comparison.
- File hashing finds only exact copies. Resized or re-saved images need perceptual hashes instead.

---

## Systems and software cards

### S1 · Chat app

*Systems and software · Design*

**Q:** In a chat app like WhatsApp, how would you make sure a message still reaches someone whose phone is offline when it's sent?

**Source:** PracHub (Meta), Design a chat system similar to WhatsApp/Messenger. https://prachub.com/interview-questions/design-a-chat-messaging-system. Meta SWE onsite system-design question: design a chat system like WhatsApp/Messenger; Glassdoor (Nimble) also reports 'design a WhatsApp-like app' (search result).

**What it really tests:** clarifying what "reaches" means and how long the phone can be offline, starting simple and then improving it, explaining trade-offs. Core ideas: messages go through a server (store-and-forward), a per-user inbox (queue) of undelivered messages, delivery when the phone reconnects, a push notification to wake the phone, delivery receipts as acknowledgements, and ordering and duplicates when something is resent.

**Hidden details**
- One-to-one text messages only.
- The receiver's phone can be offline for minutes or for several days (switched off, no signal). No message may be lost.
- When the phone comes back online, waiting messages should appear within a few seconds, even if the app isn't open.
- The sender wants the ticks: one tick when the server has the message, two when it reaches the receiver's phone.
- Messages must appear in the order they were sent.
- The server may keep an undelivered message for up to 30 days.

**Good clarifying questions:** How long can the phone be offline? Is it acceptable to lose a message? Should the receiver be told even if the app is closed? Does the sender need to know it was delivered? Does order matter? How long do we keep undelivered messages? One-to-one or groups?

**Reasonable assumptions:** Phones talk to our servers, not to each other. The server is always reachable; the receiving phone often isn't.

**Options to explore**
- Phone to phone directly: fails whenever the receiver is offline, and the sender would have to keep retrying, possibly for days.
- Store-and-forward on the server: the sender uploads the message, the server saves it and acknowledges the sender (one tick), then delivers it later.
- A per-user inbox (queue) of undelivered messages: when the receiver reconnects, the phone gets everything waiting, oldest first.
- How the phone finds out: ask the server every few seconds (polling: simple, but drains the battery and mostly returns nothing) vs a push notification through Apple's or Google's push service that wakes the phone so it connects and fetches.
- Remove (or mark delivered) only after the receiving phone acknowledges; that acknowledgement becomes the sender's second tick.
- Ordering and duplicates: the server gives each message a sequence number per conversation; each message carries a unique ID, so a resent or re-delivered copy is ignored the second time.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "The receiver uses the app on a phone and a laptop." Good adaptation: each device needs its own record of how far through the inbox it has got, so a message can't be deleted on first delivery; keep it until every device has acknowledged it or the time limit runs out.

**What a strong approach sounds like:** asks how long offline can last and whether loss is acceptable → message goes via the server → server stores it in the receiver's inbox and acknowledges the sender → push notification wakes the phone → phone reconnects and fetches what's waiting → phone acknowledges, server marks it delivered and tells the sender → mentions ordering and duplicates. *Reasonable early-year:* "the server keeps the message and sends it when the other phone comes back online, with a notification to wake it up". *Strong:* a per-user queue, delete only after acknowledgement, push to wake, receipts as acknowledgements, server sequence numbers, message IDs so retries don't show twice.

**Warning signs:** phones sending straight to each other with no thought for offline. Deleting the message from the server before the receiver confirms it. The server retrying an offline phone forever without storing the message. Ordering by phone clocks. "Use Firebase" with no idea what it does underneath.

**Stretch prompt (after the 3 minutes, if time allows):** "The sender's signal drops just after sending, so the app sends the message again. How do you stop the receiver seeing it twice?" If there is still time: "When both phones are online, how does the message arrive within a second?" (a persistent connection such as a WebSocket), or "What changes for a group chat of 500 people?" (store the message once and put a reference in each member's inbox).

**Technical notes for you**
- Store-and-forward: the server saves the message and acknowledges the sender (one tick); it delivers when the receiver connects and acknowledges (two ticks); a later "read" event gives the read tick.
- Mobile operating systems close background connections to save battery; push notifications (APNs on iOS, Firebase Cloud Messaging on Android) wake the app. The push is a small, best-effort wake-up call; the messages themselves come from the server inbox.
- Deleting only after the receiver acknowledges gives at-least-once delivery; adding a unique message ID chosen by the sending phone (idempotency) means a duplicate is recognised and shown only once.
- Phone clocks drift and can be wrong, so ordering comes from server-assigned, per-conversation sequence numbers.
- For live delivery when both phones are online (stretch only), a WebSocket (RFC 6455) keeps one long-lived, two-way connection open so the server can push without being asked.
- WhatsApp states that undelivered messages are kept on its servers for up to 30 days, then deleted.

---

### S2 · 8-second page load

*Systems and software · Debug*

**Q:** A web page takes 8 seconds to load. Walk me through how you'd find where the time goes.

**Source:** Blind (Google), Real interview question: Website is running slow. Figure out the problem. https://www.teamblind.com/post/real-interview-question-website-is-running-slow-figure-out-the-problem-tnamt8c2. Thread on the 'website is running slow' interview question; a commenter says they were asked it interviewing at Google. Glassdoor (Morningstar) 'How would you troubleshoot a slow web application?' corroborates (search result).

**What it really tests:** clarifying who is affected and when, checking by measuring, narrowing down, separating frontend from backend. Core ideas: browser dev tools network waterfall, time waiting for the server vs downloading and rendering, caching, image size, CDN.

**Hidden details**
- A university events page.
- The server responds in about 0.4 seconds.
- The page loads twelve 4 MB photos straight from the camera, shown as small thumbnails.
- Many users are on mobile data.
- It's slow every time, not just the first visit; there are no cache headers.
- The server is in one country; many users are abroad.

**Good clarifying questions:** Slow for everyone or some users? Every visit or the first? Which device and network? Has it always been slow? Is the server or the page itself slow?

**Reasonable assumptions:** It's reproducible. I can open it in a browser with dev tools.

**Options to explore**
- Guess the server is slow and add more servers: often wrong.
- Open dev tools → Network tab, read the waterfall: shows each request, its size and timing; time to first byte shows server time.
- Run Lighthouse or a similar audit: highlights large images, render-blocking scripts.
- Fixes depend on the finding: resize and compress images, lazy-load below the fold, add cache headers, serve static files from a CDN; or, if the server is slow, profile the backend and its database queries.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Users say it's only slow for people abroad." Good adaptation: points to distance and latency, so a CDN serving static files near users, and caching, matter more than server code.

**What a strong approach sounds like:** asks who and when → measures in dev tools → splits server time from download time → finds the big images → fixes the biggest cost first → measures again. *Reasonable early-year:* "I'd open the Network tab and see which file takes longest". *Strong:* reads the waterfall, separates time to first byte from transfer, prioritises by size, mentions caching and CDN.

**Warning signs:** "Use a faster framework" without measuring. Blaming the database without looking. Not knowing dev tools exist and not reasoning about how they'd find out.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you stop this happening again after the next redesign?"

**Technical notes for you**
- The network waterfall shows each request, its size, and phases such as waiting for the server (time to first byte) and content download.
- Images are usually the largest bytes on a page; 48 MB over a 10 Mbit/s connection is about 40 seconds of transfer before overheads.
- Cache headers (`Cache-Control`) let repeat visits skip downloads entirely.
- A CDN serves copies of static files from servers near the user, cutting round-trip latency.
- Google's Core Web Vitals treat Largest Contentful Paint of 2.5 seconds or less as "good".

---

### S3 · Ticket site crashes

*Systems and software · Debug*

**Q:** A concert-ticket website crashes every time popular tickets go on sale and thousands of people arrive at once. What would you do?

**Source:** Exponent (now aced.io) (Meta, Google), How would you build a system on a ticketing website to manage high traffic during simultaneous ticket purchases? https://www.aced.io/questions/420/build-system-ticketing-website-high-traffic. Interview question tagged Meta and Google about a ticketing site handling high traffic during simultaneous purchases.

**What it really tests:** clarifying what "crash" means, finding the bottleneck, thinking out loud about options and their costs. Core ideas: a predictable load spike, scaling (more or bigger servers), a virtual waiting room or queue, caching and a CDN for pages that don't change, rate limiting, load testing.

**Hidden details**
- A small ticketing company; a popular band's tour goes on sale at 10:00 on a Friday.
- About 200,000 people arrive in the first few minutes for 30,000 tickets; a normal day has a few hundred people on the site at once.
- Within 2 minutes the site shows errors, and it stays slow for about an hour.
- Two web servers and one database.
- Fans refresh again and again when the page is slow, and some use bots.
- Sale times are announced weeks in advance.

**Good clarifying questions:** What exactly happens: errors, slowness, completely down? How many people at once, compared with normal? How many tickets? What's the setup? Do we have logs? Do we know about big sales in advance? Is there a budget?

**Reasonable assumptions:** It's a load problem, not a code bug (but check the logs). Because sale times are known, we can prepare.

**Options to explore**
- Scale out or up for sale days: direct; costs money; the database may still be the bottleneck.
- Virtual waiting room: let people into the shop at a rate the system can handle, in a fair order; stops refresh storms; people wait, but they know where they stand.
- Cache the pages that don't change (event page, venue map) or serve them from a CDN: cuts load cheaply.
- Queue purchase requests and process them at the rate the database can take, rather than all at once.
- Rate-limit each user and block obvious bots.
- Split the sale: presale codes or different start times by region, to spread the peak.
- Load test beforehand (k6, JMeter, Locust) to find the real bottleneck.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "There's no money for more servers." Good adaptation: shifts to a waiting room, caching and a CDN, rate limiting and bot blocking, and splitting the sale.

**What a strong approach sounds like:** asks what happens and when → compares normal and peak load → wants logs → separates "find the bottleneck" from "fix it" → offers both process and technical fixes → plans a load test before the next sale. *Reasonable early-year:* "too many people at once, so either let fewer in at a time or add servers". *Strong:* identifies the database as a likely bottleneck, explains why refreshes and bots make it worse, uses a waiting room and caching, tests before the next big sale.

**Warning signs:** "Rewrite it in a faster language." "Use the cloud" with no idea why. Jumping to a fix before knowing what breaks.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you know, before the next big sale, that the site will cope?"

**Technical notes for you**
- A crowd arriving at the same moment is often called a "thundering herd"; retries and refreshes multiply the load.
- More web servers don't help if the database is the bottleneck (for example, many transactions competing to update the same ticket counts).
- Virtual waiting rooms (Ticketmaster's queue, Cloudflare Waiting Room, Queue-it) admit users at a controlled rate. Ticketmaster's 2022 Taylor Swift presale is a well-known failure under this kind of demand, made worse by bots.
- Selling the same ticket twice is a separate problem from crashing: it needs an atomic update or transaction in the database, not more servers.
- Load testing simulates the peak in advance; without it, the first real test is the sale itself.

---

### S4 · Simultaneous edits

*Systems and software · Problem*

**Q:** Two people edit the same sentence in a shared document at the same moment. How should the system decide what the final text is?

**Source:** PracHub (OpenAI), Design Real-Time Collaborative Editing. https://prachub.com/interview-questions/design-real-time-collaborative-editing. OpenAI technical-screen system-design question on real-time collaborative editing (concurrent edits converging).

**What it really tests:** clarifying whether losing work is acceptable and whether people edit live, starting with the simplest rule and naming what it loses, explaining trade-offs. Core ideas: last-write-wins and what it loses, locking (pessimistic) vs merging (optimistic), operational transformation (OT) and CRDTs at a high level, and showing a real conflict to the users.

**Hidden details**
- A shared text document for group coursework, like a simple online editor; 2 to 5 people edit it.
- The sentence is "The meeting is on Monday." Alice changes "Monday" to "Tuesday" while Bob adds "at 3pm" at the end, within the same second.
- Neither has seen the other's edit when they make it; both edits reach the server a fraction of a second apart.
- Silently losing someone's work is the worst outcome.
- People expect to type straight away, without waiting for permission.
- Occasionally two people change the same word to different things.

**Good clarifying questions:** Are people editing live, or saving and syncing later? How many editors? Is losing an edit acceptable? Is it OK to make someone wait? Are the two edits in the same word or different parts of the sentence? What if both change the same word? Do people edit offline?

**Reasonable assumptions:** Each edit can be described as an insert or a delete at a position. The server receives edits one after another, in some order.

**Options to explore**
- Last write wins: whichever version arrives last replaces the sentence; simple, but silently loses the other edit (here, Bob's "at 3pm" or Alice's "Tuesday" vanishes).
- Locking (pessimistic): the first person to start editing the sentence or paragraph holds a lock and others wait; no conflicts, but people are blocked, and a lock left by someone who walked away needs a timeout.
- Merging (optimistic): let both edit, then combine the changes, as Git does for changes in different places; here that gives "The meeting is on Tuesday at 3pm."
- Positions shift: Alice's edit changed the sentence length, so Bob's "insert at position 24" may now point to the wrong place. Operational transformation adjusts each incoming edit for the edits it hadn't seen; CRDTs give every character a unique ID, so edits refer to IDs rather than positions and merge to the same result in any order.
- A real overlap (both change "Monday" to different words): pick one by a fixed rule (for example, by user ID) so everyone sees the same text, or keep both and show the conflict so the users decide.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Bob was offline on a train for an hour, editing the same paragraph." Good adaptation: locking can't work offline and last-write-wins would throw away an hour of work; leans towards merging or CRDTs, and showing the users any genuine conflicts.

**What a strong approach sounds like:** asks whether losing work is acceptable and whether editing is live → names last-write-wins and what it loses → considers locking and its cost → proposes merging edits in different places → notices that positions shift → for a genuine overlap, picks a consistent rule or shows the conflict. *Reasonable early-year:* "lock it while someone types", or "merge them like Git, and ask the users if they both changed the same word". *Strong:* why last-write-wins loses data, locking vs merging, the position-shifting problem, OT vs CRDTs at a high level, every copy ending with the same text.

**Warning signs:** "Whoever saves last wins" without noticing lost work. "Use timestamps" as the whole answer. Buzzwords with no mechanism. A rule under which different users end up seeing different final text.

**Stretch prompt (after the 3 minutes, if time allows):** "If I insert a word at the start of a line while you delete a word at the end, why might your delete hit the wrong word?" If there is still time: "How would undo work when two people are editing?"

**Technical notes for you**
- Last-write-wins is the simplest policy and silently discards concurrent edits. Clocks differ across devices, so even "last" is unreliable; systems use logical ordering rather than wall-clock time.
- Pessimistic locking prevents conflicts but blocks collaborators and needs timeouts; optimistic approaches let everyone edit and detect or merge conflicts afterwards.
- Operational transformation (Ellis and Gibbs, 1989) rewrites concurrent operations so they still apply correctly; Google Docs is built on OT, with a central server ordering edits.
- CRDTs (conflict-free replicated data types; Shapiro et al., 2011) guarantee that copies converge whatever order edits arrive in; libraries such as Yjs and Automerge use them, which suits offline editing.
- The key requirement is convergence: every copy ends with the same text. Which of two conflicting word changes wins matters less, unless the product chooses to show the conflict.

---

### S5 · URL shortener

*Systems and software · Design*

**Q:** A URL shortener turns a long link into a short code like bit.ly/x7Kq2. How would you generate those codes so that no two links get the same one?

**Source:** Glassdoor (Google), Google Interview Question: Design a scalable URL shortening service. https://clear.glassdoor.nl/Interview/Design-a-scalable-URL-shortening-service-QTN_8577613.htm. Candidate-reported Google question: design a scalable URL shortening service (HubSpot report also on Glassdoor) (seen in search results; page blocks direct access).

**What it really tests:** clarifying how many links there will be and whether codes may be guessable, thinking out loud about options, checking a choice with a quick calculation. Core ideas: random codes plus a collision check, a counter encoded in base62, hashing the URL and its collisions, code length vs number of links, predictability and security.

**Hidden details**
- About 1 million new links a month, kept for at least 10 years (about 120 million links in total).
- Codes should be short; up to 7 characters is fine.
- Allowed characters: a–z, A–Z and 0–9 (62 in total).
- Users must not be able to guess other people's links; some point to private documents.
- If two users shorten the same long link, they may get different codes.
- Several servers create codes at the same time.

**Good clarifying questions:** How many links in total? How short must codes be? Which characters are allowed? Should codes be hard to guess? Should the same long link always get the same code? One server or several? Can users choose their own codes?

**Reasonable assumptions:** A database table maps code → long URL, and the code column must be unique. Codes are never reused.

**Options to explore**
- A counter (1, 2, 3, …) converted to base62: no collisions by construction and the shortest possible codes; but the next code is easy to guess, and with several servers the counter must be shared, or each server given its own block of numbers.
- Random codes plus a collision check: pick 7 random characters and insert; if the code is already taken, pick again. Hard to guess; needs a check on every insert, but collisions are rare while most codes are unused.
- Hash the long URL (for example MD5 or SHA-256) and keep the first 7 characters: the same URL always gives the same code; truncated hashes collide, so a check is still needed (rehash with something added on a clash), and anyone can work out the code for a known URL.
- Length: n characters give 62^n codes. 6 characters give about 57 billion and 7 about 3.5 trillion, so 120 million links fit easily, and the extra length keeps random collisions rare and guessing hard.
- Security: random codes, or a scrambled counter (shuffle the number before encoding), so links can't be found by counting; longer codes make guessing even harder.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Some links point to private documents, so codes must not be guessable." Good adaptation: drops the plain counter; uses random codes (or a scrambled counter) with a collision check, perhaps a longer code, and limits how fast anyone can try codes.

**What a strong approach sounds like:** asks how many links and whether guessing matters → estimates about 120 million links → picks a length using 62^n → compares counter, random and hashing → handles collisions explicitly → chooses one with a reason. *Reasonable early-year:* "make random letters and numbers, and check the database to see if the code is already taken". *Strong:* base62 arithmetic, a collision check through a unique column, the counter's predictability, why hash prefixes collide, what changes with several servers.

**Warning signs:** no thought about collisions. Believing a hash is always unique. Choosing a length without any arithmetic. "Use a UUID" without noticing it is 36 characters long.

**Stretch prompt (after the 3 minutes, if time allows):** "Two servers create codes at the same moment. How do you stop them handing out the same one?" If there is still time, the parts no longer asked: "How does clicking the short link get you to the long one?" (an HTTP redirect: 301 permanent, which browsers may cache, vs 302 temporary, which lets every click be counted), or "Links are clicked far more often than they are created. What would you speed up?" (cache the code → URL lookup).

**Technical notes for you**
- Base62 with 7 characters gives 62^7 ≈ 3.5 trillion codes; 6 characters give 62^6 ≈ 57 billion.
- Converting a counter to base62 works like converting to binary: divide by 62 repeatedly and map each remainder to a character.
- Birthday effect: random 7-character codes are expected to produce a first collision after only about √(3.5 trillion) ≈ 1.9 million codes, so collisions will happen and must be checked; but with 120 million codes in use, each new code has only about a 0.003% chance of clashing.
- A unique constraint in the database makes "check and insert" one atomic step; checking first and inserting afterwards lets two servers grab the same code in between.
- Truncated hashes collide just like random codes, and anyone can compute them; sequential counters never collide but are enumerable. Several servers can share a counter by each taking a block of numbers (server A: 1–1,000,000; server B: 1,000,001–2,000,000).

---

### S6 · Parking garage

*Systems and software · Design*

**Q:** What classes would you need for a parking garage that tracks cars, spaces and tickets, and how would they relate to each other?

**Source:** PracHub (Amazon), Design a Parking Lot Management System's Object Model with Evolving Requirements. https://prachub.com/interview-questions/design-a-parking-lot-management-systems-object-model-with-evolving-requirements. Amazon SWE LLD round: design the object model (classes, methods) for a parking lot system. Also Cracking the Coding Interview OOD 7.4.

**What it really tests:** clarifying the rules before modelling, explaining design decisions. Core ideas: classes with one clear job (`ParkingGarage`, `Level`, `Space`, `Vehicle`, `Ticket`), has-a vs is-a, one-to-many relationships, subclasses vs a size attribute for vehicle types, and which class owns "find a free space".

**Hidden details**
- One garage with 3 levels and about 100 spaces per level.
- Spaces come in three sizes: small (motorbike), standard and large.
- Vehicles are motorbikes, cars and vans. A motorbike fits any space, a car fits a standard or large space, a van needs a large space.
- The system chooses a free space at the entrance barrier and prints a ticket with the vehicle, space and entry time; the ticket is closed when the vehicle leaves.
- A sign at the entrance shows the number of free spaces on each level.
- Payments are out of scope for this question.

**Good clarifying questions:** What kinds of vehicles and spaces are there? Which vehicle fits which space? One garage or many? How many levels? Does the system choose the space, or the driver? What's on a ticket? Do we need payments now? Reservations?

**Reasonable assumptions:** No reservations. One vehicle uses one space. The system knows which space each vehicle is in.

**Options to explore**
- Core classes: `ParkingGarage` (has many `Level`s), `Level` (has many `Space`s), `Space` (size, the vehicle in it or empty), `Vehicle` (licence plate, size), `Ticket` (vehicle, space, entry time, exit time).
- Has-a vs is-a: a garage has levels and a level has spaces (composition); a car is a vehicle (inheritance); a ticket refers to one vehicle and one space for one stay.
- Vehicle types as subclasses (`Car`, `Motorbike`, `Van`) vs one `Vehicle` class with a size attribute: subclasses suit different behaviour; an attribute is simpler if only the size differs.
- Who owns "find a free space": `Space` answers "can this vehicle fit in me?", `Level` searches its own spaces, and `ParkingGarage` asks each level in turn and issues the `Ticket`. Putting the search in `Vehicle` or `Ticket` gives them a job that isn't theirs.
- Free-space counts for the sign: each `Level` keeps a count, updated when a vehicle parks or leaves, rather than scanning every space each time.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Some spaces now have electric chargers, and only electric vehicles may use them." Good adaptation: adds a charger flag to `Space` and an electric flag to `Vehicle`, and extends the "can this fit?" check in `Space`; the search code barely changes, which shows why that check belongs in `Space`.

**What a strong approach sounds like:** asks which vehicles fit which spaces → lists the nouns as candidate classes → gives each class one job → states the relationships (a garage has levels, a level has spaces, a car is a vehicle, a ticket links a vehicle to a space) → chooses subclasses or an attribute with a reason → says where "find a free space" lives and why. *Reasonable early-year:* sensible classes with fields, "a level has many spaces", "a ticket has a car, a space and a time". *Strong:* has-a vs is-a stated clearly, one-to-many relationships named, the fit check in `Space`, the search in `Level` and `ParkingGarage`, payments left out on purpose.

**Warning signs:** one giant class that does everything. Inheritance where it doesn't belong (`Level extends ParkingGarage`, `Ticket extends Vehicle`). Mixing up is-a and has-a. Writing code before knowing the rules. Spending the 3 minutes on payments.

**Stretch prompt (after the 3 minutes, if time allows):** "Now add payments: an hourly price with a daily maximum, paid by card at a machine or in an app. Which classes change, and what would you add?" Good answer: a separate `PricingPolicy` that the `Ticket` or `ParkingGarage` uses, and a `Payment` interface with `CardPayment` and `AppPayment`, so new prices or payment methods don't change the other classes.

**Technical notes for you**
- Picking classes from the nouns and methods from the verbs is a classic starting heuristic.
- Has-a (composition or aggregation) vs is-a (inheritance). Garage–Level and Level–Space are one-to-many; a Ticket links one Vehicle to one Space for one stay.
- Prefer composition over inheritance when only data differs; subclass when behaviour differs.
- Give a job to the class that has the data it needs ("information expert"): `Space` knows its size, so it answers "can this fit?"; `Level` knows its spaces, so it searches them.
- Single responsibility principle: each class should have one reason to change. For the stretch, the strategy pattern (a swappable `PricingPolicy`) is the textbook way to change pricing rules without editing other classes.

---

## Data and databases cards

### D1 · University database

*Data and databases · Design*

**Q:** A university needs to record which students are enrolled in which courses. Each student takes many courses, and each course has many students. How would you set up the tables?

**Source:** Glassdoor (MongoDB), Data Modeling: University Course and students problem. https://www.glassdoor.sg/Interview/Data-Modeling-University-Course-and-students-problem-SQL-Simple-implementation-of-Linked-List-Multi-Phase-Transaction-QTN_881939.htm. MongoDB interview question listing titled 'Data Modeling: University Course and students problem'; Citadel onsite variant also on PracHub (prachub.com/interview-questions/design-a-course-registration-system-2, fetched) (seen in search results; page blocks direct access).

**What it really tests:** clarifying what must be recorded about each enrolment, explaining modelling decisions, checking the design with a quick example query. Core ideas: a `Students` table and a `Courses` table with primary keys, why a column of course IDs inside `Students` doesn't work, a join (enrolment) table with two foreign keys for the many-to-many relationship, putting enrolment-specific data such as grade and semester in the join table, and preventing duplicate enrolments.

**Hidden details**
- About 15,000 students and 800 courses; a student takes 4 to 8 courses a semester.
- Students have an ID number, a name and an email. Courses have a code (like "CS101"), a title and a number of credits.
- The registry records which semester each enrolment is for, and a grade at the end; the grade is empty until then.
- A student may retake a course in a later semester after failing it, but can't be enrolled in the same course twice in the same semester.
- The registry often asks two things: "Which courses is this student taking?" and "Who is on this course?"

**Good clarifying questions:** What do we need to know about each student and each course? Do we record grades? Semesters? Can a student retake a course? Which questions will people ask of the data? Roughly how many students and courses?

**Reasonable assumptions:** Each student has a unique ID; each course has a unique code. A relational (SQL) database.

**Options to explore**
- One big table with a row per student per course, repeating the student's name and the course title each time: easy to start; the same fact is stored many times, so a name change must be made in many rows, and rows can end up disagreeing.
- A column of course IDs inside `Students` ("CS101,MA102,…"), or columns `course1` … `course8`: "Who is on CS101?" means searching inside text in every row; no foreign key can check that the course exists; there's a fixed limit on courses; and there's nowhere to put a grade for each course.
- Three tables: `Students(student_id PK, name, email)`, `Courses(course_code PK, title, credits)`, and `Enrolments(student_id FK → Students, course_code FK → Courses, semester, grade)`. Each enrolment is one row, and both of the registry's questions become simple queries on `Enrolments`.
- Where grade and semester go: they describe one student on one course, not the student alone or the course alone, so they belong in `Enrolments`.
- Preventing duplicates: make (`student_id`, `course_code`, `semester`) the primary key of `Enrolments`, or give it its own `enrolment_id` plus a unique constraint on those three columns. Including `semester` still allows a retake; leaving it out would forbid one.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Each course also has a lecturer, and a lecturer can teach several courses." Good adaptation: a `Lecturers` table and a `lecturer_id` foreign key in `Courses`; this is one-to-many, so it needs no join table, unlike students and courses.

**What a strong approach sounds like:** asks what is recorded about an enrolment and whether retakes happen → `Students` and `Courses` tables, each with a primary key → explains why a list of course IDs in `Students` fails → adds an `Enrolments` table with two foreign keys → puts grade and semester there → stops duplicates with a key or unique constraint → checks the design with "who is on CS101?". *Reasonable early-year:* "a students table, a courses table, and a third table where each row says this student is on this course". *Strong:* primary and foreign keys named, why the list column fails, grade and semester in the join table, a composite key or unique constraint that still allows retakes, checked against a real query.

**Warning signs:** a list of course IDs in one text column on `Students`. One big table without seeing the repetition. No keys. Putting the grade on `Students` or `Courses`. A key that forbids retakes without noticing.

**Stretch prompt (after the 3 minutes, if time allows):** "Some courses have prerequisites: you must pass CS101 before taking CS201. How would you store that?" (a `Prerequisites` table with two foreign keys, both pointing at `Courses`). If there is still time: "Each course has a capacity. How would you stop it going over when two students enrol at the same moment?" (a transaction with a locking or conditional update).

**Technical notes for you**
- A primary key uniquely identifies each row; a foreign key references another table's primary key and makes the database reject a row whose target doesn't exist (referential integrity).
- A many-to-many relationship is stored as a join (junction) table, which turns it into two one-to-many relationships. Example: `SELECT s.name FROM Enrolments e JOIN Students s ON s.student_id = e.student_id WHERE e.course_code = 'CS101';`
- A list of values in one column breaks first normal form: it can't be indexed or constrained properly, and queries need string matching.
- Data about the relationship itself (grade, semester, enrolment date) belongs in the join table.
- A primary key or `UNIQUE` constraint is enforced by the database even when two requests arrive at once; checking for a duplicate in application code first and inserting afterwards is not safe.
- For the stretch: prerequisites are a many-to-many relationship of `Courses` with itself; capacity under concurrency needs a transaction, not a check-then-insert.

---

### D2 · Sign-ups down 20%

*Data and databases · Debug*

**Q:** The number of daily sign-ups on a website dropped by 20% yesterday. How would you figure out why?

**Source:** Towards Data Science (Facebook, now Meta), Mastering Facebook's metric change data science interview question. https://towardsdatascience.com/mastering-facebooks-metric-change-data-science-interview-question-part-2-2-8bf61df63828/. Walk-through of a metric-change question described as 'asked at Facebook'; InterviewQuery also has a guide to metric-drop interview questions (interviewquery.com/p/metrics-drop-data-science-interview) (seen in search results; page blocks direct access).

**What it really tests:** clarifying what is measured and compared with what, starting with the simplest explanation (is the number even right?), narrowing down step by step, explaining what each check would rule in or out. Core ideas: check the data and tracking pipeline first; compare with the right baseline; split the drop by platform, region and traffic source; check internal changes (releases, experiments, marketing) and external ones (seasonality, holidays, outside events).

**Hidden details**
- A language-learning website: normally about 10,000 sign-ups a day.
- Yesterday was a Tuesday; Tuesdays are normally much like the rest of the working week.
- The data team has checked: the sign-up counts in the database match the dashboard, so it is not a tracking error.
- Visits to the website were normal; only sign-ups fell.
- Almost all of the drop is from visitors on Android phones; desktop and iPhone are normal.
- A website release on Monday evening changed the sign-up form (it added a date-of-birth picker).
- No marketing campaign ended, and it wasn't a holiday.

**Good clarifying questions:** How is a sign-up counted? Could it be a tracking or data problem? Compared with what: the day before, or the same day last week? Did visits drop too, or only sign-ups? Is it everyone, or certain platforms, countries or traffic sources? Did we change anything: a release, an experiment, a campaign? Any holiday or outage?

**Reasonable assumptions:** One day can be noisy, but 20% is far outside normal daily variation. Changes we made ourselves are easier to check than outside causes.

**Options to explore**
- Check the data first: is yesterday's data complete, did the tracking or dashboard change, do the database counts agree? Many "drops" are tracking bugs or late data.
- Compare with the right baseline: the same weekday over the last few weeks, to rule out normal variation and seasonality.
- Walk the funnel: visits → sign-up page views → form started → form submitted. Where does the drop appear?
- Segment: platform and browser, country, traffic source (search, ads, referrals), new vs returning visitors. A drop concentrated in one segment points to a cause.
- Check internal changes: releases, A/B tests, ended marketing campaigns, price changes.
- Check external events: holidays, news, a competitor's launch, a search-ranking change, an outage at a provider (for example, the email-verification service).

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Actually, the drop is the same on every platform, country and traffic source." Good adaptation: segmentation stops pointing anywhere, so look for something that affects everyone: the tracking, a shared step such as email verification or the sign-up server (check error logs), a site-wide release, or an outside event.

**What a strong approach sounds like:** asks how sign-ups are counted → checks the data is right → compares with the right baseline → walks the funnel → segments → lines the drop up with the release → proposes how to confirm (error logs, testing the form on Android, rolling back) before claiming the cause. *Reasonable early-year:* "first check it's not a counting mistake, then see if it's one kind of user, like just phones, and whether we changed anything". *Strong:* data check first, funnel plus segmentation, internal vs external causes, and a way to confirm the cause.

**Warning signs:** jumping to one cause ("a competitor launched") without checking. Never questioning the data. Listing possible causes without saying how to check them. Comparing only with the day before.

**Stretch prompt (after the 3 minutes, if time allows):** "Once it's fixed, how would you spot a drop like this within an hour next time, rather than the next day?"

**Technical notes for you**
- This is the standard "metric change" question in data science and product interviews. Interviewers look for a structured order: validate the data, then internal vs external causes, then segment.
- Instrumentation problems (a renamed event, a broken tracking script, a late data pipeline) are a common cause of sudden drops, so rule them out first.
- Funnel analysis shows *where* users drop out; segmentation shows *who*. Together they usually point to the cause.
- Day-of-week and seasonal patterns are large in most products; compare with the same weekday in previous weeks, not only with the day before.
- A change in the mix of visitors (more traffic from a source that rarely signs up) can move the total even when no single segment changed (Simpson's paradox).
- To confirm a cause, look for direct evidence: error logs, reproducing the problem, or comparing users who did and didn't get the release.

---

### D3 · 20 GB log, 8 GB RAM

*Data and databases · Problem*

**Q:** You have a 20 GB log file and a laptop with 8 GB of RAM. How would you find the 10 most frequent IP addresses?

**Source:** PracHub (Google), Find the Most Frequent IP Addresses in a File Too Large for Memory. https://prachub.com/interview-questions/find-the-most-frequent-ip-addresses-in-a-file-too-large-for-memory-2. Google SWE technical screen: return the ten most frequent IPs, then redesign for a file whose address map cannot fit in memory.

**What it really tests:** clarifying what fits in memory, thinking out loud about options when data is bigger than RAM, starting simple and improving. Core ideas: streaming or chunking the file, counting with a hash map, hash-partitioning to disk, external sort, a heap for the top k.

**Hidden details**
- About 200 million lines; one request per line, IP address first.
- IPv4 addresses only.
- About 5 million distinct IP addresses.
- It's a one-off task; an hour is fine.
- Plenty of free disk space.

**Good clarifying questions:** How many distinct IPs? What does a line look like? One-off or repeated? Exact answer or approximate? How much disk space? IPv4 or IPv6?

**Reasonable assumptions:** Reading the file line by line is possible. The answer must be exact.

**Options to explore**
- Load the whole file into memory: doesn't fit.
- Stream line by line and count in a hash map (IP → count): one pass; fits if the distinct IPs fit (5 million entries is well under 8 GB).
- Hash-partition: write each IP to one of, say, 100 files by `hash(ip) % 100`, then count each file separately; the same IP always lands in the same file.
- External sort (for example `sort | uniq -c | sort -rn | head`): equal IPs end up adjacent; sorting spills to disk.
- Top 10 at the end: a min-heap of size 10, O(n log 10), rather than sorting all counts.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "It turns out there are 1 billion distinct addresses." Good adaptation: the hash map no longer fits, so switch to hash-partitioning to disk or an external sort, keeping the top-10 heap per partition and merging.

**What a strong approach sounds like:** asks how many distinct IPs → realises the counts matter more than the file size → streams and counts → has a plan if counts don't fit → uses a heap or partial sort for the top 10. *Reasonable early-year:* "read it a bit at a time and keep a dictionary of counts". *Strong:* reasons about distinct keys vs memory, hash partitioning or external sort, heap for top k.

**Warning signs:** "Buy more RAM" as the only idea. Splitting into chunks and taking the top 10 of each chunk (wrong: an IP can be moderately frequent in every chunk). Sorting 200 million lines in memory.

**Stretch prompt (after the 3 minutes, if time allows):** "If you split the file into 10 chunks and took the top 10 of each, could you miss the true answer?"

**Technical notes for you**
- Memory needed depends on the number of distinct keys, not the file size. 5 million IPv4 keys with counts fits easily; in Python, expect a few hundred MB.
- Top-k per arbitrary chunk then merging is wrong; top-k per *hash partition* is correct, because each IP's full count is in one partition.
- External merge sort sorts data larger than memory by sorting chunks and merging them; GNU `sort` does this automatically with temporary files.
- A min-heap of size k gives the top k in O(n log k).
- If an approximate answer were acceptable, streaming algorithms (Misra-Gries, Count-Min sketch) find heavy hitters in fixed memory.

---

### D4 · Missing values

*Data and databases · Problem*

**Q:** You're given a dataset where several columns have lots of missing values. How would you decide what to do about them?

**Source:** Glassdoor (IBM), How to deal with the missing data? https://www.glassdoor.ca/Interview/How-to-deal-with-the-missing-data-QTN_1277892.htm. IBM interview question 'How to deal with the missing data?'; the same question is listed for Capgemini, Navan, Capital One and Ingram Micro on Glassdoor (seen in search results; page blocks direct access).

**What it really tests:** clarifying why the data is missing and what it will be used for before choosing a fix, thinking out loud about options and trade-offs, checking the effect of the choice. Core ideas: why values are missing (by pure chance, explained by other columns, or because of the missing value itself: MCAR, MAR and MNAR), dropping rows or columns vs filling in (imputing) vs adding a "was missing" indicator, and how each choice changes the analysis.

**Hidden details**
- A gym chain's member data: 50,000 rows and 20 columns, to predict which members will cancel. About 10% cancel.
- `income` is missing for 40%: it was optional on the sign-up form, and higher earners skipped it more often.
- `age` is missing for 5%: a bug in the online form dropped it for a few weeks last spring, whoever the member was.
- `last_visit_date` is missing for 15%: those members have never visited.
- `phone_number` is missing for 30%, and isn't useful for the prediction anyway.
- Some missing values are stored as blanks, some as 0.

**Good clarifying questions:** What will the data be used for? How much is missing in each column? Why is it missing: a form, a bug, a merge? Does "missing" itself mean something? Is missingness related to what we're predicting? Can the data be recovered? How are missing values recorded: blank, 0, −1?

**Reasonable assumptions:** The reason differs by column, so the fix differs by column. Throwing data away is not free.

**Options to explore**
- Drop every row with any missing value: simple; here it would keep under half the rows and remove most high earners, biasing what's left.
- Drop a column: fine if it's mostly missing and not useful (phone number); loses information if it matters.
- Fill with the mean, median or most common value: keeps every row; shrinks the spread of values and hides that the value was missing.
- Fill using other columns (a regression, nearest neighbours, or multiple imputation): better estimates; more work, and still can't recover information it never had.
- Add a "was missing" indicator column alongside the filled value: the model can learn that a missing value is itself informative.
- Use a value that has a real meaning: a missing `last_visit_date` means "never visited", which is a fact, not an unknown.
- Whatever you choose, compare the results with and without it, and fit any filling on the training data only.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "It turns out members who left income blank are much more likely to cancel." Good adaptation: missingness carries signal, so don't drop those rows or hide it with a plain mean fill; add a "was missing" indicator and keep it.

**What a strong approach sounds like:** asks what the data is for and why each column is missing → treats columns differently → keeps the meaning of "missing" where it has one → chooses drop, fill or indicator with a reason → checks the effect on the results. *Reasonable early-year:* "first see how much is missing and why; if it's only a bit, drop those rows, otherwise fill with the average, though that might be misleading". *Strong:* MCAR, MAR and MNAR in plain words, indicator columns, imputation fitted on training data only, a sensitivity check.

**Warning signs:** "Just drop the rows" without looking at how many. Filling everything with 0. One rule for every column. Never asking why the data is missing. Computing fill values on the whole dataset, test set included.

**Stretch prompt (after the 3 minutes, if time allows):** "If you fill every missing income with the average, what happens to the spread of incomes, and why might that matter?"

**Technical notes for you**
- Rubin (1976) named three cases. MCAR (missing completely at random): unrelated to anything, like the form bug. MAR (missing at random): explained by other observed columns. MNAR (missing not at random): depends on the missing value itself, like high earners hiding income. MNAR can't be fixed by imputation alone.
- Dropping incomplete rows (listwise deletion) is only unbiased under MCAR, and it always loses data.
- Mean imputation shrinks the variance and weakens correlations. Multiple imputation (for example MICE) creates several filled datasets, so the uncertainty is kept.
- A missing-indicator column is a common, practical choice for prediction. Tree-based libraries such as XGBoost and LightGBM can also handle missing values directly.
- Fill values must be learned from the training data only; using the test set leaks information into the evaluation.

---

### D5 · Messy merge

*Data and databases · Problem*

**Q:** You need to merge customer records from two systems, but names and emails are written differently in each. How would you match them?

**Source:** PracHub (Ramp), Reconcile Records Across Sources. https://prachub.com/interview-questions/reconcile-records-across-sources. Ramp SWE technical screen asking to 'reconcile person records across multiple data sources' (entity resolution, normalization).

**What it really tests:** clarifying what fields exist and what a wrong match costs, starting simple (exact match) and improving it, checking match quality. Core ideas: normalising data first, fuzzy matching (edit distance), blocking to avoid comparing every pair, precision and recall of matches, human review.

**Hidden details**
- Online shop: 200,000 customers; newsletter system: 150,000.
- Shared fields: name, email, postcode. No shared customer ID.
- Differences: "J. Smith" vs "John Smith", "JOHN@Mail.com " vs "john@mail.com", nicknames, typos.
- Some people have several emails; some households share one.
- Wrongly merging two people would mix their order histories.

**Good clarifying questions:** Which fields are in both? Is there any shared ID? What does a wrong merge cost versus a missed one? How many records? Can a person review uncertain cases? One-off or ongoing?

**Reasonable assumptions:** Email is the strongest signal but not unique to a person. Names are noisy.

**Options to explore**
- Normalise first: trim spaces, lowercase emails, remove punctuation, standardise postcodes; many "different" records then match exactly.
- Exact match on normalised email: high precision; misses people who used different emails.
- Fuzzy match on name plus postcode using edit distance (how many character edits turn one into the other): catches typos; needs a threshold.
- Blocking: only compare records sharing a postcode (or first letters of surname), instead of all 3 × 10^10 pairs.
- Score each candidate pair; auto-merge high scores, send middle scores to human review, reject low scores.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Merged customers will receive each other's invoices if we get it wrong." Good adaptation: precision now matters most; raise the auto-merge threshold, send more to review, accept more missed matches.

**What a strong approach sounds like:** asks about fields and the cost of mistakes → normalises first → exact matches → fuzzy matching with a threshold → blocking for scale → human review for the uncertain middle → measures quality on a labelled sample. *Reasonable early-year:* "make everything lowercase and match on email, then check names that are nearly the same". *Strong:* edit distance, blocking, precision vs recall of matches, review band.

**Warning signs:** matching on name alone. Comparing every pair without noticing the scale. Auto-merging everything with no review.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you measure how good your matching is?"

**Technical notes for you**
- This is record linkage (entity resolution). Fellegi and Sunter (1969) formalised it as scoring pairs into match, non-match and possible match.
- Levenshtein edit distance counts insertions, deletions and substitutions; it takes O(m × n) time per pair of strings. Jaro-Winkler is common for short names.
- All pairs of 200,000 × 150,000 is 3 × 10^10 comparisons; blocking cuts this to a manageable number.
- Precision: of merged pairs, how many were truly the same person. Recall: of true pairs, how many were found. A threshold trades one for the other.
- Normalisation (case, whitespace, punctuation) often resolves a large share of mismatches before any fuzzy matching.

---

### D6 · SQL or NoSQL?

*Data and databases · Design*

**Q:** You're building an app that stores user profiles, posts and payments. Would you use a SQL or a NoSQL database, and why?

**Source:** Glassdoor (Insight), When would you use a SQL database over NoSQL database? https://www.glassdoor.com/Interview/When-would-you-use-a-SQL-database-over-NoSQL-database-QTN_5455873.htm. Insight interview question 'When would you use a SQL database over NoSQL database?'; Microsoft has a similar Glassdoor listing (seen in search results; page blocks direct access).

**What it really tests:** clarifying what the data looks like and how it's used, thinking out loud about trade-offs instead of naming a favourite, explaining each choice. A mixed answer is valid. Core ideas: ACID transactions (essential for payments), relational data and joins, fixed vs flexible schema, how each kind scales, and that one app can use more than one database.

**Hidden details**
- An app for local sports clubs: about 50,000 users at launch, perhaps 1 million in two years.
- Profiles: name, club, photo, plus optional fields that keep changing.
- Posts: text, photos, likes and comments; read far more often than written; a feed shows recent posts from the clubs you follow.
- Payments: members pay club fees in the app; every payment must be recorded exactly once, and refunds must be traceable.
- Three developers, all of whom know SQL.

**Good clarifying questions:** What does each kind of data look like, and how much is there? How is it read: by ID, by search, combined with other data? How much does consistency matter for each part? How fast will it grow? What does the team know? Does finance need reports?

**Reasonable assumptions:** Payments need strong consistency. An app this size fits comfortably on one relational database to begin with.

**Options to explore**
- Everything in a relational (SQL) database such as PostgreSQL: ACID transactions for payments, joins across users, clubs and posts, mature tools; schema changes need migrations; spreading writes over many servers takes extra work.
- Everything in a document (NoSQL) database such as MongoDB: a flexible schema suits the changing profile fields, and a post can be stored with its comments; joins are weaker, and multi-document transactions are supported but less central.
- Mixed: SQL for users, clubs and payments; a document store, key-value store or cache for the feed, like counts and sessions. Each part gets a suitable tool, at the cost of running two systems.
- SQL with a JSON column for the flexible profile fields: one database, with some flexibility.
- Either way, photos go in file or object storage, with only a link in the database.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "The app takes off: 50 million users, and the feed is read millions of times a minute." Good adaptation: keeps payments in SQL; moves the feed to something built for huge read volume (a cache, precomputed feeds, a NoSQL store that spreads across many servers) and adds read replicas; explains that scale changes the answer for some parts of the data, not all.

**What a strong approach sounds like:** asks what each kind of data needs → separates payments (correctness) from posts and feed (volume, flexibility) → explains ACID and joins in plain words → picks one, or a mix, with reasons → says what would make them change their mind. *Reasonable early-year:* "payments have to be exact, so a normal SQL database with tables; posts could go in either; I'd start with SQL because the team knows it". *Strong:* ACID named and explained, relational vs document modelling, how each scales, a justified mix, photos outside the database.

**Warning signs:** "NoSQL, because it's faster" or "more modern", with no reason. "SQL can't scale." Putting payments somewhere without transactions and not noticing. Storing photos inside the database. One answer for all the data without asking how it's used.

**Stretch prompt (after the 3 minutes, if time allows):** "A member's payment goes through, but the app crashes before it records their membership. What should the database guarantee, and how?"

**Technical notes for you**
- ACID: atomicity (all or nothing), consistency (rules always hold), isolation (concurrent transactions don't see each other's half-finished work), durability (committed data survives a crash). Payments are the textbook case.
- Relational databases link data with foreign keys and joins. Document databases keep related data together in one document: fast to read, but data gets duplicated and queries across documents are harder.
- "NoSQL" covers several families: document (MongoDB), key-value (Redis, DynamoDB), wide-column (Cassandra) and graph (Neo4j). Many were designed to spread across many servers and to allow flexible schemas.
- Many distributed NoSQL systems relax consistency for availability (eventual consistency). MongoDB has supported multi-document ACID transactions since version 4.0.
- PostgreSQL's JSONB type gives schema flexibility inside a relational database. Using different databases for different jobs is called polyglot persistence.

---

## AI and ML cards

### M1 · Cats vs dogs

*AI and ML · Problem*

**Q:** You have only 200 labelled photos and need a model that tells cats from dogs. How would you approach it?

**Source:** Glassdoor (no company named), What would you do if you have little labelled data? https://clear.glassdoor.nl/Interview/machine-learning-research-interview-questions-SRCH_KO0,25_IP6.htm. Candidate-shared ML research interview question 'What would you do if you have little labelled data?' (company not visible in snippet) (seen in search results; page blocks direct access).

**What it really tests:** clarifying the data and the goal, honesty about how little 200 is, thinking out loud about options from simple to modern. Core ideas: transfer learning (start from a pretrained model), data augmentation, a proper train/validation split.

**Hidden details**
- 110 cat photos and 90 dog photos, all labelled by one person.
- Photos are from people's phones, all sizes.
- The model will run in a pet-adoption website's upload form.
- About 90% accuracy would be "good enough"; a wrong guess just pre-fills a dropdown the user can change.
- More unlabelled photos are available; labelling costs time.
- A laptop with no powerful GPU.

**Good clarifying questions:** How balanced are the classes? Where do photos come from? What happens if it's wrong? How accurate does it need to be? Can we get more data or labels? What hardware?

**Reasonable assumptions:** Each photo has one animal. Labels are mostly correct.

**Options to explore**
- Train a neural network from scratch: 200 images is far too few; it will overfit.
- Transfer learning: take a model pretrained on millions of images (for example a ResNet trained on ImageNet), keep its learned features, retrain only the last layer on 200 photos. Works well with small data and runs on a laptop.
- Data augmentation: flips, crops, small rotations and colour changes create varied training examples from the same photos.
- Get more data: label more photos, or use a public dataset; slower, but often the biggest win.
- Hold out part of the 200 (for example 40) for validation, or use cross-validation, and never tune on the test photos.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "You notice almost every dog photo is outdoors and almost every cat photo is indoors." Good adaptation: the model may learn "grass vs sofa" instead of "dog vs cat"; collect or balance backgrounds, test on indoor dogs and outdoor cats, and check what the model looks at.

**What a strong approach sounds like:** asks about data and stakes → says 200 is small and why that matters → starts from a pretrained model → augments → keeps a separate validation set → checks for shortcuts. *Reasonable early-year:* "200 isn't many; can I reuse a model that already knows about images?" or "flip and crop them to get more". *Strong:* transfer learning with frozen layers, augmentation, honest validation, spurious correlations.

**Warning signs:** "Train a deep CNN from scratch" with no concern. Testing on training photos. Claiming 100% accuracy is achievable easily.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you know the model is looking at the animal and not the background?"

**Technical notes for you**
- Transfer learning reuses features learned on large datasets (ImageNet has over a million labelled images); fine-tuning only the final layer needs little data and compute.
- Data augmentation adds label-preserving variations and reduces overfitting; it doesn't add genuinely new information.
- With 200 images, a single validation split is noisy; k-fold cross-validation gives a steadier estimate.
- Spurious correlations (background, watermark, lighting) are a classic failure; saliency maps or targeted test sets reveal them.
- A balanced test set or per-class accuracy matters when classes are uneven.

---

### M2 · Spam filter

*AI and ML · Design*

**Q:** How would you build a filter that decides whether an incoming email is spam?

**Source:** Glassdoor (DBS Bank), Machine learning interview questions (DBS Bank). https://static.glassdoor.at/Interview/machine-learning-interview-questions-SRCH_KO0,16_IP758.htm. Interviewed at DBS Bank, May 2024: 'If you are tasked to model a spam classifier using email, how will you approach this problem?' (seen in search results; page blocks direct access).

**What it really tests:** clarifying the goal and which mistake is worse, starting simple (rules or a basic model) and improving it, checking how well it works. Core ideas: framing it as classification, where the labels come from, features from the email (words, sender, links), a simple baseline such as naive Bayes or logistic regression, precision and recall, choosing a threshold, and spam changing over time.

**Hidden details**
- A university email system: about 20,000 users and 1 million emails a day; about half are spam.
- Two years of emails that users marked "Spam" or "Not spam" are available as labels.
- Blocking a real email (an exam timetable, a job offer) is much worse than letting a spam through.
- Spammers change their messages every few weeks.
- Each email must be decided in well under a second.

**Good clarifying questions:** What data and labels do we have? Which mistake is worse? How many emails? How fast must it decide? What happens to blocked email: deleted, or moved to a spam folder? Does spam change over time? Which languages?

**Reasonable assumptions:** Users' spam reports are mostly right. Blocked email goes to a spam folder, so mistakes can be recovered.

**Options to explore**
- Hand-written rules (block known bad senders, words like "lottery"): quick to start and easy to explain; spammers dodge them, and the list never ends.
- Learn from labelled emails: turn each email into features (words, sender domain, number of links, whether the sender is known) and train a classifier. Naive Bayes is the classic simple baseline; logistic regression or gradient-boosted trees usually do better.
- Combine: rules for clear cases (allow university senders, block known bad links) plus a model for the rest.
- Choose a threshold from the costs: block only when the model is very sure; send borderline mail to the spam folder rather than deleting it.
- Keep it current: retrain regularly on new "Spam" and "Not spam" clicks, and monitor mistakes.
- Evaluate on emails from a later period than the training data, using precision (of blocked mail, how much is really spam) and recall (of all spam, how much is caught).

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Spammers start sending the message as an image, with almost no text." Good adaptation: word features stop working; lean on the sender's reputation, links, attachments, and how many users received the same message; retrain with the new examples.

**What a strong approach sounds like:** asks which mistake is worse → asks where the labels come from → starts with a simple baseline → explains the features → picks a threshold from the costs → evaluates on later data → plans retraining. *Reasonable early-year:* "use the emails people already marked as spam to train a model on the words, and check how many real emails it blocks by mistake". *Strong:* a naive Bayes or logistic regression baseline, precision vs recall tied to the costs, evaluation on later data, drift and retraining.

**Warning signs:** "Use a big neural network" before any baseline. Reporting only accuracy. Ignoring that blocking real email is costly. Training once and never updating. Testing on the training emails.

**Stretch prompt (after the 3 minutes, if time allows):** "A month after launch, how would you know the filter is getting worse, without waiting for complaints?"

**Technical notes for you**
- Naive Bayes over word counts is the classic spam filter (Sahami et al., 1998; Paul Graham's "A Plan for Spam", 2002): fast, needs little data, and a strong baseline.
- False positive = real email blocked; false negative = spam let through. Raising the threshold improves precision and lowers recall.
- With about half of emails spam, accuracy is not wildly misleading, but it still hides which mistake is happening; report both kinds of error.
- Spam is adversarial: spammers adapt, so the data drifts. Regular retraining on recent user reports is standard.
- Evaluate on a later time period than the training data, to mimic real use.

---

### M3 · "99% accurate"

*AI and ML · Problem*

**Q:** A colleague says their model for spotting fraudulent transactions is 99% accurate. What questions would you ask before trusting it?

**Source:** Glassdoor (no company named), Data science interview questions. https://static.glassdoor.es/Interview/data-science-interview-questions-SRCH_KO0,12_IP87.htm. Listed question: 'A colleague hands you a model they claim is 99% accurate for a classification task. How do you validate that?' (seen in search results; page blocks direct access).

**What it really tests:** clarifying the problem. This question *is* clarifying questions. Core ideas: class imbalance, comparing with a baseline, data leakage, where the test set came from.

**Hidden details** (what the colleague answers)
- It predicts whether a card transaction is fraud.
- About 1% of transactions are fraud.
- They tested it on the same data they trained on.
- One input column is "chargeback filed", which is only known after the fraud is discovered.
- 10,000 transactions in total.
- They didn't check how many fraud cases it actually caught.

**Good clarifying questions:** What does it predict? How common is each class? What data was it tested on? Was it separate from training? What's the precision and recall on the rare class? Are any inputs only known after the event? What does a mistake cost?

**Reasonable assumptions:** Accuracy can be misleading. The rare class is the one that matters.

**Options to explore** (things to check)
- Compare against a baseline that always predicts the majority class.
- Check the test setup: a separate test set, split by time for this kind of data.
- Check for leakage: any input that contains the answer.
- Look at the confusion matrix, precision and recall for fraud.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Your colleague says the bank wants to use it on live transactions next month." Good adaptation: raises the stakes; insists on a proper held-out test, a leakage check and a cost discussion (missed fraud vs blocked genuine customers) before launch.

**What a strong approach sounds like:** asks what it predicts and how balanced the data is → realises 99% might be trivial → asks how it was tested → spots leakage when told about chargebacks → asks for the right metrics. *Reasonable early-year:* "what's it predicting, and what did you test it on?". *Strong:* majority-class baseline, leakage, time-based split, precision and recall for fraud.

**Warning signs:** "That's great!" Asking only about the algorithm. Not knowing what to ask, and not reasoning about it.

**Stretch prompt (after the 3 minutes, if time allows):** "Why might a random train-test split be wrong for transaction data?"

**Technical notes for you**
- With 1% fraud, always predicting "not fraud" gives 99% accuracy and catches nothing.
- Testing on training data measures memorisation, not generalisation.
- Data leakage: a feature known only after the outcome ("chargeback filed") lets the model cheat; it looks perfect in testing and fails in use.
- For time-ordered data, test on later data than training; random splits can leak future information.
- Better metrics here: precision, recall, F1 or a precision-recall curve for the fraud class.

---

### M4 · Movies for new users

*AI and ML · Design*

**Q:** How would you recommend movies to a brand-new user who hasn't watched anything yet?

**Source:** huyenchip.com (no company named), Machine Learning Interviews, 8.1.2 Questions. https://huyenchip.com/ml-interviews-book/contents/8.1.2-questions.html. Q10.2: 'How would you handle a new user who hasn't made any purchases in the past?'.

**What it really tests:** clarifying what we know about the user, starting simple (popularity) and improving, using new information when a source disappears. Core ideas: the cold-start problem, popularity-based recommendations, content-based recommendations from movie features, onboarding questions.

**Hidden details**
- A streaming service with about 10,000 movies and 2 million existing users with watch histories.
- At sign-up we know country, device and age band.
- Movies have genre, year, cast, language and descriptions.
- Most new users leave within a week if the first recommendations are poor.
- The home page shows 20 movies.

**Good clarifying questions:** What do we know about the new user? What do we know about movies? Do we have other users' histories? How quickly must it improve? What counts as success: clicks, watching to the end, staying subscribed?

**Reasonable assumptions:** Most popular movies are a safe start. The user's first few clicks are very informative.

**Options to explore**
- Most popular overall: simple, safe; same for everyone.
- Popular among similar sign-ups (same country, age band, device): a little personal; risk of stereotyping.
- Onboarding: ask the user to pick a few genres or movies they like, then recommend similar ones (content-based): fast personalisation; some users skip it.
- Learn from the first clicks: update quickly after each watch; mix in some variety (explore) rather than only safe picks (exploit).
- Collaborative filtering ("people who liked X also liked Y"): powerful once they've watched something; useless at zero history.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Marketing says the onboarding questions hurt sign-ups, so they're removed." Good adaptation: falls back to popularity by country and age band, a diverse first row to learn from, and fast updates from the first few clicks.

**What a strong approach sounds like:** names the problem (no history) → asks what is known at sign-up → starts with popularity → adds onboarding or content-based → plans to switch to collaborative filtering as history builds → says how to measure success. *Reasonable early-year:* "show what's popular, and maybe ask them a few questions". *Strong:* cold start named or clearly described, content-based vs collaborative, explore vs exploit, a success metric.

**Warning signs:** "Use collaborative filtering" without noticing there's no history. Ignoring what's known at sign-up. No way to measure success.

**Stretch prompt (after the 3 minutes, if time allows):** "If you always show safe, popular picks, how would you ever discover that this user loves Korean thrillers?"

**Technical notes for you**
- Cold start applies to new users (no history) and new items (no ratings yet).
- Collaborative filtering needs interaction history; content-based filtering uses item features and works from the first preference.
- Popularity baselines are surprisingly strong and should be the comparison for any fancier method.
- Explore-exploit trade-offs are often handled with multi-armed bandit algorithms.
- Offline metrics (precision at k) and online metrics (watch time, retention, A/B tests) can disagree; online is what matters.

---

### M5 · 98% train, 60% new

*AI and ML · Debug*

**Q:** Your model scores 98% on the training data but 60% on new data. What's going on, and what would you try?

**Source:** PracHub (ByteDance), Explain Train-Test Performance Gap. https://prachub.com/interview-questions/explain-train-test-performance-gap. ByteDance Data Scientist technical screen question on explaining a train-test performance gap.

**What it really tests:** clarifying what "new data" is, thinking out loud about options, honesty about more than one possible cause. Core ideas: overfitting, regularisation, more data, a simpler model, cross-validation, checking for data leakage or distribution shift.

**Hidden details**
- Predicting whether a customer will cancel a subscription (yes or no); about half cancel.
- 2,000 training rows, 150 features.
- The model is a decision tree with no depth limit.
- One feature is the customer ID number.
- The "new data" is from customers in the following year.

**Good clarifying questions:** What's the model and how big is the data? How many features? How was "new data" collected? Is the class balance the same? Was anything tuned on the new data? Do any features look odd?

**Reasonable assumptions:** Labels are correct. The new data is meant to be like the training data.

**Options to explore**
- Overfitting: the model memorised the training set. Fixes: simpler model (limit tree depth), regularisation, fewer features, more data.
- Use cross-validation on the training data to estimate real performance and tune settings honestly.
- Check suspicious features: an ID column lets a tree memorise individual rows.
- Check distribution shift: is next year's data different (prices changed, new customer types)? Compare feature distributions.
- Leakage the other way: a feature available in training but not at prediction time.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Even with a simpler model, cross-validation on last year's data says 80%, but next year's data still gives 62%." Good adaptation: overfitting is fixed; the remaining gap points to distribution shift, so compare the two periods, retrain on recent data and monitor over time.

**What a strong approach sounds like:** names overfitting → asks about model size and data → suggests simpler model and cross-validation → spots the ID feature → separates overfitting from shift → checks what changed. *Reasonable early-year:* "it's memorised the training data instead of learning the pattern; make the model simpler or get more data". *Strong:* regularisation, cross-validation, suspicious features, distribution shift as a separate cause.

**Warning signs:** "Train for longer." "Use a bigger model." Only one explanation offered with certainty.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you tell overfitting apart from 'the world changed'?"

**Technical notes for you**
- A large gap between training and validation scores is the classic sign of overfitting (high variance).
- An unrestricted decision tree can reach near 100% training accuracy by giving every row its own leaf.
- Regularisation (L1, L2, depth limits, dropout, early stopping) penalises complexity.
- k-fold cross-validation gives a more reliable estimate than one split and is the honest place to tune settings.
- Distribution (dataset) shift: training and deployment data differ; a model can be well fitted and still fail. Time-based validation splits reveal it.

---

### M6 · Handbook chatbot

*AI and ML · Design*

**Q:** A chatbot answers students' questions using the university handbook. How would it find the right part of the handbook to answer from?

**Source:** PracHub (OpenAI), Design an enterprise RAG assistant for internal docs. https://prachub.com/interview-questions/design-an-enterprise-rag-assistant-for-internal-docs. OpenAI SWE first-round technical screen: design an assistant that answers from internal documents.

**What it really tests:** clarifying what the handbook looks like and how students phrase their questions, starting with simple keyword search and improving it, explaining a decision (how big the pieces should be), being honest about the case where nothing relevant is found. Core ideas: keyword search vs semantic search with embeddings, splitting the handbook into chunks and why chunk size matters, retrieving the top few chunks and passing them to the model with the question (retrieval-augmented generation, RAG), and what to do when no chunk is relevant.

**Hidden details**
- The handbook is a 400-page PDF with numbered sections: rules, deadlines, extensions, appeals and so on.
- Students use their own words: "Can I get more time for my essay?", while the handbook says "extension to a submission deadline".
- An existing language model (LLM) is available through an API. It can take about 10 pages of text with each question, not the whole handbook.
- Many questions aren't covered by the handbook at all ("Where's the best coffee on campus?").
- A wrong answer about a deadline could cost a student marks.

**Good clarifying questions:** How big is the handbook, and how is it organised? Do students use the same words as the handbook? How much text can the model take with each question? What if the answer isn't in the handbook? How bad is a wrong answer?

**Reasonable assumptions:** The text can be extracted from the PDF. An existing model writes the answer; our job is to hand it the right passages.

**Options to explore**
- Give the model the whole handbook with every question: simplest; too long for this model, and slow and costly per question even where it fits.
- Keyword search (like Ctrl+F, or a search engine scoring sections by matching words): simple, fast and easy to explain; good for exact terms like "appeal form"; misses "more time" when the handbook says "extension".
- Semantic search: turn each chunk and the question into an embedding (a list of numbers that captures meaning) and pick the chunks whose embeddings are closest to the question's; finds "extension" for "more time"; can miss exact codes or names, so real systems often combine both (hybrid search).
- Chunking: split the handbook into pieces before searching. Too big, and a chunk mixes several topics, its embedding is blurry, and fewer chunks fit in the prompt. Too small, and a rule is separated from its conditions or exceptions. A sensible start: follow the handbook's own sections and paragraphs, a few hundred words each, with a little overlap, keeping the section title with each chunk.
- Retrieve the top few chunks (say 3 to 5) and put them in the prompt with the question and an instruction to answer only from them: this is retrieval-augmented generation (RAG).
- When nothing relevant is found: if even the best match scores below a threshold, don't pass weak chunks to the model; reply "The handbook doesn't seem to cover this; please contact the registry" rather than letting the model guess.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Students also ask in Spanish and Arabic, but the handbook is only in English." Good adaptation: keyword search breaks across languages; multilingual embeddings can match a Spanish question to an English chunk, or the question can be translated first; then check with a few real questions.

**What a strong approach sounds like:** asks how the handbook is organised and how students phrase questions → starts with keyword search and notices it misses different wording → moves to semantic search with embeddings → splits the handbook into chunks along its sections and argues the size both ways → retrieves the top few and gives them to the model with the question → says what happens when nothing matches. *Reasonable early-year:* "split the handbook into sections, search for the section that matches the question, then give that section to the AI to answer from". *Strong:* keyword vs embeddings with an example, chunk size argued both ways, top-k retrieval into the prompt (RAG named or described), a relevance threshold leading to "I don't know".

**Warning signs:** "Just ask ChatGPT" with no retrieval at all. Training or fine-tuning a model on the handbook as the way to find the right part. Pasting all 400 pages into every question without noticing the size or cost. No thought about questions the handbook doesn't cover. Treating embeddings as magic, with no idea what is being compared.

**Stretch prompt (after the 3 minutes, if time allows):** "How would you stop the chatbot making up an answer that isn't in the handbook, and show students which section it came from?" (answer only from the retrieved chunks, cite the section number, refuse when unsure). If there is still time: "The handbook is updated twice a year. How do you keep the chatbot up to date?" (re-chunk and re-embed the new version, remove the old chunks, record the version in each source), or "How would you test that it gives correct answers before students use it?" (a set of real questions with known answers, checking both that the right passage was found and that the answer is correct).

**Technical notes for you**
- Keyword ranking is usually TF-IDF or BM25: fast and exact, but it suffers from vocabulary mismatch (different words for the same idea).
- Embeddings map text to vectors where similar meanings are close, compared by cosine similarity; retrieval is a nearest-neighbour search. 400 pages is a few thousand chunks, so comparing against every chunk is fine; vector databases with approximate nearest-neighbour indexes matter at much larger scale.
- Typical chunks are a few hundred tokens with some overlap; splitting on the document's own structure usually beats fixed-size cuts.
- RAG (Lewis et al., 2020) combines retrieval with generation so answers are grounded in specific documents; updating it means re-indexing, whereas fine-tuning would need retraining for every change.
- A similarity threshold (or a check by the model that the passages actually answer the question) is a common way to return "not found" instead of a guess.
- For the stretch: LLMs can hallucinate (produce fluent, confident, false answers); grounding and citations reduce this but don't eliminate it. Evaluation checks retrieval (right passage found?) and the answer (correct and faithful to the passage?) separately.

---

## Scenarios cards

These are workplace situations that need technical judgement rather than an algorithm or a design. There is no single right move. Listen for whether the student finds out the facts before deciding, weighs the options and their risks, and says who they would tell and how. The **Hidden details** are facts about the situation that you reveal only when asked: who is affected, deadlines, what the logs show, who decides. The change partway through stays optional. "I'd ask my manager" is a fine part of an answer, but it is not the whole answer: a strong student also says what they would bring to that conversation.

### SC1 · Ship with a bug?

*Scenarios · Scenario*

**Q:** A release is due on Friday, and while testing you find a bug that will affect about 2% of users. There's no time to fix it properly. Do you ship?

**Source:** PracHub (Google), Answer leadership and quality tradeoff questions. https://prachub.com/interview-questions/answer-leadership-and-quality-tradeoff-questions. Google SWE technical screen (Feb 2026), Q4: 'You are testing software right before a release and discover a bug that will affect some users.'.

**What it really tests:** clarifying what the bug actually does before deciding, thinking out loud about more than "ship" or "don't ship", explaining the decision and who needs to know. Core ideas: severity and impact matter more than the raw percentage, workarounds, feature flags, ship-and-fix vs delay, telling the right people.

**Hidden details**
- You found it while testing on Thursday afternoon.
- The 2% are users who pay with a discount code: their confirmation email shows the wrong total. The amount actually charged is correct.
- No data is lost or corrupted.
- The bug is in the new email template, which is behind a feature flag; switching it off brings back the old template.
- The release also contains a feature promised to a large customer for Monday.
- A proper fix takes about 2 days including testing; a hotfix release takes half a day.
- The support team is not in at the weekend.

**Good clarifying questions:** What exactly happens to those users? Is money or data affected? Is there a workaround? Is the bug new in this release? Can the broken part be switched off on its own? Who is waiting for this release? Who decides?

**Reasonable assumptions:** The decision belongs to the team or product owner; your job is to bring the facts and a recommendation.

**Options to explore**
- Ship as is and fix next week: the customer gets their feature; 2% of users get confusing emails and may contact support.
- Delay the whole release: no bug shipped; breaks a promise for a cosmetic problem.
- Ship with the flag off for the new template: customer gets the feature, nobody sees the bug; fix it, then turn the flag back on.
- Ship and tell support, with a short known-issue note: users who ask get a clear answer.
- Staged rollout: release to a small share of users first and watch.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "You find out the 2% are actually being charged twice." Good adaptation: severity has jumped, so the percentage no longer matters much; don't ship that path (flag off or delay), tell the product owner and support straight away, and check whether anyone was already charged twice.

**What a strong approach sounds like:** asks what the bug does and who it hits → separates severity from percentage → looks for a middle option (flag, workaround) → recommends one with a reason → says who to tell → changes the decision when severity changes. *Reasonable early-year:* "it depends how bad it is; if it's just a display problem, ship and fix it, but tell someone". *Strong:* severity vs reach, feature flag or staged rollout, communication plan, a clear recommendation.

**Warning signs:** "2% is small, ship it" without asking what the bug does. "Never ship with any bug." Deciding alone and telling nobody.

**Stretch prompt (after the 3 minutes, if time allows):** "What would make 2% of users a reason to stop everything?"

**Technical notes for you**
- Severity (how bad for an affected user) and reach (how many) are separate; a 2% bug that loses money or data can outrank a 50% cosmetic one.
- Feature flags (toggles) separate deploying code from releasing a feature, so one part can be switched off without a redeploy.
- Staged (canary) rollouts limit the blast radius and give early warning.
- Every release ships with known bugs; a known-issues list and a briefed support team are standard practice.
- Engineers usually recommend; the product owner or release manager decides. Saying so is good judgement, not passing the buck.

---

### SC2 · No tests, no docs

*Scenarios · Scenario*

**Q:** You join a team, and the code you need to change is large, unfamiliar, and has no tests and no documentation. How do you start?

**Source:** PracHub (Instacart), Explain how to understand a large codebase fast. https://prachub.com/interview-questions/explain-how-to-understand-a-large-codebase-fast. Instacart SWE technical screen (Jan 2026) on rapidly understanding a large unfamiliar codebase; Dataford lists the no-tests/no-docs legacy variant.

**What it really tests:** clarifying the task and the risks, starting small and checking before changing anything, honesty about not understanding the code yet, asking for help. Core ideas: reading and running the code, characterisation tests before changing it, small changes, asking teammates, documenting as you go.

**Hidden details**
- The code is an online shop's backend: about 60,000 lines of Python in a few hundred files, 5 years old.
- Your task: add a delivery-cost rule for a new country. You don't yet know where delivery costs are calculated.
- The original author left last year; one teammate has changed it a couple of times.
- It runs on every order; a mistake means charging customers the wrong amount.
- There is a staging environment, and production logs record each order's inputs and the cost charged.
- The deadline is two weeks away.

**Good clarifying questions:** What exactly do I need to change? Who knows this code best? Can I run it locally or in staging? What does a mistake cost? Are there logs of real inputs and outputs? How long do I have? Is it in version control?

**Reasonable assumptions:** The current behaviour is mostly right, because it has been charging customers for years. Version control lets me undo changes.

**Options to explore**
- Change it straight away and hope: fastest; no way to know what else broke.
- Get a map first: find where an order comes in, follow one real order through the code (search, a debugger, the logs) to where delivery cost is calculated, and sketch what you find.
- Read the code around the change, run it with real inputs, and step through it in a debugger.
- Characterisation tests first: record what the code does now for a range of real inputs (from the logs), so any change in behaviour shows up.
- Make the smallest change that works, in small commits, and run the tests after each one.
- Ask the teammate who has changed it; ask for a code review.
- Write down what you learn (a short README or comments) for the next person.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Your manager says the change is needed today, not in two weeks." Good adaptation: scales down rather than dropping safety: a few tests around just the part being changed, the smallest possible change, a teammate's review, and the remaining risk stated plainly to the manager.

**What a strong approach sounds like:** asks what the change is and what a mistake costs → finds the relevant part by tracing one real order → reads and runs that code first → pins down current behaviour with tests → makes a small change and checks it → asks the teammate → leaves notes behind. *Reasonable early-year:* "I'd run it with some examples to see what it does, then change a little bit at a time and check it still gives the same answers". *Strong:* characterisation tests from real logs, small commits, review, documentation.

**Warning signs:** "Rewrite it properly first." Changing it with no way to check. Too proud to ask anyone. Complaining about the code instead of working with it.

**Stretch prompt (after the 3 minutes, if time allows):** "Your tests show the code gives a strange result for one country. Do you fix it while you're in there?"

**Technical notes for you**
- Michael Feathers defines legacy code as "code without tests". His characterisation tests record what the code *does*, not what it *should* do, so refactoring can't silently change behaviour.
- Approval or "golden master" testing (run many real inputs, save the outputs, compare after changes) is a fast way to get coverage on untested code.
- Small, separate commits make it easy to find and undo the step that broke something.
- `git log` and `git blame` show why lines changed and who to ask.
- Fixing an odd behaviour you find on the way should be a separate, agreed change: someone may depend on it.

---

### SC3 · Broke the site

*Scenarios · Scenario*

**Q:** Your feature passed code review, but an hour after release it took the site down. What do you do in the first 30 minutes?

**Source:** PracHub (Microsoft), Respond to a Reliability Regression Shortly After Deployment. https://prachub.com/interview-questions/respond-to-a-reliability-regression-shortly-after-deployment. Microsoft SWE onsite: respond to a post-deployment reliability regression with scoped diagnosis and safe rollback decisions.

**What it really tests:** clarifying what is actually happening, explaining priorities (stop the damage before finding the cause), communicating under pressure, honesty about their own mistake. Core ideas: incident response, roll back first, communicate, find the root cause later, blameless postmortem, why review missed it.

**Hidden details**
- Your feature is a "recommended for you" panel on the home page of an online shop.
- It's 12:30 on a weekday, peak lunchtime traffic; the site is returning errors for most users.
- The logs show "too many database connections": the panel runs a slow query on every page load.
- The previous version can be redeployed in about 5 minutes. The feature has no feature flag.
- The release also added a new database column, which the old version simply ignores.
- A teammate is on call; your manager is in a meeting; there is an incidents chat channel.

**Good clarifying questions:** What exactly are users seeing? When did it start, and what changed then? What do the logs and metrics show? Can we roll back, and how fast? Did the release change the database? Who is on call? Who needs to know?

**Reasonable assumptions:** The release is the most likely cause because the timing fits. Getting the site back matters more than understanding why.

**Options to explore**
- Debug in production until you find the bug: could take hours while the site stays down.
- Roll back to the previous version: fastest way to stop the damage; safe here because the new column doesn't break the old code.
- Turn off just the feature: ideal if there were a flag; here there isn't.
- Communicate at once: tell the on-call teammate, post in the incidents channel, keep posting short updates (what we know, what we're doing, next update when).
- After recovery: confirm the site is healthy, keep notes and a timeline, then find the root cause.
- Later: a blameless postmortem, including why review missed it (load problems rarely show in a diff) and what would catch it next time.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "You've rolled back, but the site is still down." Good adaptation: doesn't assume the rollback failed; checks the database (connections may still be stuck, so restart or clear them), looks at metrics again, brings in more help and keeps updating the channel.

**What a strong approach sounds like:** asks what users see and what the logs show → links it to the release → rolls back first → tells people early and keeps them updated → confirms recovery → leaves root cause and review for later → owns the mistake without panic. *Reasonable early-year:* "undo my change first so the site works, tell my team straight away, then work out what went wrong". *Strong:* mitigation before diagnosis, safe rollback (database changes), communication cadence, blameless postmortem, load testing or feature flags for next time.

**Warning signs:** fixing forward in production while the site is down. Hiding it or waiting to be found out. Blaming the reviewer. Spending the 30 minutes on the root cause.

**Stretch prompt (after the 3 minutes, if time allows):** "Code review passed it. What would have caught this before release?"

**Technical notes for you**
- Google's SRE practice: mitigate first (roll back, switch off), diagnose afterwards. Rollback is usually the fastest safe fix when the timing points to a release.
- A rollback is only safe if database changes are backward compatible; adding a column usually is, dropping or renaming one usually isn't.
- Incidents go better with clear roles (someone fixing, someone communicating) and regular short updates.
- A blameless postmortem asks what in the process let the problem through, not who to blame; people then report problems honestly.
- Review checks code, not load. Load testing, staged rollouts, feature flags and alerts on database connections catch this kind of failure.

---

### SC4 · Won't make deadline

*Scenarios · Scenario*

**Q:** You own a feature due next week. Halfway through, you realise it can't be finished in time. What do you do?

**Source:** PracHub (Microsoft), Handling a Deadline You Will Miss, and Why Adding Engineers Late Backfires. https://prachub.com/interview-questions/handling-a-deadline-you-will-miss-and-why-adding-engineers-late-backfires. Microsoft SWE onsite: 'You own a task, and partway through you realize it cannot be delivered by its deadline. What do you do?'.

**What it really tests:** clarifying how big the gap is and what really has to ship, being honest early, thinking out loud about options beyond "work all weekend", explaining a recommendation. Core ideas: tell people early with facts, separate must-have from nice-to-have and cut scope, negotiate the date or a phased delivery, ask for targeted help, and Brooks's law (adding people to a late project can make it later).

**Hidden details**
- The feature lets customers of a food-delivery app schedule an order for later. It's due next Friday, for a marketing campaign that starts the Monday after.
- Half the time has gone and about a third of the work is done; your honest estimate is two more weeks.
- The surprise: the payment provider can't charge a card later, so you've had to work around it.
- The core (pick a time, place the order, it arrives then) could be ready by Friday. Editing or cancelling a scheduled order, and reminder notifications, could not.
- Your manager hasn't asked; you've said "going fine" at every daily stand-up.
- A teammate knows the payment system well but is busy on another project.

**Good clarifying questions:** How far behind am I, really? What is the deadline for, and what happens if it slips? Which parts matter for that date? Who depends on it? Is the date fixed or negotiable? Who could help, and with what?

**Reasonable assumptions:** The deadline exists for a reason, but the people who set it would rather know now than on Friday. Some parts of the feature matter more than others.

**Options to explore**
- Say nothing and work nights and weekends: might just make it; usually doesn't, and then everyone finds out at the last minute with no time to adjust.
- Tell the manager now, with facts: what's done, what's left, why it slipped, a new estimate. Bring options, not just the problem.
- Cut scope: ship the core by Friday, with editing, cancelling and reminders in a follow-up release; agree with the product owner what "done" means for Friday.
- Negotiate: move the date, or start the campaign with the core feature only.
- Targeted help: an hour with the teammate who knows payments might unblock you; a new person joining the whole feature now probably won't speed it up.
- Cut corners (skip tests): saves a little time now; risky, especially around payments, and costs more later.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Your manager says: 'The date can't move. I'll put two more engineers on it.'" Good adaptation: explains that new people need time to learn the code and to be coordinated, so they slow things down at first (Brooks's law); suggests one specific person for one specific, separate piece (the payments teammate, or the reminders as a self-contained task), and still proposes cutting scope.

**What a strong approach sounds like:** asks how far behind and why → tells the manager early, with facts and a new estimate → separates must-have from nice-to-have → offers options (cut scope, phase it, move the date, targeted help) → recommends one → reflects on the estimate. *Reasonable early-year:* "I'd tell my manager straight away rather than hope, and suggest doing the most important part first". *Strong:* early and honest status, scope options with their trade-offs, Brooks's law, and a plan to estimate better next time.

**Warning signs:** hiding it until the deadline. "I'd just work all weekend" as the whole plan. Blaming the payment provider or whoever estimated it. Quietly dropping tests or features without telling anyone.

**Stretch prompt (after the 3 minutes, if time allows):** "You've said 'going fine' at every stand-up. How do you handle that when you tell your manager?"

**Technical notes for you**
- Brooks's law (*The Mythical Man-Month*, 1975): "adding manpower to a late software project makes it later". New people need time to ramp up, and the number of communication paths grows as n(n−1)/2.
- Software estimates are usually optimistic, and unknowns such as a third-party limitation are a common cause. Re-estimating as soon as you learn something new is good practice.
- Scope, time, quality and people trade off against each other; cutting scope is usually the safest lever.
- Sorting work into must-have and nice-to-have (for example MoSCoW: must, should, could, won't) makes scope cuts easier to agree.
- Bad news early gives a manager options (move the campaign, reassign people, reduce scope); bad news on the deadline leaves none.

---

### SC5 · Rewrite it?

*Scenarios · Scenario*

**Q:** A teammate wants to rewrite a working system in a new language or framework. You think it's a bad idea. How do you handle it?

**Source:** Tech Interview Handbook (Slack), Behavioral interview questions (Slack Software Engineer section). https://www.techinterviewhandbook.org/behavioral-interview-questions/. Slack SWE: 'If someone has a different viewpoint to do a project like different programming language, how would handle this situation?'.

**What it really tests:** clarifying the teammate's reasons before arguing, thinking out loud about options beyond "yes" or "no", explaining a position with evidence, accepting the team's decision. Core ideas: understanding their reasons, the costs and risks of rewrites, incremental migration and the strangler pattern, a prototype or spike, agreeing criteria, disagree and commit.

**Hidden details**
- The system is an internal booking tool: about 40,000 lines of PHP, 8 years old, few bugs.
- The teammate wants to move it to TypeScript and a modern web framework. Their reasons: it's slow to add features, and new hires don't know PHP.
- Team of 4; a large feature is due in 3 months.
- There are almost no automated tests.
- The teammate is more senior than you. The tech lead decides next week.

**Good clarifying questions:** Why do they want to rewrite it? What problem are they trying to solve? How big is the system? Does it work well today? What deadlines are coming? Who decides? Are there tests to show the new version behaves the same?

**Reasonable assumptions:** The teammate has a real problem, even if a full rewrite isn't the right fix. Both of you want the product to succeed.

**Options to explore**
- Argue against it in the meeting: may win the argument; may lose the teammate.
- Talk privately first to understand their reasons; they may know pain points you don't.
- Name the costs and risks: months with no new features, years of bug fixes lost, two systems to run during the switch, the 3-month deadline.
- Incremental migration (the strangler pattern): build new parts in the new framework and move old parts over one at a time, so the old system keeps working.
- A time-boxed spike: rebuild one small part to measure the real effort.
- Agree criteria up front (deadline risk, effort, hiring) and let the tech lead decide against them.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "The tech lead decides to go ahead with the full rewrite." Good adaptation: disagree and commit: support it properly, suggest ways to reduce the risk (tests that compare old and new behaviour, migrating in stages), and don't undermine it or say "I told you so".

**What a strong approach sounds like:** asks why they want it → acknowledges the real problem → lays out costs and risks with evidence → offers a middle path (incremental migration, spike) → proposes agreed criteria → accepts the decision. *Reasonable early-year:* "I'd ask why first, then say my worries, maybe suggest trying it on one small part first". *Strong:* rewrite risks named, strangler pattern, spike, decision criteria, disagree and commit.

**Warning signs:** "I'd just tell them no." Going round them to the manager first. Refusing to work on it if the decision goes the other way. Treating it as a personal contest.

**Stretch prompt (after the 3 minutes, if time allows):** "What evidence would change your mind and make you support the rewrite?"

**Technical notes for you**
- Joel Spolsky's "Things You Should Never Do" (2000) argues that rewriting from scratch throws away years of bug fixes hidden in old code.
- Fred Brooks's "second-system effect": the replacement tends to be over-designed.
- Martin Fowler's strangler fig pattern replaces a system piece by piece behind a stable interface, so there is no big-bang switch.
- A spike is a short, time-boxed experiment to reduce uncertainty, thrown away afterwards.
- "Disagree and commit": argue your case clearly, then fully support the decision once it's made.

---

### SC6 · Unsafe passwords

*Scenarios · Scenario*

**Q:** Your manager asks you to build a feature that stores users' passwords in a way you think is unsafe. What do you do?

**Source:** Hello Interview (community questions) (Capital One, Meta, Amazon), Tell me about a time when you strongly disagreed with your manager or peer on something important. https://www.hellointerview.com/community/questions/manager-peer-disagreement/cm5ya8anj0039rfqrg4m6t4vi. Asked at Capital One/Meta/Amazon; model answer is pushing back on a manager who wanted authentication turned off, on security grounds.

**What it really tests:** clarifying what the manager actually needs, explaining why it's unsafe in terms the manager cares about, offering alternatives, honesty and integrity under pressure. Core ideas: plaintext or reversible encryption vs a slow salted hash such as bcrypt, scrypt or Argon2; raising it with reasons and alternatives; escalating if needed; never quietly complying or quietly refusing.

**Hidden details**
- The manager wants passwords stored with reversible encryption, so support staff can read a password out to a customer who forgot it.
- The real problem: customers keep calling support because they can't log in.
- About 50,000 users of a gym-booking app, in the UK and EU.
- Passwords are currently stored with bcrypt.
- The manager isn't technical, and the deadline is next week.
- The company has a security lead, who is rarely consulted.

**Good clarifying questions:** What exactly are they asking for, and why? What problem are they trying to solve? How are passwords stored now? Who would see them? Which laws apply? Is there a security lead? What's the deadline?

**Reasonable assumptions:** The manager wants fewer support calls, not weaker security. Many users reuse the same password on other sites.

**Options to explore**
- Do it as asked: meets the deadline; anyone with database and key access, or any attacker who gets both, can read every password.
- Quietly refuse, or quietly keep hashing and say it's done: avoids harm short term; dishonest, and breaks trust when found out.
- Explain the risk in business terms: a breach exposes passwords people reuse for email and banking, plus legal and reputational damage.
- Offer an alternative that solves the real problem: a password-reset link by email, so nobody ever needs to see a password.
- Put the concern in writing; if the manager still insists, escalate to the security lead.

**The change partway through (optional):** a new constraint, not a hint, to see whether they listen. "Your manager says: 'I hear you, but it's my call. Just do it.'" Good adaptation: stays calm, restates the risk and the alternative once in writing, escalates to the security lead or the manager's manager, and is open about doing so.

**What a strong approach sounds like:** asks why they want it → explains why it's unsafe → offers a reset flow that solves the real problem → raises it openly → escalates if needed. *Reasonable early-year:* "passwords should be hashed so nobody can read them; I'd explain that and suggest a reset link instead". *Strong:* hashing vs encryption explained, salt and slow hash named, business and legal risk, alternative, escalation path.

**Warning signs:** "The manager is the boss, so I'd do it." Quietly doing something different. Calling the idea stupid without offering an alternative. Not knowing why plaintext is bad, and not reasoning about it.

**Stretch prompt (after the 3 minutes, if time allows):** "Explain to a non-technical manager, in two sentences, why hashing is safer than encryption here."

**Technical notes for you**
- Hashing is one-way; encryption is reversible by anyone with the key. If the database and key leak together, every encrypted password is exposed.
- OWASP recommends a slow, salted password hash: Argon2id first, then scrypt or bcrypt (PBKDF2 where FIPS compliance is required). Fast hashes such as MD5 or plain SHA-256 are cracked quickly on GPUs.
- A unique salt per user stops precomputed (rainbow) tables and hides which users share a password.
- NIST SP 800-63B requires stored passwords to be salted and hashed with a suitable one-way key derivation function; a reset link replaces "tell me my password".
- UK and EU GDPR (Article 32) requires appropriate security for personal data; a plaintext-equivalent password store would be hard to defend after a breach.

---

## Your experience cards

These are about the student's own technical work. There are no hidden details or change. Instead, probe for honesty and depth with the probing questions after the 3 minutes, if time allows, as you would a stretch prompt. Any project counts: coursework, a hobby project, a hackathon, a part-time job. If they have no example, let them use a school or personal one.

### E1 · Hardest bug you fixed

*Your experience*

**Q:** Walk me through the hardest bug you've fixed. How did you narrow it down?

**Source:** Tech Interview Handbook (Dropbox), Behavioral interview questions. https://www.techinterviewhandbook.org/behavioral-interview-questions/. Most-common list: 'What was the most difficult bug that you fixed in the past 6 months?'; Dropbox: solved a technical problem, 'be specific about the diagnosis and process'.

**What it really tests:** starting simple and checking (reproduce, narrow down, confirm the fix), honesty about false starts, explaining why the fix worked. Core ideas: reproducing the bug, reading the error, isolating the cause (print statements, a debugger, binary search through the code or commits), confirming the fix.

**Good structure:** what went wrong and why it was hard → how they reproduced it → how they narrowed it down, in order → the cause → the fix and how they checked it → what they'd do differently.

**Probing questions**
- "Why was that one the hardest?"
- "What did you see that told you something was wrong?"
- "What was your first guess, and was it right?"
- "How did you rule things out?"
- "What exactly was the cause? Show me with your hands, or describe the line."
- "How did you know it was really fixed?"
- "Did you understand *why* the fix worked?"

**Signs it's rehearsed or exaggerated**
- A neat story with no false starts.
- Can't name the error message, tool, language or line.
- "I just googled it and it worked" with no idea why.
- Story changes when you ask for detail.
- Claims to have fixed everything alone in a group project.

**What a strong approach sounds like:** *Reasonable early-year:* "I printed values until I found where it went wrong", plus an honest account of the fix. *Strong:* reproduces reliably, narrows systematically (halving the code, a debugger, comparing a working and broken version), confirms with a test.

**Warning signs:** blaming the tools or a teammate. A trivial typo with no reflection. "I've never had a bug."

**Stretch prompt (after the 3 minutes, if time allows):** "How would you stop that bug coming back?"

**Technical notes for you**
- Good habits to listen for: reproducing first, reading the full error and stack trace, changing one thing at a time, using a debugger or prints, explaining it aloud (rubber duck).
- Binary search through code (comment out half) or history (`git bisect`) is a strong, general technique.
- A test that failed before the fix and passes after shows maturity.
- "I fixed it but I'm still not sure why" is honest; praise it under habit 5, being honest about what you don't know.

---

### E2 · A technical decision

*Your experience*

**Q:** Tell me about a technical decision you made in a project or assignment. What were the options, and why did you choose yours?

**Source:** Exponent (now aced.io) question bank (Asana), Technical trade-offs. https://www.aced.io/questions/154/technical-tradeoffs. Tagged Asana: 'Tell me about a project where you had to make technical trade-offs.'.

**What it really tests:** thinking out loud about options and explaining the decision, honesty about downsides. Core ideas: naming real alternatives, the criteria that mattered (time, performance, team skills, requirements), and how it turned out.

**Good structure:** context → at least two options → what mattered → the choice and reason → how it turned out → what they'd do now.

**Probing questions**
- "What other option did you seriously consider?"
- "What would have made you choose the other one?"
- "Was it your decision or the group's? What was your part?"
- "How did it turn out? Anything you'd change?"
- "What's one downside of what you chose?"
- "Who disagreed, and what did they say?"

**Signs it's rehearsed or exaggerated**
- Only one option, presented as obviously right.
- "We decided" throughout, but can't say what they personally did.
- Can't explain the alternative in any detail.
- Perfect outcome, no downsides.
- Uses technical terms they can't explain when asked.

**What a strong approach sounds like:** *Reasonable early-year:* "I used a dictionary instead of a list because lookups were slow", with a reason. *Strong:* two real options, criteria named, a downside admitted, and what they'd choose now.

**Warning signs:** "The lecturer told us to use X" with no reflection. No reasons at all.

**Stretch prompt (after the 3 minutes, if time allows):** "If the project had to handle 100 times more data, would you decide differently?"

**Technical notes for you**
- Small decisions are fine (a list vs a dictionary, Python vs Java for a script, a chart type). The reasoning matters, not the size.
- Strong answers mention a constraint (deadline, team skills, marking criteria, performance) as the reason.
- "I'm not sure it was the right choice, because…" shows maturity; reward it.
- Check understanding with one gentle "How does that work, roughly?" on any term they use.

---

### E3 · Hard to learn

*Your experience*

**Q:** Tell me about something technical you didn't understand at first and had to learn quickly. How did you learn it?

**Source:** AlgoDaily (Amazon), Amazon Leadership Principles interview questions: Learn and Be Curious. https://algodaily.com/lessons/amazon-leadership-principles-interview-questions/learn-and-be-curious. Amazon LP example: 'Tell me about a time you had to learn a new skill or technology quickly.'.

**What it really tests:** honesty about what they didn't (and still don't) know, how they learn. Core ideas: whether they can explain the topic simply now, and the strategies they used (experiments, worked examples, explaining to others).

**Good structure:** what it was → why they had to learn it quickly → what was confusing → what they tried → the moment it clicked → how they'd explain it now.

**Probing questions**
- "How much time did you have, and what did you learn first?"
- "What exactly was confusing at first?"
- "What resources did you use, and which helped most?"
- "Can you explain it to me now in a sentence or two?"
- "What's a part of it you still don't fully get?"
- "How did you check you really understood it?"
- "What would you tell a first year learning it now?"

**Signs it's rehearsed or exaggerated**
- Can't explain the topic simply when asked.
- Claims full mastery of something big ("I learned machine learning").
- No detail about how they learned, only that they did.
- Vague resources ("online stuff").

**What a strong approach sounds like:** *Reasonable early-year:* recursion or pointers, explained roughly but correctly, with a concrete example of what helped. *Strong:* clear explanation in their own words, a small experiment they ran, and an honest note on what's still fuzzy.

**Warning signs:** bluffing when asked to explain the concept. Picking something they still can't explain at all, without admitting it.

**Stretch prompt (after the 3 minutes, if time allows):** "How do you know when you've really understood something rather than memorised it?"

**Technical notes for you**
- The "explain it in a sentence" probe is the best honesty test. You don't need deep expertise in their topic; listen for whether the explanation is coherent and in their own words.
- Good learning habits: small experiments, worked examples, explaining to others, practice after reading, checking against tests or exercises.
- If they say "I still don't fully get X", that is a strength on habit 5, being honest about what you don't know, not a weakness.

---

### E4 · Code feedback

*Your experience*

**Q:** Tell me about feedback you got on your code or project, from a teammate, TA or reviewer. What did you change, and what did you push back on?

**Source:** Tech Interview Handbook (no company named), Behavioral interview questions (most commonly asked). https://www.techinterviewhandbook.org/behavioral-interview-questions/. Most-common list across top tech companies: 'What is the most constructive feedback you have received in your career?' and 'How have you handled criticism of your work?'.

**What it really tests:** honesty about their own mistakes, explaining decisions (what they changed and why, and what they didn't), disagreeing respectfully. Core ideas: specific changes made in response to feedback, telling a real problem from a matter of taste, pushing back with reasons or evidence rather than defensiveness, and what they learned and still do.

**Good structure:** the project and who gave the feedback → what the feedback said, specifically → what they changed, and how → anything they pushed back on, and how → how it was settled → what they do differently now.

**Probing questions**
- "What exactly did they say? Can you remember the words?"
- "How did you react when you first read it?"
- "What did the code look like before and after, roughly?"
- "Was there a comment you disagreed with? What did you say?"
- "How was that settled?"
- "What do you do now, by default, because of that feedback?"

**Signs it's rehearsed or exaggerated**
- The "feedback" is really praise ("they said my code was almost too efficient").
- Can't name a single specific change.
- Accepted every comment without thought, or rejected every one.
- The pushback always ends with them being right and the reviewer admitting it.
- Vague about who gave the feedback, or on what.

**What a strong approach sounds like:** *Reasonable early-year:* "my TA said my functions were too long and my variable names were unclear, so I split them up and renamed things, and now I do that from the start". *Strong:* specific feedback, concrete changes, one point they pushed back on with a reason or a quick test, a respectful resolution, and a habit that stuck.

**Warning signs:** dismissing all feedback ("they didn't understand my code"). Blaming the reviewer. "I've never had any feedback." Nothing changed as a result.

**Stretch prompt (after the 3 minutes, if time allows):** "If you found the same problem in a classmate's code, how would you word the comment?"

**Technical notes for you**
- Common, credible feedback for early-year students: naming, long functions, repeated code, missing tests or error handling, no comments, inconsistent style, hard-coded values.
- Good pushback gives a reason or evidence ("I kept the simple loop because the input is always tiny; here's the timing") and accepts the outcome; it isn't about winning.
- Google's code review guidelines ask reviewers to comment on the code, never the developer, and to explain their reasoning; listen for whether the student separates the code from themselves.
- "I was defensive at first, then realised they were right" is honest; reward it under habit 5, being honest about what you don't know.

---

### E5 · Do it differently

*Your experience*

**Q:** Tell me about a project you'd build differently now. What would you change, and why?

**Source:** Tech Interview Handbook (Amazon), Behavioral interview questions (Amazon Software Engineer section). https://www.techinterviewhandbook.org/behavioral-interview-questions/. Amazon SWE: 'Tell me a situation where you would have done something differently from what you actually did.'.

**What it really tests:** honesty about past mistakes, explaining decisions with hindsight, showing what they have learned. Core ideas: specific technical changes (structure, data structures, testing, version control, planning, scope), the reason each one matters, and the cost of the original choice.

**Good structure:** the project → what they built and how → what went wrong or became painful → what they'd change → why that would be better → what it cost them at the time.

**Probing questions**
- "What exactly became painful, and when did you notice?"
- "Why did you make the original choice at the time?"
- "What would the change have cost you back then?"
- "How do you know the new way would actually be better?"
- "Have you done it the new way since? How did it go?"
- "Is there anything you'd keep exactly the same?"

**Signs it's rehearsed or exaggerated**
- Only generic lessons ("I'd plan better", "I'd start earlier") with no technical detail.
- A "flaw" that is really a boast ("I'd make it less ambitious because it was too impressive").
- Can't say why the original choice was made.
- Can't explain how the new approach works.

**What a strong approach sounds like:** *Reasonable early-year:* "my game kept everything in one huge file; I'd split it into classes, because every change broke something else". *Strong:* a specific change, the problem it would solve, a fair account of why the original choice seemed sensible, and evidence the lesson stuck.

**Warning signs:** "I wouldn't change anything." Blaming the brief or the lecturer. Changes that don't connect to any problem they described.

**Stretch prompt (after the 3 minutes, if time allows):** "What's one habit from that lesson that you use in every project now?"

**Technical notes for you**
- Common, credible answers: no version control, one giant file or function, no tests, hard-coded values, the wrong data structure, too much scope for the time.
- A strong answer explains why the original choice was reasonable then (deadline, didn't know better); that is good judgement, not an excuse.
- Hindsight is easy; listen for whether they can say what signal should have warned them earlier.
- Check the new approach with one gentle "How would that work, roughly?"

---

### E6 · Vague brief

*Your experience*

**Q:** Tell me about a time you had to start a task with a vague or incomplete brief. What did you do?

**Source:** Exponent (now aced.io) question bank (Google, Amazon), Face ambiguity. https://www.aced.io/questions/5018/face-ambiguity. 'Tell me about a time in your career when you faced ambiguity.' Tagged Google, Amazon, Salesforce, Netflix, DoorDash; roles include Software Engineer.

**What it really tests:** clarifying the problem in real life (habit 1 outside the interview), stating assumptions, starting simple and checking it with whoever set the task. Core ideas: asking questions early, writing assumptions down and confirming them, building a small first version for feedback, checking against marking criteria or requirements.

**Good structure:** the task and what was unclear → what they asked, and whom → what they assumed and how they checked → a first version → feedback and changes → the outcome.

**Probing questions**
- "What exactly was unclear?"
- "Who did you ask, and what did they say?"
- "What did you assume, and did you tell anyone?"
- "Did any of your assumptions turn out wrong? What happened?"
- "How did you know you were building the right thing?"
- "What would you ask first if you got the same brief tomorrow?"

**Signs it's rehearsed or exaggerated**
- "I just figured it out" with no questions asked or assumptions named.
- Can't say what was unclear in the brief.
- Every assumption turned out right.
- No mention of checking with anyone.

**What a strong approach sounds like:** *Reasonable early-year:* "the coursework didn't say what format the output should be, so I asked on the forum and wrote my assumption at the top of the report". *Strong:* specific questions, written assumptions, an early version shown for feedback, and an assumption that turned out wrong and how they handled it.

**Warning signs:** guessing silently and blaming the brief later. Waiting until the deadline to ask. Never having noticed a brief was vague.

**Stretch prompt (after the 3 minutes, if time allows):** "If you couldn't reach anyone to ask, how would you decide what to build?"

**Technical notes for you**
- This is habit 1, clarify the problem, applied for real; link your feedback to it.
- Writing assumptions down (in a README, the report or a message) makes them easy to check and protects the student if they turn out wrong.
- A small early version shown for feedback is the cheapest way to find a misunderstanding.
- Marking criteria and example answers are part of the brief; strong students read them as requirements.

---

## 8. Tips for students

Read or show these at the end of the session, or point to the takeaways slide.

1. **Clarify the problem.** Ask two or three questions about scale, constraints and what matters; the question is vague on purpose. Then say your assumptions out loud and check them: "I'm going to assume… Is that fair?"
2. **Think out loud.** Give two or three options before you pick one, and say the downside of each. Silence looks like being stuck; "I'm thinking about whether…" keeps the interviewer with you.
3. **Explain your decisions.** Say why you chose what you chose. When the interviewer answers a question or changes something, say what it changes and use it.
4. **Start simple, then improve and check it.** Get a basic version first, even a slow one. Improve it, then test it on an example and an edge case before you say you're done.
5. **Be honest about what you don't know.** "I don't know, but here's how I'd reason about it" is a strong answer. Bluffing isn't.
6. **Practise with a friend.** Pick any app you use (a search box, a maps route, a game leaderboard), give yourself 1 minute to think, then 3 minutes to talk through "how would I build that?" out loud.

---

## 9. Feedback notes sheet

One row per student. No scores: quote one thing they said that was good, and note the one habit to work on.

| Student | Question | What went well (quote them) | What to work on |
|---|---|---|---|
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |
| | | | |

---

## 10. Sources

The public source for each interview question is on its card's **Source:** line. The references below support the guide's method and the technical notes.

**Structured interviews and interview practice**
- Schmidt, F. L. and Hunter, J. E. (1998). The validity and utility of selection methods in personnel psychology. *Psychological Bulletin*, 124(2), 262–274.
- Sackett, P. R., Zhang, C., Berry, C. M. and Lievens, F. (2022). Revisiting meta-analytic estimates of validity in personnel selection. *Journal of Applied Psychology*, 107(11), 2040–2068. Structured interviews came out as one of the strongest predictors of job performance.
- Levashina, J., Hartwell, C. J., Morgeson, F. P. and Campion, M. A. (2014). The structured employment interview: Narrative and quantitative review of the research literature. *Personnel Psychology*, 67(1), 241–293.
- Google re:Work: Use structured interviewing. https://rework.withgoogle.com/
- Tech Interview Handbook: behavioural interviews and the STAR format. https://www.techinterviewhandbook.org/

**Problem solving**
- Pólya, G. (1945). *How to Solve It*. Princeton University Press. Understand the problem, devise a plan, carry it out, look back.
- McDowell, G. L. *Cracking the Coding Interview*. CareerCup. On thinking out loud and asking clarifying questions.

**Facts used in the question cards**
- Cormen, T. H., Leiserson, C. E., Rivest, R. L. and Stein, C. *Introduction to Algorithms* (4th ed., 2022). MIT Press. Stacks, heaps, hash tables, order-statistic trees, sorting, graph search, external sorting. (A1–A6, D3)
- Dijkstra, E. W. (1959). A note on two problems in connexion with graphs. *Numerische Mathematik*, 1, 269–271. (A3)
- Hart, P. E., Nilsson, N. J. and Raphael, B. (1968). A formal basis for the heuristic determination of minimum cost paths. *IEEE Transactions on Systems Science and Cybernetics*, 4(2), 100–107. (A3)
- Kleinberg, J. and Tardos, É. (2006). *Algorithm Design*. Pearson. Chapter 4: greedy algorithms, interval partitioning. (A5)
- Redis documentation: Sorted sets. https://redis.io/docs/latest/develop/data-types/sorted-sets/ (A2)
- Fette, I. and Melnikov, A. (2011). RFC 6455: The WebSocket Protocol. IETF. https://www.rfc-editor.org/rfc/rfc6455 (S1)
- Ellis, C. A. and Gibbs, S. J. (1989). Concurrency control in groupware systems. *ACM SIGMOD Record*, 18(2), 399–407. Operational transformation. (S4)
- Shapiro, M., Preguiça, N., Baquero, C. and Zawirski, M. (2011). Conflict-free replicated data types. *SSS 2011*, LNCS 6976, 386–400. (S4)
- MDN Web Docs: HTTP redirections. https://developer.mozilla.org/ (S5)
- Chrome DevTools documentation: Network panel. https://developer.chrome.com/docs/devtools/network (S2)
- Rubin, D. B. (1976). Inference and missing data. *Biometrika*, 63(3), 581–592. MCAR, MAR and MNAR. (D4)
- Kleppmann, M. (2017). *Designing Data-Intensive Applications*. O'Reilly. Data models, transactions, replication and partitioning. (D6)
- Fellegi, I. P. and Sunter, A. B. (1969). A theory for record linkage. *Journal of the American Statistical Association*, 64(328), 1183–1210. (D5)
- Sahami, M., Dumais, S., Heckerman, D. and Horvitz, E. (1998). A Bayesian approach to filtering junk e-mail. *AAAI-98 Workshop on Learning for Text Categorization*. (M2)
- Yosinski, J., Clune, J., Bengio, Y. and Lipson, H. (2014). How transferable are features in deep neural networks? *NeurIPS 2014*. (M1)
- Lewis, P. et al. (2020). Retrieval-augmented generation for knowledge-intensive NLP tasks. *NeurIPS 2020*. arXiv:2005.11401. (M6)
- Feathers, M. (2004). *Working Effectively with Legacy Code*. Prentice Hall. Characterisation tests. (SC2)
- Beyer, B., Jones, C., Petoff, J. and Murphy, N. R. (eds.) (2016). *Site Reliability Engineering*. O'Reilly. Managing incidents; postmortem culture. https://sre.google/sre-book/table-of-contents/ (SC3)
- Brooks, F. P. (1975). *The Mythical Man-Month*. Addison-Wesley. Brooks's law; the second-system effect. (SC4, SC5)
- Spolsky, J. (2000). Things you should never do, Part I. *Joel on Software*. Fowler, M. (2004). Strangler fig application. martinfowler.com. (SC5)
- OWASP Password Storage Cheat Sheet. https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html (SC6)
- NIST SP 800-63B: Digital Identity Guidelines, Authentication. Storing passwords as salted one-way hashes. https://pages.nist.gov/800-63-4/sp800-63b.html (SC6)
- Google Engineering Practices: How to do a code review; Courtesy. https://google.github.io/eng-practices/review/ (E4)
