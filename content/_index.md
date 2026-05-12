---
title: "Atmospheric Reviews"
date: 2026-05-12
type: landing

sections:
  - block: dev-hero
    content:
      username: torsten-goerke
      title: "Atmospheric Reviews"
      greeting: "Modular Peer Review for the Atmosphere"
      typewriter:
        enable: true
        prefix: "A "
        strings:
          - "federated review substrate"
          - "modular evaluation protocol"
          - "reviewer-owned credit system"
          - "rigorous alternative to platform review"
        type_speed: 80
        delete_speed: 50
        pause_time: 2500
      show_status: true
      show_scroll_indicator: true
      scroll_target: "#problem"
      cta_buttons:
        - text: The Problem
          url: "#problem"
          icon: hero/exclamation-triangle
        - text: SFU Lecture
          url: /talks/sfu-lecture.html
          icon: hero/presentation-chart-line
    design:
      style: centered

  - block: markdown
    id: problem
    content:
      title: "The Problem"
      text: |
        Scientific peer review is slow, opaque, gameable, and platform-captured. Reviewers receive no portable credit; readers cannot inspect the actual review when it would be most useful (post-publication, alongside the article); funders cannot tell good review work from poor.

        As more research moves toward AT Protocol-based, modular research workflows ([ATScience](https://atproto.science)), the question becomes urgent: **what does *review* look like on this substrate?**

  - block: markdown
    id: protocol
    content:
      title: "What we're building"
      text: |
        - **A modular review protocol** — review as a composition of evaluation primitives (claim-level assessment, method check, replication check, novelty judgment) rather than a monolithic letter. Each primitive is an AT Protocol record, signed by its author, citable on its own.
        - **atmospheric.reviews coordination layer** — software for soliciting, composing, and surfacing reviews against research artifacts published in the ATScience ecosystem.
        - **Reviewer-owned credit** — reviews are DID-linked AT Protocol records; portable identity carries review history across institutions and platforms; aggregation views surface contribution patterns without platform lock-in.
        - **Reference deployments** — end-to-end pilot review cycles with at least two real research communities in the BiTS / ATScience portfolio.

  - block: markdown
    id: approach
    content:
      title: "Approach"
      text: |
        The protocol design extends ongoing work presented in the [**SFU 2026 lecture on atmospheric reviews**](/talks/sfu-lecture.html) and builds on **ATScience** infrastructure.

        Modular review primitives are specified as **AT Protocol Lexicons**; conformance and composition rules are verifiable by tooling rather than by editorial discretion. Federated by design — any community can run its own review front-end against the shared protocol.

        Aligned with **Modal Foundation / Eurosky** for European hosting.

  - block: team-showcase
    id: about
    content:
      title: "About"
      user_groups:
        - Team
    design:
      max_columns: 2
      show_social: true
      show_interests: true
      max_interests: 4
      show_role: true
      show_organizations: false

  - block: contact-info
    id: contact
    content:
      username: torsten-goerke
      title: "Get Involved"
      text: "Interested in modular review or the ATScience portfolio?"
      social:
        - icon: at-symbol
          url: mailto:hello@atmospheric.reviews
          label: hello@atmospheric.reviews
        - icon: brands/bluesky
          url: https://bsky.app/profile/tgoerke.bsky.social
          label: Bluesky
---
