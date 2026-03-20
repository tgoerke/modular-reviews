# Atmospheric Reviews: Modular Research as a Commons
## Full-Text Script — SFU Computing Guest Lecture 2026
### Torsten Goerke | TU Dresden / CODIP
#### Status: DRAFT v0.2

---

## SLIDE 1 — Title

Thank you for having me. I want to talk today about a problem you already know — and a set of tools and communities that are beginning to do something about it. The talk is called Atmospheric Reviews, which is the name of a project I'm part of, but really it's about a broader question: what would it look like to build research communication infrastructure as a commons rather than as a platform? I'll move through some theory, some protocol design, and some very live community work — including a working group whose third meeting happened just recently.

---

## SLIDE 2 — What If

Let me start with a provocation. What if your most-cited figure — that plot, that diagram, that visualization you spent weeks on — could be cited independently of the paper it appears in? What if a dataset you built in 2019 accrued credit every time someone reused it, regardless of which platform they found it on? What if your community — your specific research community, with its specific standards and norms — got to define what peer review means for your discipline, rather than having that definition handed down by a journal?

And here is a fourth question, less obvious but equally important: what if you had the vocabulary to describe what you actually produce? Research is not only papers and datasets. It includes artistic practices, co-creation processes, cultural work, and forms of knowledge-making that current research platforms have no affordances for — not because they are not legitimate research, but because the platforms were built around a narrow model of what research looks like. When a system can only offer you the actions "submit," "review," "publish," and "cite," it implicitly defines what counts as research. The vocabulary gap is not incidental — it is structural. And it connects directly to something we will return to: the difference between selecting from a platform's menu and specifying your own affordances.

A researcher in a working group I participate in put it this way: "We need a seamless formal research environment — a standard protocol for easily modular publishing — with outputs interoperable across platforms." That is not a wish list. That is a specification. The infrastructure to build it already exists. This talk is about how we hatch it — a term I'll come back to.

---

## SLIDE 3 — From Albums to Streams

Courtney Babott and Rowan Cockett, who will be keynoting ATScience 2026 in Vancouver in just a few days, have written something clarifying. They argue that scientific publishing is under growing strain — not because science is broken, but because the infrastructure bundling it together was built for a different era. The PDF bundles research the way albums bundled music: text, figures, data, methods, citations, all wrapped into one artifact, one citation, one locus of credit. Music did not change because audiences suddenly wanted playlists. It changed because digital infrastructure made it possible to break apart bundled products, reconnect them in new ways, and move value through use rather than control.

The same transition is underway in research. Modular research outputs — reproducible notebooks, scientific figures, tables, datasets, methods, code — can now each be independently shareable, citable, and reusable. The question is not whether this transition will happen. It is how it will be shaped, and by whom. The ecosystem is already forming. ATScience 2026 projects include Chive for decentralized eprints, Margin.at and Seams.so for social annotation, Lanyards for portable researcher profiles, Semble as a social knowledge network, Paper Skygest Feed for personalized research discovery, Groundmist for Obsidian integration with ATProto, Astrosky for astronomy, and Hypgen Infinity for evaluating scientific AI agents. These are not prototypes — they are live projects building on a shared protocol substrate.

---

## SLIDE 4 — POSIWID

To understand why we are in the situation we are in, I want to borrow a principle from cybernetics, surfaced recently by Larens Hof in his essay "The Purpose of Protocols." The principle comes from Stafford Beer: the purpose of a system is what it does — not what its designers intended, not what its mission statement says, but what it actually produces in the world.

Applied to the protocols that built the internet, this is sobering. SMTP, HTTP, RSS — these protocols claimed to be neutral infrastructure. Their silence on questions of governance, ownership, and power was presented as a feature, a kind of principled non-interference. But silence on governance is not neutrality. It is a choice, and the outcomes of that choice are now legible: concentration of authority, platform lock-in, the passive user who consumes rather than governs. When we apply this lens to research communication, the picture is uncomfortable but clear. Journal systems claim to disseminate knowledge; the outcome is subscription lock-in and copyright transfer. Preprint servers claim to enable open access; the outcome tends toward single-platform indexing monopolies. Citation indexes claim to track impact; the outcome is commercialized metrics and opaque algorithms. The purpose of these systems is what they do.

---

## SLIDE 5 — The Governance Vacuum in Research

The pattern that produces these outcomes has a name in platform studies: enshittification. It describes how platform quality degrades over time as users lose alternatives — the lock-in that precedes extraction. Research platforms follow identical topology: proprietary infrastructure, opaque algorithms, and the steady extraction of value from community labor. Researchers produce the papers, do the peer review, sit on editorial boards, and generate the citations — and the value created by that labor accrues to platforms they do not govern.

Hof makes a pointed observation: protocol design can constrain how actors operate within a system, but it cannot ensure the conditions that keep the broader ecosystem functioning. The governance mechanisms required to sustain a commons — what Elinor Ostrom identified as defined community boundaries, collective choice mechanisms, accessible conflict resolution, and proportional cost-benefit distribution — are absent from every major research infrastructure we currently use. This is the governance vacuum. It is not an oversight. It is structural. And it is the condition that a commons-based approach to research infrastructure must deliberately address from the very start.

---

## SLIDE 6 — The User/Developer Dualism

There is a deeper problem beneath the governance vacuum, and it is worth naming precisely. The dominant topology of research platforms does not merely extract value — it constructs researchers as passive consumers. The affordances available to researchers on current platforms are set and fixed: submit, cite, download, share. These actions were designed for an undifferentiated "everyone" — a fiction of a universal user that serves no actual research community particularly well.

What researchers cannot do on these platforms is specify: they cannot define what counts as a contribution in their discipline, cannot determine how credit should flow to figures or datasets or methods, cannot decide what peer review means for their community's standards. This user/developer dualism has two specific consequences I want to name. First, the process is lost: AI tools optimized for task completion deliver outputs rather than understanding, and the cognitive work of research — the reasoning, the uncertainty, the situated judgment — is increasingly outsourced. Second, the literacy is lost: the capacity to carry out peer review, to evaluate evidence, to situate claims within a field. When the process is automated away, so is the practice that makes the process meaningful. The latest manifestation of this dualism is AI-assisted vibe coding — a pattern we will return to.

---

## SLIDE 7 — Protocols: Hard to Study, Easy to Ignore

Venkatesh Rao and colleagues, writing in the Summer of Protocols research program, describe protocols as "hard to study and easy to ignore." This is apt. Protocols are the connective tissue of digital infrastructure — they govern how systems communicate, how data moves, how identities are established — and precisely because they work when they are invisible, we rarely interrogate them.

There are at least three theoretical traditions that help us understand what protocols actually do. Actor-Network Theory, developed by Latour and Callon among others, treats protocols as bridges between ontologies — they connect the engineering world of objects, functions, and interfaces with the social world of power, identity, and norms. This is not a smooth translation; it is a negotiation, and what gets encoded in a protocol reflects the assumptions and power relations present in that negotiation. The concept of assemblages, developed by Deleuze and Guattari, adds that communities and technologies have emergent properties that only come into being when they become part of a larger configuration — protocols enable the connections through which these emergent properties arise. And from cybernetics, Wiener's framework reminds us that protocols are fundamentally about governance: the science of communication within and governance of, by, and for networks.

---

## SLIDE 8 — The Governance Ladder

If we arrange the major open protocols along a spectrum of normative explicitness — how much they say about governance, rights, and power — a ladder emerges. Early protocols like SMTP, HTTP, and RSS were almost entirely silent on these questions. Their silence was not neutral: it enabled the mimetic convergence that produces monopolies, as users copy successful choices and infrastructure concentrates around dominant providers.

ActivityPub, which powers Mastodon and the broader Fediverse, was more explicit. It was designed with decentralization as a stated goal, and its federated architecture does distribute control across instances. But it recreates platform dynamics at the instance level: governance defaults to administrator discretion, and there are no formal mechanisms for accountability, appeal, or collective decision-making across the network. AT Protocol, which powers Bluesky, is the most normatively explicit of the current generation. Its design documentation states that "speech and reach should be two separate layers" — a meaningful commitment to separating what you publish from who amplifies it. Yet Bluesky itself dominates the ATProto ecosystem, and the shared infrastructure faces the same governance vacuum that Hof identifies across the protocol landscape. As Hof puts it: protocol architecture shapes which governance mechanisms are natural, but it cannot enforce them.

---

## SLIDE 9 — Hatching: Initializing the Commons

This is where the concept of hatching becomes essential. The term comes from the Commons Stack, and it addresses exactly the gap the governance ladder reveals: protocols can create the conditions for democratic governance, but they cannot initialize it. Someone — or some community — must do the initializing work deliberately and participatorily.

The concept is precise: engineering any complex system is a consideration of its initialization conditions. In a Commons, these initial conditions are the Hatch. Hatching is not simply building — it is co-constructing topology and governance simultaneously, rather than layering democracy onto infrastructure that has already been built with different assumptions embedded. It shapes what we call the governor-engineer role: a practice of translating social frameworks into actionable technical steps, grounded in interdisciplinary work between engineering and social science. This unfolds through a five-step governance pipeline: identifying the initial conditions, establishing new roles, applying technical knowledge in the service of governance, shifting focus to empowering users to describe and specify their own systems, and implementing deliberative practice as an ongoing feature of the commons rather than a one-time design decision.

---

## SLIDE 10 — Why ATScience

ATScience — atproto.science — is a community and movement co-founded by Ronen Tamari, myself, and Barry Prendergast. Its mission is to empower science communities with open, democratic, researcher-owned infrastructure. We chose AT Protocol as the substrate for this work for four specific reasons. Sovereign identity: on ATProto, your identity is anchored to a cryptographic DID that you control — it is not owned by a publisher, a platform, or an institution. Portable data: your research objects, your posts, your annotations, your relationships travel with you across services, with provenance intact. Speech/reach separation: what you publish is architecturally distinct from who amplifies it, which means communities can govern their own discovery and curation layers. And credible exit: the structural condition that makes community self-determination real rather than rhetorical — you can leave any service without losing your data or your network.

ATScience 2026 takes place on March 27 in Vancouver as a full-day exploration of AT Protocol applications in science, education, and open knowledge. More than ten projects are already building on this substrate. The hatch is in progress.

---

## SLIDE 11 — Atmospheric Reviews: The Hatch in Progress

Atmospheric Reviews is the specific application of the hatching framework to research communication on AT Protocol. Applying the hatching process cycle to research means working through four phases. The first is enabling deliberation: asking, concretely, what affordances this research community needs. The second is algorithmic choice: building community-governed discovery and curation, where the algorithms that surface research are specified by and accountable to the community. The third is sovereign identity: ensuring researcher identity is genuinely portable and independent of any publisher or platform. The fourth is implementing rules at the protocol level — encoding governance not as a policy document, but as a structural feature of how the system works.

Atmospheric Reviews treats modular research objects as first-class protocol citizens. A figure, a dataset, a method, a panel of evidence — each is an addressable object with its own identity, its own license, its own provenance trail. Review, curation, and annotation become specifiable community affordances rather than platform defaults. And critically, the governance conditions are being set now, before concentration occurs — before any single provider dominates the infrastructure, before the governance vacuum opens.

---

## SLIDE 12 — From Select to Specify

This brings me to what I consider the central distinction of this talk. Current research platforms offer researchers a fixed menu of actions: submit, review, publish, cite, download. These actions were designed for everyone and therefore serve no one particularly well. A genomics lab, a humanities scholar, a clinical trial team, and a computational social scientist all get the same affordances — the same definition of "review," the same model of "contribution," the same citation structure — regardless of whether those affordances fit their practice.

What AT Protocol and the commons approach affords is something different: the capacity to specify rather than select. To specify is to define what counts as a contribution in your discipline, to determine how credit flows — to the figure, the dataset, the method, not just the paper — to decide what review means for your community's standards, and to set the conditions under which reuse is permitted and attribution required. This also means having the vocabulary to name what you produce: artistic practices, co-creation, cultural work — forms of research that current platforms cannot describe because they were never designed for them. This is what I mean by Information Civics: treating network architecture as civic design. The question is not what algorithms can do for researchers. It is what kinds of collective futures research communities want to build — and with what authority they want to build them.

---

## SLIDE 13 — Reuse Incentive Working Group

I want to spend time now on live community work, because I think it demonstrates something important: the intellectual and practical work of building a research commons is already happening, in deliberate and sophisticated ways, among the communities who will inhabit it.

The Reuse Incentive Working Group is co-led by Creative Commons and the Continuous Science Foundation. It brings together approximately thirty members — researchers, librarians, publishers, funders, technologists, infrastructure builders — from institutions across the world. I am one of them, and I am speaking from that position. The group has been meeting since February 2026, with a third meeting just recently. Its goal is to surface the points of friction around reuse and licensing of modular research, to explore how licensing serves as both a technical and cultural enabler of reuse, and to produce a framework and recommendations for modular science reuse. The framing question the group opened with is worth sitting with: reuse is still treated as optional or downstream in current research infrastructure. What would it look like to treat reuse — and the permission to reuse — as core infrastructure for how science is shared?

---

## SLIDE 14 — What Does Modular Research Actually Need?

Through structured breakout discussions across three groups, the WG surfaced twelve distinct friction areas, organized into four clusters. The first concerns publishing for reuse: researchers need to know whether and how they can reuse a component as a primary source; they need to know whether and how they can license their own components; and they need clear guidance on what proper licensing actually requires. These are not exotic edge cases — they are the friction researchers encounter every time they try to work with someone else's figure or share their own dataset.

The second cluster concerns attribution expectations: authors need to track the attribution and credit they receive at the level of individual components — per figure, per panel of evidence, per paper repo — and to distinguish citations received for primary versus secondary sources. The third cluster concerns reuser guidance: knowing what a license requires, being able to comply with it easily, and tracking whether you have done so. The fourth and most structurally significant cluster concerns what the WG called thinking outside the PDF: preventing the gaming of citation metrics, establishing a standard protocol for modular publishing with outputs that are interoperable across platforms, and ensuring that attribution mechanisms work not just in formal publication contexts but during the informal sharing — on Slack, on social media, at conference talks — where much of actual science communication happens.

---

## SLIDE 15 — Citation as Currency

One tension the working group named with particular clarity is worth dwelling on. Citation as currency is the operating logic of current research evaluation: your work's value is measured by how many times others cite it. But citations have no sentiment. A citation that supports your claim, a citation that refutes it, a citation that merely notes your existence as prior work — all count equally. This creates a well-known gaming problem, and the working group named it explicitly: if reuse is tied to citation, and citation is currency, then systems designed to maximize citation will be gamed.

What modular research requires instead is attribution that propagates downward — to sub-components, figures, datasets, methods — and credit that travels across platforms rather than being locked to a single index. The TASLAR metadata standard — Title, Author, Source Link, License Link, Attribution Statement, Rights Statement — is an approach to embedding this at the object level, so that trust and permission travel together with the research object itself. The aspiration named in the working group is precise: machine automation of attribution as a cultural norm, not just a legal requirement. The goal is to make proper attribution the easy thing by encoding it into the infrastructure.

---

## SLIDE 16 — AIDLE: A Research Agenda

I want to close the substantive part of this talk with a provocation and a research agenda. There is a remaining gap in the picture I have been painting: the governor-engineer role — the capacity to co-construct topology and governance simultaneously — requires both technical and governance literacy. That intersection is rare. And AI tools, as currently designed, are making it rarer.

The dialectic is worth stating clearly. The thesis: AI-assisted vibe coding is the latest manifestation of the user/developer dualism — it optimizes for outputs, not understanding, and produces fluency illusions and metacognition bypass at scale. The antithesis: hatching a commons, the deliberate co-construction of communities that specify their own affordances. The synthesis — which is the research agenda I am working toward under the name AIDLE, at CODIP — is the design of AI systems that optimize for human capability development rather than task completion. AI that knows when not to answer. AI that scaffolds co-design rather than completing it. The Atmospheric Reviews project is the testbed: agentic tools that help research communities specify their own protocol affordances, rather than accepting the defaults. This is not a product. It is a direction for what AI research, in the context of open science, should become.

---

## SLIDE 17 — Protocol-Mediated Agency

The PDF bundled research the way albums bundled music. AT Protocol gives us the infrastructure to unbundle — and to re-bundle on community terms. Protocol-mediated agency means communities that specify their affordances rather than selecting from a platform's menu, governance that is initialized before concentration occurs, and researchers who hold their identity, their data, and their relationships across any service they choose to use.

The work is underway. The Reuse Incentive Working Group is mapping the friction. ATScience brings together the builders on March 27. Atmospheric Reviews is initializing the commons. AIDLE is asking what AI systems should be designed to do. These are not separate projects — they are facets of the same question, which I will leave with you:

*What affordances does your research community need to specify — and who currently decides?*

---

## REFERENCES

- Rao, V. et al. (2023). *The Unreasonable Sufficiency of Protocols.* Summer of Protocols.
- Hof, L. (2026). *The Purpose of Protocols.* Connected Places. https://connectedplaces.online/the-purpose-of-protocols/
- Goerke, T. & Barthold, S. (2025). *Democracy by Default — Hatching a Commons for Digital Deliberation.* Weizenbaum Conference 2025.
- Goerke, T. & Barthold, S. (2026). *Information Civics as Counter-Imaginary.* Socializing Algorithms Conference submission.
- Babott, C. & Cockett, R. (2026). *From Albums to Streams: How Modularity Changes Systems.* https://doi.org/10.62329/phrt5367
- Akamatsu, M. (2025). *The Modular Paper Repo.* [Figure].
- Commons Stack. (2021). *What's In a Hatch?* Medium.
- Zhang, G.Z. (2025). *The Critical Legacy of Chinese Cybernetics.* Combinations.
- Reuse Incentive Working Group. (2026). Meeting notes, Feb–March 2026. Creative Commons / Continuous Science Foundation.
- ATScience. (2026). atproto.science.
