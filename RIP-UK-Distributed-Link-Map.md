# RIP UK — distributed link-map memorials

**Status:** editorial/product specification, 23 October 2026. **Canonical repository:** `KarstenEvans/RIP-UK`, not RIP-UK2. **Model:** RIP UK keeps the memory; the family keeps the memorial. **Existing source of truth:** [RIP-UK.md](RIP-UK.md), [RIP-UK-Tasks.md](RIP-UK-Tasks.md). Follow [Aletheia Protocol](https://github.com/KarstenEvans/aletheia-protocol) for provenance and optional [Thalia](https://github.com/KarstenEvans/thalia-protocol/blob/main/THALIA_PROTOCOL.md) for family-chosen respectful warmth and humour.

## Two separate files, two different owners

1. **RIP UK link registry:** optional public `Name.md` record containing **a name and approved URLs only**, with very short labels for navigation. This is not a copied obituary. A record may contain *only one link*. Do not ingest or reproduce the linked material.
2. **Family memorial:** optional exportable `memorial.md` kept **by the person/family/author at a provider of their choosing** (Google Drive, Sites, OneDrive, YouTube, own website, etc.). It may include as many personally approved stories, media references, family-history links or documents as they choose. RIP UK may guide its creation but does not take ownership or persist a copy.

If a family has only YouTube, an Instagram tribute or a Google Sites page, that is sufficient. They **do not need to produce an extra memorial document** to register a link. If they choose a Markdown life map, its authored copy resides with them.

## Minimal public register example

```markdown
# Name chosen by submitter

- [Our family tribute](https://example.org/family-tribute)
- [Video memories](https://www.youtube.com/watch?v=EXAMPLE_ID)
- [More about the person's work](https://example.org/project)
```

URL placeholders here are examples, not real memorials. No dates, location, living people's names, contact details, or identity documents are required. Use one `Name.md` plus a stable internal public identifier only if needed to distinguish names; public admin metadata is not added.

## Memorial life map (optional, owner-authored and owner-hosted)

The builder is a *gentle guide*, not an extraction engine. It suggests thematic branches, each pointing at the creator's own hosted content; empty branches are skipped.

- **Their own voice:** publicly shared talks, YouTube, Instagram, podcasts, interviews or writings, only where owner permits listing.
- **Who they were:** the names, values, quirks, humour, interests and experiences the owner *chooses* to preserve.
- **What they loved:** music, cooking, walks, clubs, animals, traditions, pets, places, photographs.
- **What they made or worked for:** art, science, craft, profession, projects, charity, advocacy, community initiatives.
- **Who loved them and remembers them:** links to *existing* family or friend tributes, with no newly collected living-person details.
- **What they hoped to carry forward:** charitable causes, an existing campaign such as Mental Health Mondays, useful resources, projects; do not claim a wish without source or authority.
- **Their places and connections:** an optional family-created map, and a separate family genealogy/GEDCOM resource hosted privately or publicly as they choose. Never map private residential addresses by default.
- **Continuing memories:** optional anniversaries, new letters, audio, pictures or tribute links added by the owner from their own hosting, with permission.

The site can *visualise links* as a tree/timeline/constellation or simple ordered list, using only labels and URLs already approved; it does not need to host the graph's underlying stories or assets. For people and pets; family chooses tone (warm default, storytelling, celebratory, reflective, gently funny), not RIP UK's automated inference.

## Verification: two different questions

**Reachability check:** Does the supplied URL resolve for the public visitor, with appropriate permissions? A private Google Drive link, login wall or transient URL must never be declared universally public merely because an editor could open it.

**Owner's approval:** Did the person who controls the memorial submit or approve this exact address, its intended audience, the displayed name and the public listing? A news source proving the link exists is not permission to register it on the family's behalf.

States: `research-draft-unlisted`, `submitted-awaiting-verification`, `owner-approved-listed`, `needs-link-update`, `withdrawn`. These states are administrative, not claims about the deceased person's identity or funeral details. Do not claim family approval for public-source celebrity examples.

Do not scrape, archive, transcribe, mirror, or republish someone else's copyrighted media just because it is online. The owner's host retains the source; RIP UK retains a pointer. Honor removals and edits. Avoid automatically publishing everything found online.

## Link lifecycle and durability

- Prefer original owner's stable URLs before news sites, reposted clips or mirrors.
- Identify links by original/third-party provenance, not as equal replacements. For Presley, Mental Health Mondays originated chiefly on Instagram; other videos may be publisher clips or podcasts. No verified official Presley-owned YouTube channel found during this research.
- Provide a manual `Replace broken link` request; validate with the owner before changing it.
- Later, perform opt-in automated *reachability* checks without downloading private content or falsely identifying consent. A link going offline is not an obituary correction.
- Offer a printable/downloadable owner-controlled Markdown and offline ZIP backup. Warn that Google Drive accounts, social platforms and YouTube videos can be deleted or restricted; persistence is not guaranteed.
- If an owner dies or loses access, offer a documented voluntary successor-approval process. Do not assert authority over accounts.
- Clear delist/takedown/correction control and human moderation before broad public launch.
- RIP UK can function with no cookies/accounts for casual visitors. If later an email is needed for admin recovery, store it separately from publicly hosted Markdown and minimise retention.

## Mini-AI-me is a separate, opt-in companion

The public registry has **no AI avatar, no synthetic first-person deceased speech and no Mini-AI-me advertisement**. A privately delivered research/profile file may be offered **only as an option** to a family or estate; let them approve sources and intended use. An AI memory companion can organise their own memories and answer factual questions with citations, but it must disclose it is an AI and not the person. Do not imply a bot restores direct conversation with the deceased or replaces human support. Do not publish the file or use family photographs, letters or voice models in training without the rights-holder's informed permission.

## Source-led pilot: Presley Walker Gerber

- [Unlisted name + public links sample](Presley-Walker-Gerber.md).
- Main themes: original family tributes, Presley's own `Mental Health Mondays` series and Studio 22 interview, charity collaboration; no downloaded media or reproduced letters.
- Respect the family's request for privacy; send only a brief optional introduction via verified public professional channels, if specifically authorised, with no repeated follow-up.
- Do not place an unsolicited, synthetic personality model in front of recently bereaved relatives.
- Do not insert a public listing until family (or appropriate rights-holder) says which links they want published.

## Existing design preserved

RIP-UK's planned original warm ivory/sage-green design, Create/Find/Map/Resources/About navigation, family-controlled eight-step creator, pets, cultural traditions, history/GEDCOM, and Irish RIP.ie wake/storytelling inspiration remain intact. RIP-UK2 is a separate Google-generated prototype: do not import its invented sample notices, badge claims, prefilled funeral details, data model or page styling.

**Next implementation gates:** recover the original ChatGPT-built site source/PC ZIP; reconcile its builder; add a link-only publication mode with public/private and owner-confirmation checks; test Google Drive link privacy and standalone Markdown; only then build the optional interactive life-map view.
