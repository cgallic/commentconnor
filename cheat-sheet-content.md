# The AI Cheat Sheet
## 5 Workflows That Save People Thousands

*By Connor Gallic | commentconnor.com*

---

## Workflow 1: Insurance Denial Appeal

**The situation**: Your insurance claim got denied. The letter says "not medically necessary" or "out of network" or some other boilerplate reason. You're staring at a $2,000-$10,000 bill you shouldn't owe.

**The prompt** (paste this into ChatGPT or Claude):

```
I received an insurance denial for [PROCEDURE/SERVICE]. The denial reason
stated is: [PASTE THE EXACT DENIAL REASON FROM THE LETTER].

My policy is [POLICY TYPE — e.g., PPO, HMO, employer-sponsored] through
[INSURANCE COMPANY].

Write me a formal appeal letter that:
1. References the specific denial reason and explains why it's incorrect
2. Cites relevant medical necessity guidelines (use AMA CPT guidelines
   and the insurer's own coverage criteria if possible)
3. Includes a section requesting an external review if the internal
   appeal is denied
4. References my rights under [STATE] insurance regulations
5. Maintains a firm but professional tone

Include placeholders for my doctor's supporting documentation.
```

**What to do next**:
1. Copy the letter AI generates
2. Have your doctor add a supporting statement (most will do this if you ask)
3. Send it certified mail AND upload it to the insurer's portal
4. If denied again, request an external review — insurance companies lose these 40-60% of the time

**Why it works**: Insurance denials are designed to make you give up. Most people do. A formal appeal letter that cites specific guidelines and regulations signals you won't. The external review request is the real weapon — it costs them more to fight than to pay.

---

## Workflow 2: Performance Review Rewriter

**The situation**: Self-review season. You need to write about your accomplishments but everything you write sounds either too humble or too braggy. Your boss writes in corporate-speak. You need to match their tone.

**The prompt**:

```
Here are 3 emails/Slack messages my manager has written recently:

[PASTE 3 REAL MESSAGES FROM YOUR BOSS]

Here are my accomplishments this review period:
[LIST YOUR ACCOMPLISHMENTS — bullet points, informal is fine]

Rewrite my accomplishments in my manager's communication style.
Match their:
- Sentence structure and length
- Level of formality
- How they frame results (numbers vs. narrative)
- Vocabulary and buzzwords they actually use

Format as a self-review with 3-5 paragraphs. Include specific metrics
where I provided them. Make it sound like something my manager would
write about their best direct report.
```

**What to do next**:
1. Pull 3 recent emails or Slack messages from your boss (the more recent, the better)
2. List your wins in plain language — don't worry about sounding polished
3. Paste both into the prompt
4. Edit the output for accuracy — AI gets the tone right but might exaggerate numbers
5. Submit before your peers. First reviews set the anchor for the team.

**Why it works**: Managers unconsciously rate higher when the review "sounds right" to them. By matching their exact communication patterns, your review reads as credible and aligned. They hear their own voice reflected back.

---

## Workflow 3: Medical Billing Code Audit

**The situation**: You got a medical bill and the number looks wrong. Maybe it's $800 for a 10-minute visit. Maybe they billed for a procedure you don't remember getting. You want to verify what they actually charged.

**The prompt**:

```
I received a medical bill with the following CPT codes and charges:

[LIST EACH CODE AND AMOUNT — e.g., "99214 - $350", "36415 - $45"]

The visit was for: [DESCRIBE WHAT ACTUALLY HAPPENED — e.g., "15-minute
follow-up with my primary care doctor, blood pressure check, brief
discussion about medication"]

For each CPT code:
1. Explain what the code covers in plain English
2. Tell me the typical cost range for this code nationally
3. Flag if the code seems inappropriate for what I described
4. Identify if any codes might be "upcoded" (billed at a higher level
   than the service provided)

Also check if any codes are commonly bundled together (meaning they
shouldn't be billed separately).
```

**What to do next**:
1. Get your itemized bill (call billing and ask — they're required to provide one)
2. Run the codes through the prompt
3. If anything looks off, call billing and say: "I'd like to discuss CPT code [X]. Can you explain why this was coded as a [LEVEL] visit when the encounter was [DESCRIPTION]?"
4. If they won't adjust, file a dispute with your insurance company
5. For bills over $1,000, consider a medical billing advocate (they work on contingency — 30-50% of savings)

**Why it works**: Medical billing errors happen on roughly 80% of bills (according to Medical Billing Advocates of America). Most people never check. The CPT code system is public — anyone can look up what each code means. Asking specific questions about specific codes signals you know the system.

---

## Workflow 4: IRS Deduction Finder

**The situation**: Tax season. You know you're probably missing deductions but you don't know which ones apply to you. You don't want to pay $300+ for a CPA for a straightforward return.

**The prompt**:

```
I need to find tax deductions I might be missing. Here's my situation:

- Filing status: [single/married filing jointly/head of household]
- Employment: [W-2 employee / self-employed / both]
- Income range: [approximate — e.g., "$60K-$80K"]
- State: [your state]
- Housing: [rent / own home with mortgage / own outright]
- Major life events this year: [moved, had a kid, got married, started
  a side business, went back to school, etc.]
- Side income: [freelance, rental property, investments, etc.]
- Health: [HSA, high medical bills, etc.]

Give me a comprehensive list of deductions and credits I likely qualify
for, organized by:
1. Deductions most people in my situation miss
2. Credits that could reduce what I owe dollar-for-dollar
3. State-specific deductions for [STATE]
4. Deductions that require action before Dec 31 vs. ones I can still
   claim at filing

For each one, tell me the approximate dollar value and what
documentation I need.
```

**What to do next**:
1. Fill in the blanks honestly — the more specific you are, the better the output
2. Review the list and check off what you already claim
3. For anything new, Google "[deduction name] IRS requirements" to verify eligibility
4. If you find more than $500 in new deductions, it might be worth running them by a CPA for $150-200 (still net positive)
5. Set a calendar reminder for November to review the "action before Dec 31" items

**Why it works**: The IRS doesn't tell you what you can deduct. They publish the rules, but navigating 75,000 pages of tax code isn't realistic. AI can cross-reference your situation against the full list of deductions in seconds. The average person misses $1,000-$3,000 in legitimate deductions per year.

---

## Workflow 5: Salary Negotiation Script

**The situation**: You got a job offer (or you're asking for a raise). The number is lower than you want. You need to push back without losing the offer or burning the relationship.

**The prompt**:

```
I need a salary negotiation script. Here's the situation:

Context: [new job offer / asking current employer for a raise]
Their offer/current salary: $[AMOUNT]
My target: $[AMOUNT]
My minimum (walk-away number): $[AMOUNT]

My leverage:
- [List 2-3 specific accomplishments or qualifications]
- [Market rate data if you have it — e.g., "Glassdoor shows $X-$Y
  for this role in my city"]

Their likely objections:
- [e.g., "budget constraints", "you don't have enough experience",
  "that's above the band for this level"]

Write me:
1. An opening statement that anchors high without being aggressive
2. Responses to each likely objection
3. A "bridge" phrase for when they push back (something that
   acknowledges their constraint while holding my position)
4. A closing that creates urgency without ultimatums
5. A follow-up email template to send after the conversation

Tone: confident, collaborative, not combative. I want them to feel
like we're solving a problem together, not fighting.
```

**What to do next**:
1. Practice the opening out loud 3 times before the conversation
2. Have the objection responses written on a notepad in front of you (they can't see it on a call)
3. Never accept in the first conversation — always say "I'd like to take a day to think about this" even if you love the offer
4. If they can't move on salary, ask about: signing bonus, extra PTO, remote days, equity, title bump, review timeline
5. Send the follow-up email within 2 hours of the conversation

**Why it works**: Most people go into negotiations with a vague sense of what they want. Having specific scripts for specific objections eliminates the freeze response. The "bridge phrase" is the key — it lets you hold your position without escalating. And the 24-hour delay is powerful because it signals you have other options (even if you don't).

---

## What's Next?

**Want the full toolkit?** The Corporate Survival Kit has 30 copy/paste scripts for every corporate nightmare — delays, approvals, scope creep, meetings, boundaries, and escalation. Notion templates. $37 one-time.

**Got a specific problem?** Book a 30-min AI Audit. I solve your problem live on screen share. You leave with the finished document. $147.

Both at **commentconnor.com**

---

*Follow @connorgallic on TikTok for new workflows every week.*
