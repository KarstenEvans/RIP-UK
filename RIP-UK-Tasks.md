# RIP-UK-Tasks — implementation and research backlog

**Canonical owner:** KarstenEvans/RIP-UK. **Snapshot:** 2026-10-04. **Status:** documentation specification; implementation and live deployment unverified.  
**Technical contracts:** [Aletheia Protocol](https://github.com/KarstenEvans/aletheia-protocol) for evidence and provenance; [Thalia Protocol](https://github.com/KarstenEvans/thalia-protocol/blob/main/THALIA_PROTOCOL.md) as an optional tactful, human-appropriate humour companion. Generated memorial Markdown should include both references near its beginning (after YAML/title) but must not display technical branding prominently on public memorials.  
**Shared development rules:** [Aletheia GUI](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-GUI.md), [Aletheia development guide](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-dev.md), and [Aletheia Improve](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-improve/aletheia-improve.md).

## Priority snapshot (4 October 2026)

- [x] Locate existing `KarstenEvans/RIP-UK` (main only README.md and LICENSE initially); confirm `RIP-UK2` is noncanonical Gemini prototype.
- [x] Recover historical Aletheia-RIP-UK, rip-uk-site, tasks and ideas from the user's Library.
- [ ] Obtain ChatGPT-built PC ZIP/export; inventory actual 8 steps and working functions before touching HTML.
- [ ] Add repo-local `RIP-UK-GUI.md`, `RIP-UK-dev.md`, `RIP-UK-page.md`, and `AGENTS.md` using shared Aletheia rules; do not silently invent features of preview.
- [ ] Preserve visual styling observed: ivory + dark forest green, large readable serif headings, mobile hamburger and existing five navigation entries.
- [ ] Implement source-of-truth `memorial.md` editor with compact required name/type and optional known/approximate dates, description, hobbies, interests, achievements, sayings, favourite locations, images/media URLs, cultural preferences, charity/donation, family history; omitted fields disappear; literal "none" remains.
- [ ] Add optional Tone/Vibe selector with family approval: warm, reflective, joyful, gentle humour, wake/storytelling; no forced humour or BBC-derived copyrighted expression.
- [ ] Validate public URL fetch/render for Drive, OneDrive, family website; account for CORS, permissions, expiration, redirect, HTML viewer pages instead of raw Markdown, no unsafe HTML; provide realistic fallback.
- [ ] Implement minimal Git-backed registry index ID→approved public memorial URL/status; stable ID with change URL/transfer custodian process, unlist/tombstone after repeated failures, deletion on authorised request; no private contacts in public repo.
- [ ] Provide local-only export ordinary backup `.zip` with `memorial.md` and family-owned files when supplied; do not download third-party protected material without entitlement.
- [ ] Add GEDCOM 7 `.ged` import/export, standards-valid GEDZIP `.gdz` with mandatory `gedcom.ged`, referenced media and optional `memorial.md` only when accurately referenced; test with independent viewer; PAF legacy migration guide; privacy filters for living relatives.
- [ ] Draft a non-stereotyping optional tradition questionnaire with reviewed source links per faith and geography.
- [ ] Research free-first photo restoration/colourisation, pre-built cross-platform and web tools, Canva/CapCut trials, MyHeritage Deep Nostalgia historical context; privacy / authenticity disclosures and source originals.
- [ ] Build contextual `RIP-UK-rsc.htm` with opt-in books, florists, family genealogy aids, grief resources, charity links, disclosure and no commercialization in tribute.
- [ ] Pilot Dinesh Gohil *privately* pending family permission; do not publish photo, webcast credentials, household address or sensitive living-family details.
- [ ] Run static, accessibility, mobile and true link validation; produce PASS/PARTIAL/FAIL evidence and human publishing gate.

## Recovered September checklist (historical, statuses require current verification)

The checklist below was written prior to the ChatGPT website preview and may have now-completed UI features. Do not mark those items as verified live simply because a screenshot shows a control.

---
# RIP UK — Tasks

**Status:** Working task list  
**Project principle:** **RIP UK keeps the memory. The family keeps the memorial.**

Legend:

- `[ ]` not started
- `[-]` in progress
- `[x]` completed
- `[R]` research/decision required

---

## 0. Protect what already exists

[x] Download Google AI Studio prototype ZIP.

[x] Keep `KarstenEvans/RIP-UK2` as the untouched/reference Google AI Studio prototype.

[x] Keep `KarstenEvans/RIP-UK` as the intended clean project repository.

[ ] Add `Aletheia-RIP-UK.md`, `ideas.md` and `tasks.md` to `RIP-UK`.

[ ] Do not overwrite/delete `RIP-UK2` while the replacement is being developed.

---

## 1. Canonical memorial format

[ ] Adopt a versioned YAML + Markdown memorial schema.

[ ] Remove all invented defaults, especially the prototype's fallback birth year.

[ ] Add:
- `rip_id`
- `record_type`
- `species`
- approximate/unknown dates
- verification state
- source list
- media arrays
- family-history fields
- external hosting URLs
- map URL
- resource location fields

[ ] Define verification states:
- family-submitted
- source-linked
- independently-checked
- historic-record-linked
- unverified

[ ] Keep living administrator email outside public Markdown.

[ ] Produce a clean Mitten test memorial using the new schema.

---

## 2. GEDCOM / GEDZIP

[R] Confirm exact GEDCOM 7 encoding for:
- memorial Markdown as a referenced document/file;
- photographs;
- MP4/video;
- audio;
- PDFs;
- remote URLs.

[ ] Define an **Aletheia Memorial GEDZIP Profile**.

[ ] Build a tiny valid test `.gdz`.

[ ] Test opening/importing the `.gdz` in at least one GEDCOM-compatible application.

[ ] Decide how pets are represented without corrupting human genealogy semantics.

[ ] Add GEDCOM/GEDZIP import to the create flow.

[ ] Add **Download memorial archive**.

[ ] Add **Restore memorial from archive** later.

---

## 3. New site design

[ ] Build a new RIP UK front-end using the Google prototype only as functional inspiration.

[ ] Replace dark blue dashboard appearance with warm memorial design:
- ivory/paper
- sage
- soft blue
- dusty rose/terracotta
- warm charcoal

[ ] Keep primary navigation minimal:
- Create
- Find
- Map
- Resources
- About

[ ] Remove visible Aletheia/Odysseus/protocol/debug material from the normal user journey.

[ ] Homepage headline around remembering life rather than managing death.

[ ] Make photographs and stories visually dominant.

[ ] Mobile-first test.

[ ] Accessibility test: contrast, keyboard, text size, screen-reader labels.

---

## 4. Create-a-memorial flow

[ ] Person / Pet selection.

[ ] Optional pet species.

[ ] Basic facts with unknown/approximate dates supported.

[ ] Story prompt.

[ ] Buttons:
- **I'll write it**
- **Suggest some words**

[ ] AI text must use supplied facts only.

[ ] Multiple image upload/selection.

[ ] Multiple video/media entries.

[ ] Audio and document entries.

[ ] Optional funeral/service details.

[ ] Optional charity/donation link.

[ ] Optional family-history import/link.

[ ] Review screen before generation.

[ ] Generate Markdown.

[ ] Generate archive.

[ ] Generate sharing text.

---

## 5. Distributed publishing chooser

Build a final "Where would you like your memorial to live?" step.

[R] Verify current public-sharing behaviour and account requirements for:
- Google Sites
- Google Drive
- Google Photos
- Google My Maps
- OneDrive
- YouTube
- Internet Archive

[ ] Add "I already have a website" URL option.

[ ] Add "Not sure — help me choose" option.

[ ] Write short, 9-year-old-readable publishing guides.

[ ] Add a public-URL test before registration.

[ ] Explain that social media is optional and is not the family archive.

---

## 6. RIP UK registry

[ ] Define minimal public registry schema.

[ ] Create first registry storage implementation.

[R] Choose storage for private administrator records:
- Cloudflare D1/KV?
- another minimal database?
- encrypted small store?

[ ] Separate public registry data from private admin data.

[ ] Generate stable RIP IDs.

[ ] Add register/update memorial URL workflow.

[ ] Add email ownership/confirmation method.

[ ] Add administrator recovery method.

[ ] Add delist/delete flow.

[ ] Add transfer-to-new-admin flow later.

[ ] Add broken-link status rather than silently deleting records.

---

## 7. Link health

[ ] Create manual "Check memorial link" function first.

[ ] Later: scheduled Odysseus link check.

[ ] Do not mark a memorial broken after one transient failure.

[ ] Notify administrator privately after repeated failure.

[ ] Let administrator replace URL while retaining same RIP ID.

---

## 8. Maps

[ ] Add optional Google My Maps guide.

[ ] Let family save `map_url`.

[ ] Add map privacy choice:
- town only
- cemetery/public place
- precise location (explicit choice)

[ ] Categories:
- People
- Pets
- Cemeteries
- Churchyards
- War memorials
- Historic graves

[R] Research best method to show opt-in RIP UK regional map without taking ownership of family maps.

[R] Confirm current Google My Maps import/export and sharing limits before automating.

[ ] Consider MapLibre/OpenStreetMap only when scale/independence requires it.

---

## 9. Family-history research

[ ] Add Family History section to human memorial.

[ ] Add `.ged` / `.gdz` upload.

[ ] Add external tree URL.

[ ] Add related RIP UK memorial IDs.

[R] Research/link:
- GRO
- probate search
- local register offices
- FreeBMD
- FamilySearch
- parish/church records
- archives

[ ] Build **Research this person** page.

[ ] Do not bulk-import every deceased person.

[ ] Create PAF-to-GEDCOM help page.

---

## 10. Resources and affiliate model

[ ] Add one calm top-level **Resources** link.

[ ] Add clear affiliate disclosure.

[ ] Create resource categories for:
- grief/support
- books/audiobooks
- florists
- funeral directors
- wakes/catering
- celebrants
- cemeteries/natural burial
- memorial stones/masons
- probate/wills
- genealogy
- photo restoration
- pet aftercare
- pet crematoria/cemeteries
- memorial keepsakes

[ ] Put trustworthy/free help before commercial links.

[R] Research suitable UK affiliate programmes.

[R] Research local-business referral/listing model.

[ ] Reuse Swindon/A2Z locality ideas where appropriate without making RIP UK dependent on Swindon.org.uk.

---

## 11. Pet aftercare guides

[R] Build jurisdiction matrix for England, Wales, Scotland and Northern Ireland.

[ ] Create sourced guide: "My pet has died — what do I do now?"

[ ] Create sourced guide: "Can I bury my pet at home?"

[ ] Cover:
- ownership of land
- water/ground conditions
- depth guidance
- biodegradable wrapping/container guidance
- circumstances where a vet should advise first
- cremation choices
- pet cemeteries
- renters
- moving house

[ ] Every guide shows source and last-reviewed date.

[ ] Do not recommend lime/chemicals/plastic as generic advice.

---

## 12. Social sharing

[ ] Fix pet-specific wording. Never use "tail wags" unless appropriate and supplied/selected.

[ ] Facebook post generator.

[ ] LinkedIn post generator.

[ ] WhatsApp/short-copy generator.

[ ] Social-card image generator later.

[ ] Never invent the production URL.

[ ] Only show/share a URL after it has actually been registered/tested.

[ ] Automatic posting only as a later, explicit opt-in connector.

---

## 13. Privacy and legal

[R] Run exact RIP UK operation through ICO data-protection-fee self-assessment before public launch.

[ ] Draft privacy notice covering administrator data.

[ ] Draft cookie policy only for cookies actually used.

[ ] Data minimisation review.

[ ] Define retention/deletion period for admin data.

[ ] Do not publish administrator email.

[ ] Abuse/fraud/takedown process.

[ ] Terms for family-submitted memorials.

[R] Review affiliate disclosure obligations.

[R] Review user-uploaded media/copyright terms.

---

## 14. Prototype code defects to remove

[ ] Remove hard-coded `uknotices.rip` URL.

[ ] Remove `1945` fallback.

[ ] Remove generic dog language from pet posts.

[ ] Replace localStorage-as-publishing claim with honest local draft behaviour.

[ ] Replace mock affiliate entries or label them clearly during development.

[ ] Replace overconfident verification badge.

[ ] Add genuine distributed-hosting step.

[ ] Add multiple media support.

[ ] Add GEDCOM/GEDZIP.

[ ] Hide protocol modal from normal families.

---

## 15. Deployment

[ ] Build clean site in `KarstenEvans/RIP-UK`.

[ ] Connect `RIP-UK` to Cloudflare Pages.

[ ] Use free `pages.dev` URL first.

[ ] Add custom domain only after the project proves itself.

[ ] Add basic analytics only if privacy-compatible and useful.

[ ] Add Search Console when public.

[ ] Add sitemap/robots.

[ ] Add structured data after schema research.

---

## 16. First usable release definition

RIP UK v0.1 is usable when a family can:

[ ] create a Person or Pet memorial;

[ ] add a cover photo and several other media links/files;

[ ] write text or request an editable suggestion;

[ ] download `memorial.md`;

[ ] download a portable memorial archive;

[ ] choose a free public hosting method using a simple guide;

[ ] provide/test the public memorial URL;

[ ] register it with a RIP ID;

[ ] keep administrator email private;

[ ] generate a correct Facebook/LinkedIn/WhatsApp post;

[ ] find the memorial again by name/location/RIP ID;

[ ] access the Resources page without the memorial becoming an advert.

---

## 17. Source notes already checked

These are starting points, not a substitute for nation-specific review.

- FamilySearch GEDCOM 7 / GEDZIP specification: https://gedcom.io/specifications/FamilySearchGEDCOMv7.html
- GOV.UK animal burial / groundwater guidance (England): https://www.gov.uk/guidance/animal-burials-prevent-groundwater-pollution
- RSPCA pet bereavement / burial guidance: https://www.rspca.org.uk/adviceandwelfare/pets/bereavement/goodbye

## 18. Local help search

[ ] Add **Find local help** to Resources.

[ ] Ask for town/postcode/area.

[ ] Add multi-select checkboxes for:
- florists
- funeral directors
- cemeteries
- crematoria
- wake venues/catering
- celebrants
- memorial masons
- probate/wills
- bereavement support
- pet aftercare
- genealogy help

[ ] Reuse/generalise Aletheia Local Search / Swindon.org.uk A2Z logic.

[ ] Keep national RIP UK search independent of Swindon.org.uk.

[ ] Define ranking rules: relevance/trust first; commission never determines inclusion.

[ ] Add affiliate/sponsored disclosure.

[R] Compare local-search providers/APIs and free limits before automating.

---

## 19. Cloudflare first-site launch

[ ] Generate the first static RIP UK site from `rip-uk-site.md`.

[ ] Put deployable site files under `/public`.

[ ] Ensure `/public/index.html` exists.

[ ] Connect `KarstenEvans/RIP-UK` to Cloudflare Pages.

[ ] Cloudflare project name: request `rip-uk` if available.

[ ] Production branch: `main`.

[ ] Build command: `exit 0` for the first static version.

[ ] Build output directory: `public`.

[ ] Keep project Markdown/spec files outside `/public`.

[ ] Test the resulting `*.pages.dev` address on mobile and desktop.

[ ] Do not buy a custom RIP UK domain until the prototype proves useful.

---

## 20. Google presence

[ ] Recover/appeal the existing Swindon.org.uk Business Profile before attempting a duplicate.

[R] Confirm Swindon.org.uk still meets current Google Business Profile in-person eligibility.

[R] Do **not** create a RIP UK Business Profile merely to obtain a map pin if RIP UK is online-only.

[ ] If RIP UK later genuinely serves customers face-to-face at an eligible staffed location during stated hours, review Business Profile eligibility then.

[ ] In the meantime use:
- public RIP UK website
- Google Search Console
- Google My Maps
- Google Sites/Drive guidance
- structured data and normal Google indexing

---

## 21. Affiliate launch

[ ] Apply for/activate Bookshop.org UK affiliate account.

[ ] Use Bookshop.org UK as the primary book link initially.

[R] Keep Waterstones/Awin as a possible later alternative, not a duplicate default link.

[ ] Apply to Awin for useful non-book categories as the Resources catalogue grows.

[ ] Add a standard affiliate disclosure component.

[ ] Keep affiliate links out of the memorial-creation emotional flow unless directly useful.

---

## 22. Back burner — AI information page

**Status:** Back burner / not part of the first RIP UK release.

[ ] Create a separate informational page about useful AI services.

[ ] Keep this page **separate from Resources**. It is informational, not part of the funeral/pet-support affiliate area.

[ ] Include ordinary official links for:
- ChatGPT / OpenAI
- Google Gemini
- Claude / Anthropic
- DeepSeek
- Manus
- Perplexity
- Grok / xAI
- Mistral / Le Chat
- other useful AI services as the landscape changes

[ ] For each service, briefly explain:
- what it is good for;
- whether a free tier exists;
- whether file/image upload is available;
- whether it may help with memorial writing, family-history research, document organisation or similar RIP UK tasks.

[ ] Do not imply an affiliate relationship where none exists.

[ ] Keep affiliate/referral status as metadata only, so links can be changed later without redesigning the page.

[R] Periodically check whether any of these services launch a genuine public affiliate/referral programme.

[R] Google Workspace and Manus may be worth reviewing separately later, but do not prioritise them for the first release.

[ ] No AI-company affiliate work should block the main RIP UK site, Cloudflare deployment, memorial workflow, maps, registry or local-help search.


## Three-pass research completed (4 October 2026)

Reviewed BBC Ghosts for warm character-led humour, RIP.ie/MuchLoved/ForeverMissed, culturally diverse mourning and remembrance, GEDCOM/GEDZIP/PAF, and free-first pre-built local photo restoration. Findings and source references: [RIP-UK-Research.md](RIP-UK-Research.md). Research does not establish that the features are implemented, families consulted or browsers tested.
