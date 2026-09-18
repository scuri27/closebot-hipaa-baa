# closebot hipaa: What the Growth Plan Includes, What a BAA Actually Covers, and Whether It Fits Your Practice

If you typed "closebot hipaa" into a search bar, you're probably standing at one of two doors. Either you run a clinic, dental office, med spa, or a healthcare marketing agency and got told the CRM chatbot "can't touch PHI" — or you're already using CloseBot and just found out the compliance part sits behind a plan you can't buy from the pricing page.

Both questions have concrete answers, and neither one is "yes, it's all HIPAA compliant, don't worry." CloseBot's HIPAA story is narrower than the homepage comparison table suggests, and the details matter if a patient's name, condition, or appointment reason is going to flow through a text conversation.

Here's what's actually confirmed, what it costs, and where the edges are.

## The short version

CloseBot is HIPAA compliant, but only on the **Growth plan**, which is custom-priced and sold through sales rather than self-serve checkout. There are signed BAAs on file, compliance work runs through Anthropic as the AI provider, and CloseBot doesn't let you bring your own API key. If you're on Free or Core, you are not covered — and that's a design choice, not an upsell accident.

That's the whole shape of it. The rest of this article is about whether the shape fits your situation.

## What "HIPAA compliant" means on CloseBot specifically

The word gets thrown around loosely, so it's worth separating what CloseBot states from what it doesn't.

**Compliance lives on one plan.** The healthcare page is direct about it: HIPAA is available on Growth plans only, and the plans page puts "HIPAA compliant" in the Growth feature list alongside quarterly audits, 99.99% priority uptime, and priority support. HIPAA isn't an add-on you can bolt onto a Core subscription.

**BAAs are in place.** CloseBot states that signed BAAs are on file, with third-party BAAs covering the vendors in the chain. Details sit in their Trust Center, which runs on Vanta — that's where you'd point your own compliance officer or legal reviewer instead of taking a marketing page at its word.

**The AI provider is locked.** Their help docs say CloseBot is currently HIPAA compliant with Anthropic, so HIPAA accounts are pushed to that provider for all messages and agent processing. You don't get to pick Gemini or OpenAI on a HIPAA account. If you already have opinions about which model handles patient conversations, that opinion is now a constraint to work around, not a preference.

**No bring-your-own-key.** CloseBot won't let you plug in your own OpenAI or Anthropic key, and explains it as a security decision. Their own blog goes further and argues that any system requiring your own API key isn't HIPAA compliant, since you'd be the one holding the compliance relationship with the model provider. That's CloseBot's position rather than a regulator's ruling, but it's consistent with how their product is built.

**PHI stays inside your CRM's channels.** Per the healthcare page and the homepage FAQ, conversations happen in the text channels your CRM already uses — HighLevel, HubSpot, custom systems — or through CloseBot's standalone HIPAA-compliant chat widget if you don't have a CRM wiring it up. CloseBot also states it does not train AI on your data.

One more detail from the healthcare page worth knowing: CloseBot says support staff with account access are trained in data protection and background-checked within the US.

> The practical takeaway: "CloseBot is HIPAA compliant" is true only when the account is on Growth and the agents are routed through Anthropic. On any other plan, you're running a general-purpose sales AI that happens to be excellent at booking appointments.

## Do you actually need the Growth plan?

Not every healthcare-adjacent business does. The line is whether identifiable patient information enters the conversation — not whether you sell to clinics.

You likely need a BAA on file if:

- The agent asks for or receives patient names, dates of birth, insurance details, symptoms, or treatment interests
- You're booking consultations inside a specialty where the appointment reason itself is health data (implants, fertility, med spa treatments, chiropractic, behavioral health)
- Your intake flow collects anything a patient would consider private before they've signed anything

You probably don't need it if:

- The agent only handles scheduling for non-clinical services like gym memberships or general wellness retail
- Conversations stay at the "what time works for you" level with no health context
- You're routing everything to a human before any detail gets collected

CloseBot's healthcare page frames the use case as scheduling, intake, and follow-up — which is exactly the part of the funnel where PHI shows up fastest. A patient opening with "I've been missing a tooth for a while" has already told you something clinical, and that happens in the first message, before any form exists.

## The full plan lineup, and where HIPAA sits

Here's the current structure from CloseBot's plans page. HIPAA appears in one row, and that row has no number on it.

| Plan | Best for | Core inclusions | Price | Billing | Purchase |
| --- | --- | --- | --- | --- | --- |
| Free | Testing CloseBot or very low lead volume | 100 messages/mo, 1 agent, 1 user seat, 1 MB storage, unlimited account connections | $0 | Always free | [ Start on the CloseBot free plan](https://app.closebot.com/a?fpr=li87) |
| Core (Business) | Businesses automating their own lead qualification | 500 messages included at base, message costs bundled into the price, 15+ templates, human support, add-on users at $5/seat, additional agents and storage available | $64/mo monthly, or $53/mo billed annually as $640/yr | Month to month, or annual | [ Check CloseBot Business plan pricing](https://app.closebot.com/a?fpr=li87) |
| Core (Agency) | Agencies building and rebilling AI setters for clients | Unlimited agents, white-label client portal, rebill all costs including messages, invite additional users | $397/mo monthly, or about $331/mo on annual billing | Month to month, or annual | [ See the CloseBot Agency plan](https://app.closebot.com/a?fpr=li87) |
| Growth | Regulated and high-volume operations needing SLAs and compliance | HIPAA compliant, quarterly audits, 99.99% priority uptime, priority support, 50+ templates, "unlimited potential" | Custom — quoted through sales | Custom | [ Request a Growth plan trial from CloseBot sales](https://app.closebot.com/a?fpr=li87) |

A few notes on that table, because the numbers are less straightforward than they look.

Annual billing unlocks the larger template library — 50+ templates versus 15+ — so the cheaper monthly figure comes with a feature difference, not just a discount. CloseBot describes the annual cadence as effectively ten months for twelve.

The Business track scales with message volume, so $64/mo is the entry point for 500 messages rather than the price for a busy practice. Extra storage runs from $0.10 to $3.00 per MB per month depending on how much you need, and additional user seats are $5 each.

There's also a documentation gap you should know about before you talk to sales. CloseBot's help center still lists Business pricing as $64 for 1 job flow, $197 for 3, $297 for 10, and $397 for unlimited — a structure that doesn't match the current plans page, which prices by message volume instead. Treat the plans page as current and ask sales to confirm which model your account will be billed on.

The Agency per-message rate has the same issue: the plans page says agencies are billed a flat $0.012 per message that can be rebilled, while the help docs describe paying $0.006 per message plus markup. Worth clarifying in writing if you're modeling margins.

## What the Growth plan adds besides the BAA

Compliance is the headline, but Growth bundles things a clinic actually feels.

**Quarterly audits.** Useful if your own risk assessment cycle needs documentation, and far more useful than a badge if you're ever asked to show your work.

**99.99% priority uptime and priority support.** For a practice where a dropped chatbot means after-hours calls going unanswered, support priority is a real operational difference rather than a line item.

**"Unlimited potential."** That phrasing maps to the Agent Node configuration in CloseBot's docs — you can add many tools and unlimited instruction size, but billing shifts from per-message segments to token costs. The upside is a more capable agent; the downside is that cost predictability gets fuzzier. Budget conservatively if you plan to run heavy agents.

**50+ templates.** Helpful when you're standing up agents for multiple locations or specialties rather than one clinic.

What Growth does not change: channel coverage. CloseBot is text-based — SMS, website chat, email through the CRM. There's no voice agent in the product. If patients call the front desk, that's still a human or a separate voice platform.

## Getting HIPAA switched on: the practical path

There's no self-serve button for this. The steps are:

1. **Run the free plan first** to see whether the conversation quality actually holds up on your patient scenarios. It costs nothing and caps at 100 messages, which is enough to see how the agent handles a nervous first message.
2. **Contact sales for a Growth trial.** CloseBot's healthcare page explicitly directs you to set up a free trial of the Growth plan through sales. That's where the BAA conversation starts, and it's also where you'd confirm pricing.
3. **Get the BAA executed before any real patient conversation happens.** This is the step people skip. A trial with real patient data before paperwork exists is the worst possible version of this process.
4. **Confirm the Anthropic routing** on your agents once the HIPAA account is live, since that's the provider CloseBot pushes HIPAA accounts toward.

CloseBot is clear that there are no refunds, but there is a real trial on any paid plan plus a free-forever tier under 100 messages. Plans run month to month with no contract, so testing the setup and walking away is genuinely possible.

## Three things to verify before you rely on it

**Identity verification is on you.** A chatbot that will discuss an appointment with anyone who types a patient's name is a problem regardless of how good its BAA coverage is. This comes up constantly in health IT discussion — the compliance paperwork can be flawless while the conversation itself hands out information to the wrong person. CloseBot lets you build custom tools and conversational guardrails, so verification questions are something you configure, not something that comes pre-solved.

**Total cost includes more than CloseBot.** If you're wiring this through GoHighLevel or HubSpot, that subscription sits underneath. A practice wanting roughly 1,000 messages a month is paying for CloseBot plus a CRM tier, before any agency service fees on top.

**Vendor numbers are vendor numbers.** CloseBot advertises 1M+ booked appointments, around 150,000 daily messages, and 99.99% uptime. Those aren't audited figures — they're the company's own claims. They're consistent with a mature product, but build your expectations on the trial, not the homepage counters.

## Who this actually fits

If you're a dental office, med spa, chiropractic clinic, or private practice that gets leads through forms, ads, and SMS — and you want those leads qualified and booked without a front-desk person triaging texts at 9pm — Growth is the only plan you can legally run that on, and the pricing is a conversation rather than a checkout page.

If you're an agency serving healthcare clients, the interesting combination is the Agency plan for the rebilling and white-label layer. But HIPAA still requires Growth, and CloseBot hasn't published how those two stack. That's a question for sales, and it's worth asking before you promise a client anything about compliance.

If your volume is genuinely low — a few dozen conversations a month, mostly handled by staff — the free plan plus a human is not a compliance failure. It's just a smaller operation, and there's no requirement to automate it.

The honest framing: CloseBot treats HIPAA as an enterprise feature with enterprise paperwork attached, and prices it that way. Whether that's reasonable depends entirely on how much identifiable patient information your conversations touch. Figure that out first, then go get the quote — [👉 get started with CloseBot here](https://app.closebot.com/a?fpr=li87) if you want to see the agent quality on the free plan before you talk pricing.

## FAQ

**Is CloseBot HIPAA compliant on the free plan?**
No. HIPAA is available on Growth plans only, per CloseBot's own healthcare page. Free and Core plans are not covered, regardless of how you configure the agents.

**How much does the HIPAA-compliant Growth plan cost?**
Pricing is custom and quoted through sales. CloseBot doesn't publish a number, and the plan is aimed at operations needing SLAs, compliance, quarterly audits, or high volume.

**Does CloseBot sign a BAA?**
Yes. The healthcare page states signed BAAs are on file with third-party BAAs in place, and points to a Vanta-hosted Trust Center for the details.

**Which AI model handles HIPAA conversations?**
Anthropic. CloseBot's docs state that HIPAA accounts are pushed to Anthropic for all messages and agent processing, and you don't choose the provider on that account type.

**Can I bring my own API key to lower costs?**
No. CloseBot disallows bring-your-own-key and describes it as a security measure. Your model spend is part of the plan.

**Does CloseBot work without a CRM?**
Yes — there's a standalone HIPAA-compliant chat widget for website use if you're not routing through HighLevel, HubSpot, or a custom system.

**Is there a free trial of the Growth plan?**
CloseBot offers a 7-day trial on paid plans, and the healthcare page tells you to contact sales to set up a free trial of the Growth plan. There are no refunds after billing starts, so the trial is where you do your testing.
