# RIP-UK — distributed memorial system

**Canonical owner:** KarstenEvans/RIP-UK. **Snapshot:** 2026-10-04. **Status:** documentation specification; implementation and live deployment unverified.  
**Technical contracts:** [Aletheia Protocol](https://github.com/KarstenEvans/aletheia-protocol) for evidence and provenance; [Thalia Protocol](https://github.com/KarstenEvans/thalia-protocol/blob/main/THALIA_PROTOCOL.md) as an optional tactful, human-appropriate humour companion. Generated memorial Markdown should include both references near its beginning (after YAML/title) but must not display technical branding prominently on public memorials.  
**Shared development rules:** [Aletheia GUI](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-GUI.md), [Aletheia development guide](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-dev.md), and [Aletheia Improve](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-improve/aletheia-improve.md).

## October 2026 decisions: precedence over archived September specification below

- **Correct repository:** `KarstenEvans/RIP-UK` is the owner. `RIP-UK2` is an initial Google AI Studio/Gemini **appearance-only prototype**; do not reuse its backend claims, seed notice data, verification shortcuts, or production code. The actual ChatGPT-built RIP UK site exists separately as a preview; obtain its PC ZIP/source and preserve its eight-step creator, dark-green/ivory visual design, Create/Find/Map/Resources/About menu. The canonical GitHub repository currently had only README/LICENSE before this documentation import. No working site code in this repository has been verified.
- **Memorial lives with family:** The family independently hosts `memorial.md` plus photos/audio/videos/files or external references on their own shared Drive, website or suitable hosting. All descriptions, hobbies, interests, achievements, memories, favorite places, dedications and public family-approved stories can be contained in Markdown. Empty optional fields do not render; do not invent biographies or "nice" traits. A record can be two heartfelt lines. Family remains curator/custodian; guide, do not seize accounts.
- **RIP-UK is a reference register:** store a durable ID and minimal approved discoverability/locator metadata, source URL and status; not replicated memorial text/media. Update URL when family moves and retain an inactive/unlisted recoverable reference after repeated link failure pending governance, unless deletion is requested. No service/password, private home, living person details or contact information in public GitHub.
- **Viewer:** fetch and validate family-hosted `memorial.md`, parse/sanitize safely, display linked media, and show readable fallback when an external file is missing. Google Drive share-link compatibility, cross-origin restrictions, cached copies, security, and family-chosen privacy must be specifically tested, not assumed. Provide local ZIP backup and restore guide. An optional future RIP-hosted facility must separately document storage limits, consent, costs and transfer/export guarantees; do not promise free perpetual hosting.
- **Created Markdown must be portable:** UTF-8, versioned YAML, ordinary Markdown, approved external URLs, provenance/uncertainty; relative media links resolve relative to document location only where host supports this. Users can locally edit/export without cloud AI.
- **Genealogy support is required:** PAF = Personal Ancestral File (LDS historical software); GEDCOM `.ged` is the portable genealogy format; FamilySearch GEDCOM 7 GEDZIP `.gdz` is ZIP-based, requires `gedcom.ged` and supports referenced local media. An additional `memorial.md` may be packaged as a GEDCOM-referenced file where compliant and validated, or shipped in a separate ordinary ZIP; simply renaming any ZIP to .gdz is *not* interoperable. Include FamilySearch/other family-tree URL, related RIP memorials, PAF migration guidance, and living-relative privacy. Never claim a match based only on a shared name.
- **User's new optional choice: Memorial vibe / tone.** Options: Warm & Loving (default), Reflective / Solemn, Joyful / Celebratory, Gentle Humour / Funny, and Wake / Storytelling; family may mix tones. Respect actual loved one's quirks, sayings and sense of humour; allow short stories, honest imperfections. Avoid forced jokes, stereotypes, mocking grief, or invented quotations. The **BBC Ghosts (UK, 2019–2023)** series is *research inspiration* for warm, character-first, cross-generational comedy and poignancy, not permission to reproduce its characters, artwork, writing or branding. Distinguish remembrance writing from ceremony/wake arrangements, which is a separate question. Suggested families approve all AI-drafted tone changes before publishing.
- **Cultural traditions:** ask "Are there any family, religious or cultural traditions you want represented?" rather than assuming ethnicity implies beliefs. Offer optional culturally researched sets, local custom text, and independent source dates for Irish Christian wakes/month's-mind, Gujarati Hindu Antyesti/prayers, Sikh Antam Sanskar, Buddhist Thai temple/cremation, Muslim Janazah, Jewish shiva, humanist and additional traditions; funeral and remembrance variations depend on family, region and faith.
- **Optional resources** separated from the memorial: books about genuine hobbies/interests/locations, grief help, funeral guides, genealogy, florist/charity pages, donations, memorial keepsakes, and photo restoration/colourisation/animation tools. Free/open-source precompiled installers or trustworthy browser apps first. Do not require paid apps, compilation, or affiliate purchase. Disclose referral relationships. For old-photo restoration: never silently overwrite originals, distinguish authentic from AI-enhanced or generated moving/talking portraits, obtain family permission, warn about uploads/privacy and about AI fabrication/false posthumous speech.
- **Pilot:** Dinesh Jiva Virji Gohil, born 1950-11-25, died 2026-09-24. Family-provided announcement is a **private example pending permission**, not an independently verified public funeral source. An extracted portrait exists in conversation artifacts but must **not be committed** or published until permission. Obitus webcast is a credential-protected transient service, not a public archive; do not store/reproduce its credentials.
- **Local app files needed:** `RIP-UK-GUI.md`, `RIP-UK-dev.md`, `RIP-UK-page.md` (page reconstruction), `RIP-UK.htm`, `RIP-UK-rsc.htm` and docs/how-to. Markdown is canonical; HTML is interface/resources. Follow Aletheia GUI/dev patterns while remaining a separately owned project. Aletheia Improve must check current RIP-UK repo files and PC preview source before modifications.
- **Privacy caveat:** deceased persons' data are not UK GDPR personal data, but data about living family, contributors, records, server access and moderation may be. A URL registry is not automatically exempt from compliance. Approvals, minimisation, moderation, contacts outside public repos, delisting, copyright/source documentation and accountable governance matter.

## Historical full-length design source (13 September 2026)

The material below is the recovered original `Aletheia-RIP-UK.md` from the user's file library. It is retained for decisions and provenance. If it conflicts with the October rules above, **October rules prevail**. Older examples and promised features are drafts and not evidence of implemented behaviour.

---
# Aletheia RIP UK

**File:** `Aletheia-RIP-UK.md`  
**Status:** Canonical project specification / app guidance  
**Version:** 0.2-draft  
**Project:** RIP UK  
**Public motto:** **RIP UK keeps the memory. The family keeps the memorial.**

---

## 1. Purpose

RIP UK is a free-to-use, distributed memorial registry and memorial-making guide for people and pets.

RIP UK is **not intended to become a giant warehouse of everybody's photographs and videos**. Its core job is to:

1. help a family create a respectful memorial;
2. produce a portable memorial record;
3. help the family choose where the memorial will live on the open web;
4. register the public location so it can be found again;
5. keep private administrator/contact information separately;
6. help families preserve an offline copy;
7. provide optional maps, family-history links and useful resources.

The public-facing site should feel like a gentle guide to remembering a life, not a funeral-management dashboard.

Aletheia provides the truth, provenance and portable-record rules.  
Odysseus provides the guided workflow, publishing choices and interoperability.

Neither name needs to dominate the public user interface.

---

## 2. Core principle

> **RIP UK keeps the memory. The family keeps the memorial.**

RIP UK keeps the minimal public registry record and the private administration pointer.

The family controls the full memorial, media and archive and may host it wherever they choose.

RIP UK should prefer open, portable, replaceable components over lock-in.

---

## 3. Public experience

### 3.1 Primary navigation

Keep the site deliberately uncluttered.

Suggested top-level navigation:

- **Create a memorial**
- **Find a memorial**
- **Map**
- **Resources**
- **About**

Do not expose protocol documentation, developer controls, confidence engines, AI terminology or test functions in the normal family journey.

### 3.2 Homepage message

Suggested structure:

**Remember a life. Keep the memories yours.**

Create a free memorial for someone or a much-loved pet.  
We can help you gather the words, photographs, videos and family history, then show you free places where you can keep and share it.

Primary buttons:

- **Create a memorial**
- **Find a memorial**

Secondary link:

- **Explore the memorial map**

---

## 4. Visual and emotional design

The site should be warm and human rather than dark, corporate or funeral-parlour-like.

### Design direction

- warm ivory / paper-like main background
- soft leaf or sage green
- muted sky blue
- gentle dusty rose / terracotta accents
- warm charcoal text
- generous white space
- large photographs
- rounded, calm controls
- restrained animation
- strong mobile accessibility

Avoid assuming religion, afterlife beliefs, species or family structure.

Do not make "Rainbow Bridge" a site category. If a family wants that language in an individual pet memorial, it may be used there.

Do not use black-heavy "mourning" styling by default.

### Memorial tone

The emotional centre is:

- who they were;
- why they mattered;
- what people remember;
- photographs, voices, videos and stories.

The death date and service information are important facts, but should not visually dominate the page.

---

## 5. Create-a-memorial journey

The creation experience should feel like a mentor, not a long form.

### Step 1 — Who are we remembering?

- Person
- Pet

For pets, optionally ask species. Never assume "pet" means dog.

### Step 2 — Name and basic facts

Collect only what is useful:

- full/name used in life
- date or approximate year of birth
- date of passing
- town/area
- optional service/funeral information
- optional charity/donations

Unknown dates must remain unknown. Never invent fallback years.

### Step 3 — Tell their story

Offer:

- **I'll write it**
- **Suggest some words**

Suggested prompts may include:

For anyone:
- What always made you smile about them?
- What were they known for?
- What place, song, hobby or habit brings them to mind?
- What should never be forgotten?

For pets:
- Favourite sleeping place?
- Favourite person?
- Favourite food, toy or habit?
- What made them unmistakably *them*?

AI-generated wording must use only supplied facts and clearly remain editable.

### Step 4 — Memories and media

Support multiple items, not a single photograph:

- cover photograph
- image gallery
- MP4 or other short videos
- hosted video URLs
- audio/voice recordings
- scanned letters
- drawings
- service sheets
- PDFs and documents

Large media should normally be referenced from family-selected storage rather than stored in the public Git repository.

### Step 5 — Family history

For human memorials, optionally support:

- GEDCOM `.ged`
- GEDZIP `.gdz`
- FamilySearch link
- other genealogy/family-tree URL
- related RIP UK memorial IDs
- family-map URL

Pets may be represented in the Aletheia memorial layer as family companions without falsifying standard human genealogical relationships.

### Step 6 — Choose where the memorial lives

RIP UK should offer simple choices and guidance rather than forcing central hosting.

Possible homes include:

- Google Sites
- Google Drive shared folder
- Google Photos shared album
- OneDrive shared folder
- YouTube for video
- Internet Archive where appropriate
- family-owned website
- GitHub Pages / Cloudflare Pages for technical users
- another public URL supplied by the family

The interface should say what each option is best for and whether visitors need an account.

### Step 7 — Optional map

Offer a family-created Google My Map or another map URL.

A family map can contain:

- memorial location
- cemetery or churchyard
- family homes
- meaningful places
- war memorials
- historic graves
- other family-history locations

RIP UK may later create optional regional aggregate maps from memorials whose administrators opt in.

### Step 8 — Publish and share

Generate, but do not force:

- Facebook post
- LinkedIn post
- WhatsApp/copyable text
- social image/card
- calendar file for service information
- shareable memorial URL

Social networks are mirrors and discovery channels, not the canonical archive.

### Step 9 — Keep your own copy

Offer a clear final action:

**Download your memorial archive**

The family should be able to keep a portable offline package so it is not dependent on RIP UK, Google, Facebook or any other provider.

---

## 6. Portable memorial format

### 6.1 Canonical Markdown

Each memorial should have a human-readable Markdown record with structured YAML front matter.

Example:

```yaml
---
schema: "aletheia-rip-uk/0.2"
rip_id: "RIP-UK-00001234"
slug: "mitten-evans"

name: "Mitten Evans"
record_type: "pet"
species: "cat"

birth:
  year: 2010
  approximate: true

death:
  date: "2026-08-02"
  town: "Swindon"
  country: "England"

verification:
  status: "family-submitted"
  sources: []

media:
  cover: "media/cover.jpg"
  gallery: []
  video: []
  audio: []
  documents: []

family_history:
  gedcom: "gedcom.ged"
  gedzip: ""
  external_tree_url: ""
  related_memorials: []

map:
  public_url: ""
  location_precision: "town"

publishing:
  memorial_url: ""
  archive_url: ""
  photo_album_url: ""
  facebook_url: ""
  linkedin_url: ""

resources:
  town: "Swindon"
  postcode_area: "SN1"
---
```

The body then contains the human memorial text.

### 6.2 Verification language

Do not label a record "verified" merely because a family member submitted it.

Suggested states:

- `family-submitted`
- `source-linked`
- `independently-checked`
- `historic-record-linked`
- `unverified`

For human notices, source links may include funeral-director pages, probate/index records, published notices or other appropriate evidence.

Private evidence must never be published automatically.

---

## 7. GEDCOM and GEDZIP

RIP UK should support FamilySearch GEDCOM 7 where possible.

A GEDZIP `.gdz` is a ZIP archive with a required `gedcom.ged` file and the local media/documents referenced by that GEDCOM.

RIP UK may define an **Aletheia Memorial Profile** for GEDZIP so a memorial package can contain, where referenced appropriately:

```text
gedcom.ged
memorial.md
media/
  cover.jpg
  photo-01.jpg
  memory.mp4
  voice.m4a
documents/
  service-sheet.pdf
  letters.pdf
```

The family should be warned that large videos can make a `.gdz` very large. They may choose to keep large videos as external URLs while preserving thumbnails, metadata and links in the package.

Aletheia should not misuse human GEDCOM family structures to pretend pets are genealogical human individuals. Pet/family-companion relationships belong in the Aletheia memorial metadata/viewer layer unless a future standards-compatible method is agreed.

---

## 8. RIP UK registry record

RIP UK's public registry should remain small.

Example:

```yaml
rip_id: "RIP-UK-00001234"
name: "Mitten Evans"
record_type: "pet"
species: "cat"
date_of_passing: "2026-08-02"
location: "Swindon"

memorial_url: "https://..."
archive_url: "https://..."
family_tree_url: ""
map_url: "https://..."

verification: "family-submitted"
status: "active"
last_link_check: "2026-09-13"
```

Do not put the administrator's email address in this public record.

---

## 9. Private administration record

RIP UK needs a private administration layer linking a memorial to a living administrator.

Minimum useful fields:

```text
rip_id
administrator_email
consent_timestamp
update/recovery credential or secure token reference
last_contact_check
link-status notification preferences
```

Collect the minimum possible information.

Administrator data is personal data and must be treated accordingly.

The legal structure and ICO data-protection-fee position must be checked before public launch, especially once affiliate/referral activity begins.

---

## 10. Distributed storage principle

RIP UK should not require a paid central hosting plan for every family.

The preferred model is:

```text
RIP UK registry
      |
      +-- public memorial URL
      +-- public archive URL (optional)
      +-- photo/video album URL (optional)
      +-- family-history URL (optional)
      +-- map URL (optional)
      +-- social mirrors (optional)
```

If a family changes provider, it should only need to update the URL in the RIP UK registry.

Odysseus may later perform periodic link-health checks and contact the administrator privately when a registered memorial disappears.

---

## 11. Maps

### Initial map model

Use Google My Maps as a friendly initial option because many users already have Google accounts and can create/share maps.

Two levels may coexist:

1. **Family map** — created and controlled by the family.
2. **RIP UK regional/public map** — optional aggregate map of opt-in memorials, cemeteries, churchyards, war memorials and historic graves.

Site categories:

- People
- Pets
- Cemeteries
- Churchyards
- War memorials
- Historic graves

Family History belongs primarily inside memorials and family maps rather than as a death-map category.

Never expose a precise private-home burial location by default. Use town/area precision unless the administrator explicitly chooses otherwise.

---

## 12. Resources and sustainability

The memorial-making service should remain free to families.

RIP UK may support itself through a single calm **Resources** area using:

- affiliate links
- referral links
- carefully labelled sponsored resources
- optional premium local-business listings later

The legal/business structure should not be described as a registered charity or formal non-profit unless it actually becomes one.

### Resource categories

For people:

- funeral directors
- florists
- wakes and catering
- celebrants
- cemeteries and natural burial grounds
- monumental masons / memorial stones
- probate and wills
- bereavement support
- grief books and audiobooks
- photo restoration
- memorial printing
- family-history and genealogy services
- charities

For pets:

- pet bereavement support
- vets and aftercare
- crematoria
- pet cemeteries
- memorial stones/plaques
- urns and keepsakes
- grief books
- home-burial guidance
- local legal/environmental guidance where relevant

Resources should be ranked by usefulness and trust, not solely by commission rate.

Affiliate relationships must be clearly disclosed.

---

## 13. Pet aftercare and burial guidance

RIP UK may provide pet-burial and aftercare information because families often need practical help quickly.

This content must be **jurisdiction-specific, sourced and cautious**.

Do not invent a universal burial depth or recommend chemicals, lime, plastic wrapping or containers without authoritative guidance.

For example, current England guidance permits burial of small domestic pets such as cats or dogs on the owner's land, while animal-welfare guidance recommends suitable depth, distance from water sources and biodegradable wrapping. Rules and circumstances can vary, including disease/treatment and nation within the UK.

The site should therefore provide:

- "Can I bury my pet at home?"
- "How deep should the grave be?"
- "What should I wrap or place them in?"
- "What if I rent?"
- "What if there is groundwater?"
- "When should I ask my vet?"
- "Pet cremation vs home burial"
- "Find a pet cemetery"
- "How to create a place to remember them"

Each page should show its source and last-reviewed date.

---

## 14. Public records and family-history research

RIP UK should not attempt to ingest every deceased person in Britain.

Instead offer **Research this person** tools that help families locate relevant records and then choose whether to create/link a memorial.

Potential sources and links include:

- General Register Office
- local register offices
- probate records
- FreeBMD / historic indexes
- parish and church records
- FamilySearch
- archives
- commercial genealogy services where useful

Do not imply that RIP UK has independently verified a death unless it has actually checked an appropriate source.

---

## 15. Aletheia rules

```text
[ALETHEIA_RIP_UK_INIT]
VERSION: 0.2
MODE: DISTRIBUTED MEMORIAL CREATION AND REGISTRY

1. Treat supplied facts as claims until supported.
2. Never invent birth years, dates, species, relationships, service times or URLs.
3. Distinguish family-submitted information from independently checked information.
4. Keep living administrator contact information private.
5. Prefer portable formats and user-owned storage.
6. Generate editable wording; never replace the family's voice.
7. Preserve source URLs and provenance.
8. Do not force religious or afterlife language.
9. Treat pets as family when the family does, without corrupting genealogy standards.
10. Keep the public interface simple; protocol machinery stays backstage.
11. Resource recommendations must disclose affiliate/referral relationships.
12. Safety/legal guidance must be jurisdiction-specific and source-linked.
13. Do not publish precise private locations by default.
14. A family must be able to export its memorial and leave RIP UK.
[END_ALETHEIA_RIP_UK_INIT]
```

---

## 16. Odysseus workflow

```text
START
  |
  +-- Person or Pet
  |
  +-- Collect facts
  |
  +-- Story / "Suggest some words"
  |
  +-- Add multiple memories/media
  |
  +-- Optional family history / GEDCOM import
  |
  +-- Evidence/source links where appropriate
  |
  +-- Generate memorial.md
  |
  +-- Generate/update gedcom.ged where applicable
  |
  +-- Generate GEDZIP / portable archive
  |
  +-- Choose free/public home for memorial
  |
  +-- Verify public URL works
  |
  +-- Register minimal record with RIP UK
  |
  +-- Optional family My Map
  |
  +-- Generate Facebook / LinkedIn / WhatsApp sharing
  |
  +-- Download family-owned archive
  |
END
```

Odysseus should recommend the simplest path first and expose advanced options only when useful.

---

## 17. Existing Google AI Studio prototype

The Google AI Studio version is a useful prototype, not the canonical finished application.

Useful parts to retain:

- person/pet classification
- memorial cards
- intake flow
- Markdown generation
- social-post generation
- service/calendar ideas
- local-resource concept
- search/filter ideas

Known prototype issues to replace:

- dark/blue application-dashboard feel
- protocol/test material exposed to families
- single-photo assumption
- invented fallback birth year
- generic "tail wags" pet wording
- overconfident verification labels
- hard-coded non-live production URL
- browser-local storage presented as if it were GitHub publishing
- mock affiliate data
- no genuine public-record search
- no distributed-hosting chooser
- no GEDCOM/GEDZIP workflow

`RIP-UK2` should remain the reference snapshot of the Google prototype until the replacement is stable.

---

## 18. Site implementation direction

Initial public site:

- GitHub repository: `KarstenEvans/RIP-UK`
- deploy from GitHub to Cloudflare Pages
- start on the free `pages.dev` address
- custom domain later if/when appropriate
- mobile-first
- progressively enhanced
- keep static/public content separate from private administration data

The first site does not need every automated connector.

KISS sequence:

1. create memorial locally in browser;
2. download Markdown + archive;
3. guide user to a free hosting option;
4. user supplies public URL;
5. RIP UK stores the registry entry and private admin contact;
6. add automation/connectors later.

---

## 19. Success test

A non-technical person should be able to arrive after losing someone or a pet and, without knowing what GitHub, Cloudflare, GEDCOM, Aletheia or Odysseus are:

1. create something warm and personal;
2. add more than one photograph/video;
3. get help with wording only if wanted;
4. understand free ways to keep it online;
5. keep their own offline copy;
6. share it with family;
7. find it again through RIP UK.

If the technology becomes the story, simplify it.

---

## 20. Find Local Help — location-aware resources

The public site should not call this feature "A2Z". The user-facing name should be something plain such as:

**Find local help**

Under the hood it may reuse/generalise the Aletheia Local Search / Swindon.org.uk A2Z search approach.

### User flow

1. Ask for a **town, postcode or area**.
2. Let the user tick one or more categories.
3. Search only the selected categories near that location.
4. Show useful results with clear external links.
5. Mark affiliate/sponsored results clearly.
6. Do not rank solely by affiliate commission.
7. Allow the user to change location without restarting.

Suggested category checkboxes:

- Florists
- Funeral directors
- Cemeteries
- Crematoria
- Wake venues
- Caterers
- Celebrants
- Memorial masons / headstones
- Probate / wills
- Bereavement support
- Pet crematoria
- Pet cemeteries
- Pet memorials
- Genealogy / family-history help

Example:

> **Find local help**
>
> Where do you need help? `[Swindon / SN1]`
>
> ☑ Florists  
> ☑ Funeral directors  
> ☐ Cemeteries  
> ☐ Wake venues  
>
> **Search nearby**

### Search behaviour

- Prefer real current businesses and services.
- Use location-aware web/business search rather than a frozen directory where possible.
- Reuse Swindon.org.uk directory knowledge when useful, but RIP UK must work nationally.
- Show distance/area only when supported by the search source.
- Never imply that RIP UK endorses a provider merely because it appears.
- Provide a short "How results are chosen" explanation.
- Affiliate links may be used where available, with disclosure.
- Free/public services should remain visible even when no affiliate relationship exists.

### Resource monetisation rule

For books, the default RIP UK book affiliate should currently be **Bookshop.org UK** unless a later commercial review changes this. The current public Bookshop.org UK affiliate offer is 10% for non-bookstore affiliates. Waterstones' current Awin terms are materially lower for ordinary publishers, so avoid duplicating every book with two shop links unless there is a user benefit.

The Resources page should stay calm: one primary book-buying route is enough.
