# RIP-UK-Ideas — research and future enhancements

**Canonical owner:** KarstenEvans/RIP-UK. **Snapshot:** 2026-10-04. **Status:** documentation specification; implementation and live deployment unverified.  
**Technical contracts:** [Aletheia Protocol](https://github.com/KarstenEvans/aletheia-protocol) for evidence and provenance; [Thalia Protocol](https://github.com/KarstenEvans/thalia-protocol/blob/main/THALIA_PROTOCOL.md) as an optional tactful, human-appropriate humour companion. Generated memorial Markdown should include both references near its beginning (after YAML/title) but must not display technical branding prominently on public memorials.  
**Shared development rules:** [Aletheia GUI](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-GUI.md), [Aletheia development guide](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-dev.md), and [Aletheia Improve](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-improve/aletheia-improve.md).

**Rule:** The entries below are research candidates, **not committed product capabilities**. Project scope: no storing the family's voice/media centrally in RIP UK; it only registers the family-owned memorial URL.

## October 2026 additions and creative studies

1. **Vibe/voice choice (proposed MVP):** warm/loving, reflective, joyful celebration, affectionate humour, wake storytelling. A wake may be a real gathering *and* a way of telling stories; ask ceremony type separately from writing tone. Never make a comedy setting the default for bereaved families; allow hybrid.
2. **BBC Ghosts creative lessons:** Character-first sketches, histories across decades, amusing little habits, warmth, belonging and bittersweet endings. Reference comedy research for *patterns* only; do not copy scripted lines, personalities, props, or visual style, and do not suggest the real deceased is speaking from beyond the grave.
3. **Legacy story prompts:** `Things Dad always said`, `The story that still makes us laugh`, `The recipe they guarded`, `The card trick everyone remembers`, `A wonderful ordinary day`, `How they welcomed people`; every entry optional.
4. **Photo repair and animation (family-controlled):** scan/straighten/de-scratch, optional colourisation, restore faded exposures, black & white conversion, non-destructive face enhancement, motion from still photo, clearly labelled AI talking-photo recreations. Keep before/after and source. Prioritise accessible prebuilt/open-source tools and vetted free trials; research actual privacy practices before naming upload services as safe.
5. **Culture-by-choice templates:** optional individual Hindu, Sikh, Buddhist, Jewish, Muslim, Christian, Irish-wake and secular guidance with source checking and family override; avoid cultural overgeneralisation.
6. **Memorial/archival portability:** GEDZIP profile plus general family backup ZIP, relative/absolute URL export/rebase manifest, migrations between Drive accounts, restore old versions, confirm media link health, safe import with size limits.
7. **Genealogy discovery:** PAF to GEDCOM help; FamilySearch individual link, records/probate/FreeBMD, related memorials, opt-in family history map with sources and deceased-first default.
8. **Resources rather than advertisements:** family-specific books, local flowers, favourite charity donations, genealogy guides, memory albums, photo restoration tutorials, inexpensive creative gifts. Clearly distinguish genuine family preferences from recommendation engines; family controls display.
9. **Family curation and inheritance:** private custodian contact, opt-in successive caretakers, downloadable annual checkup instructions, link health alerting, restoration from ZIP.
10. **Future optional facilitation only:** RIP UK-hosted memorial for families without storage, separately approved cost/retention/privacy policy and easy family export. Not the default.

## Recovered September ideas (historical source)

# RIP UK — Ideas

**Status:** Living idea register  
**Rule:** Ideas are not commitments. Promote an idea into `tasks.md` only when we decide to build or research it.

---

## Product identity

- Public name: **RIP UK**
- Motto: **RIP UK keeps the memory. The family keeps the memorial.**
- Position RIP UK as a guide, registry and mentor rather than a central media warehouse.
- Keep Aletheia and Odysseus backstage; explain them only in About / technical documentation.
- Free-to-use for families, supported by useful resources, affiliate/referral income and possibly optional local-business listings.
- Do not call the organisation a charity/non-profit in the legal sense until a structure is actually chosen.

---

## Memorial creation

- Person / Pet as the two primary memorial classes.
- Optional species field for pets.
- No imposed "Rainbow Bridge" category or belief language.
- One cover image plus multiple gallery images.
- Multiple MP4/video memories.
- Audio/voice recordings.
- Scanned letters, drawings, PDFs and service sheets.
- "Suggest some words" button for users who want help.
- "I'll write it myself" always equally prominent.
- Prompt for funny, characteristic, affectionate memories rather than only dates and service details.
- Optional timeline of memories.
- Optional favourite songs/playlist links.
- Optional "things they always said" / phrases / nicknames.
- Optional recipes, hobbies, clubs, workplaces or causes.
- Optional memory contributions from invited friends/family.
- Moderated Book of Remembrance later.

---

## Portable memorial / family archive

- Canonical `memorial.md`.
- GEDCOM 7 import/export for family history.
- GEDZIP `.gdz` downloadable family archive.
- Aletheia Memorial Profile for predictable folder names and metadata.
- External URLs for very large video where a GEDZIP would become unwieldy.
- Optional encrypted family archive.
- "Restore this memorial" from a saved Markdown/GEDZIP.
- Import older GEDCOM/PAF-exported trees.
- Preserve source citations and provenance.
- Family should be able to leave RIP UK without losing its memorial.

---

## Distributed hosting

Offer guided choices rather than one mandatory host:

- Google Sites — complete memorial website.
- Google Drive — archive/folder/files.
- Google Photos — images/video album.
- Google My Maps — family/memorial map.
- OneDrive — shared archive/folder.
- YouTube — long video.
- Internet Archive — public archival option where appropriate.
- Own website/domain.
- Cloudflare Pages / GitHub Pages — technical users.
- Other URL supplied by family.

Create simple "How to publish for free" guides for each.

Possible future Odysseus actions:

- create folder structure
- test public sharing
- generate index page
- verify final URL
- detect broken links
- help migrate from one host to another

---

## Maps

- Each family can optionally create and control its own Google My Map.
- Family map can show meaningful places, not merely burial location.
- Categories: People, Pets, Cemeteries, Churchyards, War memorials, Historic graves.
- Optional regional RIP UK maps using opt-in memorial locations.
- Cemetery/history walking maps.
- Historic grave tours.
- "People connected to this place" view.
- Link family history from map points.
- Do not publish exact home burial location by default.
- Future MapLibre/OpenStreetMap layer only when scale or independence makes it worthwhile.

---

## Family history and genealogy

- GEDCOM/GEDZIP upload.
- FamilySearch links.
- FreeBMD/GRO/probate/parish-record research helpers.
- Historic churchyard records.
- Link several memorials into a family.
- Family map generated from genealogy locations.
- "Research this person" workflow rather than importing every deceased person.
- Optional external Ancestry/Findmypast/etc. links.
- Family tree view on human memorial pages.
- Aletheia companion/pet relationships shown separately from formal GEDCOM human relationships.
- PAF migration guide for older family archives.

---

## Resources and affiliates

Keep one calm **Resources** link in the public navigation.

### Grief and remembrance
- grief books
- audiobooks
- children's grief books
- pet-loss books
- bereavement organisations
- counselling directories
- remembrance journals

### Funerals and services
- funeral directors
- celebrants
- florists
- wake venues
- catering
- natural burial grounds
- cemeteries
- crematoria
- monumental masons/headstones
- probate/will services

### Pet aftercare
- vets
- home-burial guidance
- pet crematoria
- pet cemeteries
- urns
- stones/plaques
- keepsakes
- photo memorial products
- pet bereavement support

### Family history
- genealogy books
- archive services
- scanning
- photo restoration
- family-tree software/services

Principles:
- useful/free resource first;
- affiliate option second;
- clear disclosure;
- never rank solely by commission;
- local resources should use town/postcode where useful.

---

## Pet practical guides

Potential pages:

- My pet has died: what do I do now?
- Home burial: is it allowed where I live?
- Burial depth and groundwater considerations.
- What should I wrap my pet in?
- When not to bury at home.
- Cremation options.
- Individual vs communal cremation.
- Finding a pet cemetery.
- Creating a garden memorial.
- Children and pet loss.
- What to do if you rent or may move home.
- Moving a memorial when a family moves.

All burial guidance must be sourced, nation-specific and reviewed. Do not improvise advice about lime, chemicals or plastic.

---

## Social sharing

- Generate Facebook text.
- Generate LinkedIn text for professional/community memorials.
- WhatsApp/copyable short version.
- Social tribute card.
- OpenGraph image for external sharing.
- Link to existing Facebook/LinkedIn profile where the family chooses.
- Suggest a final memorial post, but never post automatically without explicit authorisation.
- RIP UK Facebook Page could share opt-in memorial notices and useful resources, but should not become the canonical archive.

---

## Registry and administration

- RIP ID for every registered memorial.
- Minimal public record.
- Private administrator email.
- Secure update/recovery mechanism.
- Administrator can change memorial URL without rebuilding record.
- Periodic link-health check.
- Email administrator when URL has failed repeatedly.
- Memorial status: active / moved / temporarily unavailable / archived.
- Transfer administration to another family member.
- Multiple administrators later.
- Deletion/delisting process.
- Abuse/fraud reporting.
- Sensitive-location controls.

---

## Look and feel

- Warm ivory/paper background.
- Sage/leaf green.
- Soft sky blue.
- Dusty rose/terracotta accents.
- Warm charcoal text.
- Large photos and stories.
- Minimal dashboard language.
- Optional family-selected themes later:
  - garden
  - coast
  - woodland
  - simple album
  - bright celebration
  - night sky
- Religious symbols/themes only when selected.
- Pet themes should not default to paw prints/dogs.

---

## Discovery

- Name search.
- Town search.
- Date/year.
- Person/Pet filter.
- Cemetery/churchyard links.
- Family connections.
- Map discovery.
- Search-engine-friendly public pages.
- Schema.org structured data research.
- `llms.txt` / AI-readable descriptions later.
- Public index should never leak administrator email.

---

## Site/business growth

- Cloudflare Pages initially without custom domain.
- Consider a dedicated domain only after the service proves useful.
- Recover historic Swindon.org.uk Google Business Profile separately where eligible.
- Do not create an ineligible Google Business Profile merely for a pin.
- Possible future RIP UK physical/development office only if it genuinely meets Google's in-person eligibility rules.
- Swindon.org.uk may link to RIP UK as a local project, but RIP UK remains its own service.

---

## Possible later features

- QR memorial plaques linking to RIP UK record.
- Printable memorial cards.
- NFC memorial tags.
- Cemetery walking tours.
- "On this day" memories.
- Family anniversaries/reminders.
- API/export for funeral directors.
- Funeral-director submission portal.
- Local-history society access.
- Church/cemetery curator tools.
- Volunteer transcription projects.
- AI-assisted old-photo restoration links/tools.
- Oral-history recorder.
- Audio transcription.
- Multilingual memorials.
- Legacy planning: create a draft memorial while alive, held private until released.

## Local help search

- Public label: **Find local help**, not A2Z.
- Reuse/generalise the Aletheia Local Search / Swindon.org.uk A2Z method.
- Ask for town/postcode once.
- Tick-box category search:
  - florists
  - funeral directors
  - cemeteries
  - crematoria
  - wake venues/catering
  - celebrants
  - memorial masons
  - probate/wills
  - bereavement support
  - pet crematoria/cemeteries
  - genealogy help
- Search nationally, while allowing Swindon.org.uk local data to contribute when relevant.
- Clear affiliate/sponsored labels.
- One primary book retailer initially: Bookshop.org UK.
- Consider a "near the funeral" search and a separate "near me" search later.


## Three-pass research completed (4 October 2026)

Reviewed BBC Ghosts for warm character-led humour, RIP.ie/MuchLoved/ForeverMissed, culturally diverse mourning and remembrance, GEDCOM/GEDZIP/PAF, and free-first pre-built local photo restoration. Findings and source references: [RIP-UK-Research.md](RIP-UK-Research.md). Research does not establish that the features are implemented, families consulted or browsers tested.
