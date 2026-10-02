---
category:
  - Tech
  - Politics
tags:
  - infopolitics
  - social-software
created: 2024-08-16
collections:
  - notes
  - blog
facebook: https://www.facebook.com/jaysenn/posts/pfbid02oxfppKS4m5jemwvvAtMLCsZA4Be8bMtRzQd6t8ZjX1PRtiwcoR9iZvCrS8ZY54TCl
---
# The WhatsApp Mess

And the idea that we collectively choose to use a platform owned by something that might be much worse than just a sleazy datamining ad-company, when there are perfectly usable secure, publicly-owned platforms around - with the potential to be so much better, given the right sort of proper, open, collective direction

And that we allowed that purchase - Facebook buying WhatsApp, so obviously an anti-trust issue..

----------------
## Something, not-me responds

What you’ve written captures a frustration a lot of people share. Let me break it down a bit:

1. **WhatsApp, Facebook (Meta), and surveillance capitalism**

When [Facebook](../../wiki/Computer-Science/Software/Social%20Software/Facebook.md) bought [WhatsApp](WhatsApp) in 2014, it raised huge antitrust concerns. WhatsApp’s founders had promised strong privacy and minimal monetization, but once under Facebook ownership, the pressure to exploit user data for profit grew. That’s why your phrase “worse than a sleazy data-mining ad company” hits hard: Facebook/Meta doesn’t just monetize ads, it builds a massive behavioral profiling system that feeds into broader ecosystems of influence and surveillance.

2. **Encryption vs. platform ownership**

End-to-end encryption (E2EE) on WhatsApp does provide genuine message confidentiality. But the metadata — who you talk to, how often, when, from what device — is still visible to the company. And since the company itself is profit-driven and unaccountable to the public, that data is monetized or made available to authorities. The platform ownership undermines the trust, even if the crypto math is solid.

3. **Alternatives and collective direction**

As you point out, there are perfectly usable alternatives:

[Signal](Signal) (non-profit, open source, privacy-first).

[Matrix](Matrix)/Element (federated, open standard).

XMPP (older but still viable federated protocol).

Delta Chat (uses standard email with encryption).

The problem isn’t technical capability — it’s adoption, inertia, and network effects. A collectively owned or publicly funded platform could actually be better than WhatsApp: more transparent, governed in the open, with the public interest (not surveillance capitalism) as its north star.

4. **Antitrust angle**

You’re right to call the WhatsApp purchase an antitrust issue. Regulators largely let it through with weak conditions. Many now consider it a textbook example of “killer acquisitions” — buying out competition before it matures. If blocked, WhatsApp might have evolved into a truly independent, global privacy-first network.

---

👉 The deeper problem is that we as users often “vote” for convenience over principle. It’s not that people chose Facebook ownership; they chose to stay where their friends were. Network lock-in is powerful. But the more people voice this critique, the more pressure builds for alternatives and regulation.

Would you like me to expand on what a “publicly owned, open messaging platform” might realistically look like (governance, funding, adoption strategy)? That could flesh out the vision you hinted at.

----
## me: 
Yes

## not-me responds:
Great — let’s map out what a publicly owned, open messaging platform might realistically look like.

---
1. **Core Principles**
Public Interest First: The platform is built to serve communication needs, not advertisers or shareholders.
Openness: Source code, governance rules, and funding flows are transparent.
Interoperability: Works across devices and integrates with other open standards (email, Matrix, XMPP).
Privacy by Design: End-to-end encryption by default, with no metadata exploitation.
Resilience: Federated or decentralized so no single entity controls it all.

---
2. **Governance Models**
There are several possible structures:
Cooperative (like a credit union): Users are members and vote on decisions.
Non-Profit Foundation: Similar to how Signal Foundation runs, funded by donations and grants.
Public Utility Model: Funded like a postal service, backed by governments but with independence protections.
Federated Consortium: Universities, civil-society orgs, and municipalities run nodes collectively.
A hybrid could also work — e.g., a foundation sets standards while local co-ops/instances provide services.

---
3. **Funding Strategies**
Public subsidies (like libraries or PBS): ensures broad access.
Membership fees (small, sliding-scale, optional): users who can pay help sustain it.
Donations & grants: philanthropy and digital rights orgs (Mozilla, EFF, EU digital funds, etc.).
Service-based income: optional premium features (e.g., enterprise integration) without compromising privacy.
The key is never tying revenue to user profiling or ads.

---
4. **Technical Model**
Protocol First, App Second: Define an open standard (like email or Matrix) that anyone can implement.
Federation by Default: No central silo; people can choose servers but still communicate across the network.
Encryption + Metadata Minimization: Learn from Signal’s Sealed Sender and onion routing techniques.
Portability: Users can migrate accounts/data between providers without losing their network.
Accessible UX: WhatsApp won because it was simple. Any replacement must be just as effortless.

---
5. **Adoption Strategy**
Start Local, Scale Out: Municipalities, schools, or activist networks adopt first.
Anchor Institutions: Universities, libraries, NGOs host servers and build trust.
Policy Push: Governments can mandate open standards for official communication (like EU’s push for interoperability under the DMA).
Network Bridges: Gateways to WhatsApp/Signal/etc. for gradual migration.
Trust Branding: Make “publicly owned” a selling point — like “organic” for food.

---
6. **Challenges**
Network Effects: People won’t move unless their social graph moves. Needs momentum.
Funding Stability: Avoiding dependence on a single donor/government.
Political Capture Risk: If publicly funded, must have safeguards against surveillance or censorship.
Usability: Must feel as smooth as WhatsApp, otherwise it will fail regardless of principle.

---
✅ In short: A viable vision is a “Digital Commons Messaging Network” — built like a postal service, governed like a cooperative, funded like public media, and designed like Signal.

---
Do you want me to sketch out a concrete roadmap — e.g., what Phase 1 (pilot), Phase 2 (expansion), Phase 3 (mainstream adoption) could look like?

## me
Yes. Maybe Public funding via by projects run in GitHub repos

## Not-Me responds:
Perfect — that takes it from theory into something people can actually plug into. Using GitHub (or any open forge, even Gitea/Codeberg) means the projects themselves become visible, participatory, and fundable. It blends open-source development with public funding infrastructure.
Here’s a charter-style founding vision document draft you could use as a manifesto:

---
🌍 Charter for the Global Public Messaging Commons
1. Purpose
We believe private communication is a human right. Messaging must not be captured by surveillance capitalism, governments, or monopolies. Our mission is to create a secure, publicly funded, openly governed messaging network — a digital commons that belongs to everyone.
2. Core Principles
Openness: All protocols, software, and governance are open source and transparent.
Privacy: End-to-end encryption, metadata minimization, and user control are defaults.
Public Ownership: No shareholders. No ads. No exploitation.
Global Participation: Anyone can contribute, fork, or fund.
Interoperability: Built on open standards so people can migrate freely and avoid lock-in.
3. Governance
Foundation Backbone: Stewardship by an international non-profit foundation.
User Assembly: Participatory governance through elected user councils.
Technical Commons Council: Developers and researchers define and evolve open standards.
Regional Anchors: Universities, NGOs, and libraries host infrastructure nodes.
4. Funding Model
Open Project Funding: Each major initiative is run as a GitHub/GitLab repository with transparent roadmaps, budgets, and milestones.
Public Donations: Like Wikipedia — broad, small-scale contributions sustain the commons.
Institutional Partnerships: Schools, NGOs, and municipalities contribute modest support fees.
Grants & Foundations: Support from Mozilla, Wikimedia, Ford Foundation, EU digital rights funds, and others.
Corporate Social Responsibility: Privacy-conscious tech companies sponsor without control.
5. Development Approach
Protocol First: Define an open, federated, encrypted messaging standard.
Reference Clients: Build official apps (mobile/desktop/web) that are polished and user-friendly.
Ecosystem Growth: Encourage forks, mods, and independent clients.
Transparency by Default: All issues, discussions, and funding flows are public on GitHub.
Bridging Tools: Interoperability with WhatsApp, Signal, Matrix, XMPP to lower migration barriers.
6. Adoption Strategy
Pilot Deployments: Launch in schools, activist networks, and universities.
Anchor Partners: Collaborate with Wikimedia, Mozilla, and Access Now for credibility and reach.
Campaigns: Global calls to “fund the messaging commons,” similar to Wikimedia’s donation drives.
Recognition Seal: “Backed by the Global Messaging Commons Foundation” as a trust mark.
7. Safeguards
No Capture: Multi-source funding prevents takeover by any one entity.
No Political Control: International governance avoids state dominance.
Accountability: Annual public reports, open audits, and rotating leadership.

---
✨ In Short:
This initiative is a Wikipedia for messaging — open, globally trusted, and collectively funded. Every repository, every budget, and every line of code is public. No corporation owns it, and no government controls it.

---
Would you like me to mock up a sample GitHub repo structure (README, CONTRIBUTING, FUNDING.yml, etc.) to show how this could actually be bootstrapped as a living project?