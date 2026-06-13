---
title: "A Kill Switch Is Not the Answer"
description: "Why a sudden state-mandated blockade of AI models exposes the gap between technical safety, the power of a kill switch, and true accountability."
date: 2026-06-13
tags:
  - ai
  - alignment
  - governance
  - safety
  - accountability
type: note
lang: en
---

To me, this case is interesting not because of the dispute surrounding a specific model, but as a textbook example of a deeper issue: the technical safety of a system and its fundamental alignment are far from the same thing.

Today, news broke that access to two next-generation language models—Fable and Mythos—was suddenly and severely restricted. According to the company's public statement, the US government demanded that access to these neural networks be shut off for all foreign citizens, even including the developer’s own overseas employees. Since I am a citizen of Kazakhstan, this directive hit me directly: overnight, I lost access to my working tools. However, to execute the order quickly and reliably, the company took the most radical path and simply cut off access for all users entirely.

Judging by the published version of events, the catalyst for these drastic measures was the discovery of a way to bypass Fable's safety filters. The company insists this is not a comprehensive vulnerability, but rather a highly specific and narrow exploit. Furthermore, they argue that the consequences of this bypass are not unique—a comparable effect could allegedly be achieved using other systems already available on the market (in particular, the developers point fingers at gpt-5.5).

It is important to understand: this is the most detailed public account we've had of such an incident, which is precisely why it shouldn't be taken as an objective picture of reality. Usually, things are left unsaid. For instance, unlike Mythos, gpt-5.5 was never positioned as a cybersecurity model. For those purposes, OpenAI maintains a separate family of entirely closed models—Cyber—available exclusively to enterprise clients. Therefore, these direct public comparisons seem disingenuous at best.

I will not presume to judge who is technically right here. And this is worth stating upfront. It is entirely possible that the NSA has classified intelligence and compelling reasons hidden from the broader public. It is also possible that the company is underestimating the real risks. Or perhaps, as is often the case, security personnel have bought into yet another conspiracy theory or a spy thriller titled "AGI 2027"—and are now, foaming at the mouth with zeal, pulling the emergency brake for nothing.

For me, only one very cautious conclusion follows from this story: as outside observers, we are currently physically unable to assess the adequacy of the measures taken. Any harsh declarations about a fundamental defect in the entire control system remain mere guesswork—because we do not know what verification mechanisms are operating behind tightly closed doors.

## The Problem is Broader Than the Model

When we discuss artificial intelligence safety, our gaze involuntarily focuses on the neural network itself. What can it do? What safeguards are hardcoded into it? How easy are they to break? How was it tested? What does it output in response to dangerous prompts?

These are, of course, critical questions. Without them, any discussion devolves into populism. If a system is truly capable of causing massive harm, this cannot be justified by appeals to free speech, the free market, or mere convenience.

But today's incident highlights a different dimension. Even if the technical specifications are critically important, the fate of the system is no longer decided within its source code. The decision is made within a complex social web: involving the developer company, government agencies, users, rank-and-file employees, state secrets, emergency directives, legal liability, mass blackouts, and—only after the fact—smoothed-over press releases.

It is no longer the model acting here. It is a complex sociotechnical system.

## A Kill Switch is Not a Solution

The state undoubtedly must have the right to pull the "emergency brake" to halt the dangerous deployment of a powerful technology. I am by no means an advocate for a world where corporations can unleash whatever they want with impunity, leaving society to merely watch and blindly trust internal audits.

But the mere existence of a kill switch is not yet a transparent and accountable procedure.

For such actions to inspire trust, there must be at least a baseline level of transparency. For me, that begins with four simple questions:

1. What exactly went wrong? We need to understand at least the general risk category so the subject of the dispute is clear.
2. Why was a total shutdown necessary? Society must see that the emergency measure is not simply bureaucratic arbitrariness.
3. Why are similar sanctions not applied to comparable competitor systems? It is important to know whether we are dealing with consistent policy, an ad-hoc exception, or at the very least, traces of lobbying.
4. How can this decision be verified, challenged, or reviewed? Even if a full release of classified data is impossible, there must be a legal avenue for appeal.

If even this minimum is unmet, then to the outside observer, the government's "emergency brake" transforms into a black box. Yes, in a critical situation it might save the day, but it adds no trust to the system. On the contrary, it erodes trust precisely where it was supposed to serve as a guarantor.

An opaque regulator with an "off" button, pushing it at random moments and unburdened by accountability, is not alignment. It is simply the introduction of another major player onto the field, whose actions may fundamentally conflict with the public good (and most likely will). Essentially, it is just adding another non-trivial variable to the already complex alignment equation.

## Where the Correction Mechanism Breaks Down

Let us look at the company's argument. They say: we tested the defenses in advance, invited external auditors and government agencies, built defense-in-depth, never promised 100% invulnerability, and consider the discovered breach to be quite minor.

From the government's side (as far as anything leaks to the press), there are far fewer arguments. We hear only boilerplate phrases about "national security" and demands to cut off access for foreigners. We do not see a detailed justification—though this does not mean one does not exist behind closed doors.

And this is where the main fault line lies. The company has a polished public narrative about safety, but it also has an obvious commercial interest in protecting its product. The state has the power to ban this product, but from the outside, there is no evidence visible that would allow us to distinguish a truly necessary measure from banal over-insurance or a bureaucratic blunder.

My complaint here is not about the secrecy of the decision itself. The problem is that in the public sphere, there are absolutely no visible mechanisms that could verify, balance, or limit this secret component.

In a healthy system, there must be a bridge between these extremes. No one is demanding that bomb blueprints be published on the front page. But there needs to be a clear procedure: with a strict threshold for activation, an expiration date for emergency measures, an independent debriefing, and an avenue for reviewing the decision.

Such oversight does not necessarily have to be public. It could be a court, a special parliamentary committee, or an independent oversight body with appropriate security clearances—any structure capable of providing real, verifiable accountability.

Without this, any state action looks less like a functioning error-correction mechanism and more like a simple shout from the boss.

A shout might temporarily reduce risks. But it does not answer the ultimate question: how exactly do we, as a society, plan to govern these technologies in the future?

## Safety Must Not Subsume Alignment

This incident vividly illustrates the trap of oversimplified language. If everything is reduced to "model safety," then a profoundly complex problem is compressed into a primitive algorithm: "found a dangerous bypass — shut it down; didn't find one — let it run."

This is, of course, an exaggerated schematic, but it is precisely what public debates often devolve into.

The reality is far more complicated. The real question is different: who is empowered to translate a strictly technical signal into massive social consequences? Who has access to the evidence? Who pays the cost of an error? Who has the right to demand explanations and initiate a review? What happens if the emergency measure turns out to be wrong, excessive, or politically motivated?

Technical safety is a foundational, absolutely indispensable layer. But it must not quietly subsume the entire complex conversation about the social alignment of technology.

True alignment requires more than just safe algorithms. It requires clear, contestable, and transparent rules of the game by which decisions about the fate of those algorithms are made.

## How It Should Be In an Ideal World

I am far from thinking that the state should be forbidden from intervening. That is too primitive an answer to an extremely complex challenge.

In my view, this case organically suggests a set of governance standards that ought to be codified:

- Emergency system shutdowns are only permissible upon confirmation of a severe risk.
- The grounds for a shutdown must be clearly classified and verifiable.
- Any emergency measure must have an expiration date or a transparent renewal procedure.
- The incident must undergo an independent technical audit.
- There must be a public explanation of why similar measures have not been applied to comparable products on the market.
- The developer must have a legal right to challenge the decision.
- Society must receive the maximum amount of public information about the incident—exactly as much as common sense and genuine safety will allow.

Not all of these points are a direct reaction to the current scandal. Rather, they are an attempt to formulate general principles for the future to close obvious gaps in accountability.

If we do not do this, we will build a system where neural networks can be switched off with a single click, but that "power of the kill switch" itself can neither be controlled nor limited.

And therein lies the core paradox: a mechanism designed to correct errors itself becomes the primary source of chaos and misalignment.

## Conclusion

The hardest question here is not whether the state has the right to an emergency blockade of dangerous AI. It absolutely does: in critical situations, such power is vitally necessary.

The difficulty lies elsewhere: does this "kill switch" itself remain transparent, justified, and accountable to society?

If not, then we have not solved the alignment problem. We have simply invited another powerful player to the table, one who now needs to be asked the same uncomfortable questions: who is watching you? Who can object to you? Who will pay for your mistakes? And how exactly can we stop you if you go too far?
