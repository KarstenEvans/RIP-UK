# RIP-UK Research: memorial traditions, Ghosts, genealogy and family photo repair

**Research date:** 2026-10-04. **Status:** three research/Improve iterations, NOT implemented functionality or live tests.  
**Canonical:** [RIP-UK.md](RIP-UK.md), [RIP-UK-Tasks.md](RIP-UK-Tasks.md), [RIP-UK-Ideas.md](RIP-UK-Ideas.md).  
**Protocols:** [Aletheia](https://github.com/KarstenEvans/aletheia-protocol) for provenance/uncertainty; [Thalia](https://github.com/KarstenEvans/thalia-protocol/blob/main/THALIA_PROTOCOL.md) optional respectful humour.

## Research method and three passes

**Improve pass 1: compare the working concept with established examples.** BBC British Ghosts, gentle eulogy humour, RIP.ie, MuchLoved and ForeverMissed. Key conclusion: a memorial is about recognizable character and memories, not only death logistics. Preserve basic one-paragraph memorial. Add optional descriptions/hobbies/interests/achievements and personal jokes.

**Walkabout: explore celebrations and commemorations outside UK/Irish memorial directories.** Looked at Hindu, Sikh, Thai Buddhist, Jewish, Muslim, secular, Irish, Indigenous Mexican, Japanese Obon, New Orleans jazz funeral and the Ga community of Ghana. Found prompts worth offering for music, favourite foods, symbolic items, annual dates, places lived and sharing family stories. Never create stereotyped preset based on surname, appearance, location or heritage.

**Improve pass 2: separate dimensions.** Writing tone is not the same as type of gathering. Offer a tone selector (Warm & Loving default; Reflective; Celebratory; Gentle Humour; Family Storytelling) and a distinct optional event selector (Wake, funeral, burial, cremation, remembrance, family gathering, private). Can mix tones, never force funny text or invent first-person quotes. Treat BBC Ghosts as creative analysis, not copyable characters, jokes, designs, images or show branding.

**Improve pass 3: compare available free-first tools and provenance/privacy.** Prefer local precompiled apps, preserve originals, disclose cloud photo uploads and AI invented details. Keep books/gifts and services on the optional Resources page. Record technical blockers (drive URL/CORS, security of imported GEDZIP, living relative info). Research/refinement occurred; these are NOT three deployed revisions.

## Evidence and design implications

### TV comedy and funeral writing

- [Ghosts, cast interviews](https://www.comedy.co.uk/tv/ghosts/interviews/series-4-q-and-as/): warm, character-led humour and an affectionate ensemble. [RTS interview](https://rts.org.uk/article/laurence-rickard-ghosts-series-five-kylie-minogue-and-emotional-double-whammy-christmas). Use genuine quirks and little habits to evoke the person rather than invent jokes. No copyrighted TV material.
- [How humour can work in a eulogy](https://funeral.com/blogs/the-journal/humor-in-a-eulogy-when-it-works-when-it-doesn-t-and-examples-of-safe-warmth): affectionate family-recognizable true incidents, not embarrassing or mocking jokes.
- [RIP.ie FAQ](https://rip.ie/faq?menu=181): acknowledgements, Month's Mind, anniversaries, birthday memorials and checked family notices. In RIP UK fold optional ongoing remembrance into one family-owned memorial Markdown instead of creating separate paid notices.
- [MuchLoved](https://funeralprofessionals.muchloved.com/features/tribute-pages/): after funeral, events can be archived and life memories remain central; charity, memories and contributions. [ForeverMissed](https://www.forevermissed.com/ourplans): stories, privacy, themes, collaborator roles and media. Learn functional patterns, do not clone websites.
- Suggested prompts: their favourite saying; what made you smile; the story everyone tells; recipes/food; favorite song; favorite club or place; proud achievement; private family stories; anniversary dates; optional family-confirmed charity and interest-based links. Blank sections do not render. When they say "none" it remains explicit. User words are primary.

### Traditions: ask first, offer researched optional modules

| Example | Possible questions, not a universal practice | Source |
|---|---|---|
| Irish/Christian wakes | Wake gathering, neighbours, stories, songs, food, Month's Mind or anniversary | [RTÉ, Sep 2026](https://www.rte.ie/brainstorm/2026/0908/1590683-ireland-death-wake-funeral-customs-traditions-food-bees-graveyard-clay/), [RIP.ie](https://rip.ie/faq?menu=181) |
| Hindu, including some Gujarati families | Antyesti, Om Shanti, prayer, Sraddha, annual rites, ashes customs according to family | [Hindu American Foundation](https://www.hinduamerican.org/blog/hindu-funerals-an-overview) |
| Sikh | Antam Sanskar, Ardas, music/prayers, gurdwara information if desired | [Funeral Guide](https://www.funeralguide.co.uk/help-resources/arranging-a-funeral/religious-funerals/sikh-funerals) |
| Thai Buddhist | Temple, chanting, monks, cremation and later merit-making dates if family practices them | [Thailand Foundation](https://www.thailandfoundation.or.th/culture_heritage/thai-funeral/) |
| Jewish | Shiva, Yahrzeit and family-selected remembrance, avoid universal florist prompts | [My Jewish Learning](https://www.myjewishlearning.com/article/shiva-what-you-need-to-know/) |
| Muslim | Janazah and family-arranged burial, charity; seek guidance from local mosque | [UK guide](https://www.afterloss.uk/guides/muslim-funeral-customs-uk) |
| Secular/humanist | Music, chosen readings, personal symbols and celebration | [Humanists UK](https://humanists.uk/ceremonies/old-non-religious-funerals/) |
| Indigenous Mexico Día de Muertos | Optional remembrance altars, flowers and favourite dishes, not a pan-Mexican default | [UNESCO](https://ich.unesco.org/en/RL/indigenous-festivity-dedicated-to-the-dead-00054?RL=00054) |
| Japan | Obon ancestral gatherings, grave visits, dances, yearly remembrance | [JNTO](https://www.japan.travel/en/guide/august/) |
| New Orleans | Jazz funeral can move from solemn procession to celebratory music | [New Orleans](https://www.neworleans.com/things-to-do/music/history-and-traditions/jazz-funeral/) |
| Ga community in Ghana | Designer coffins can represent professions and interests, but they are uncommon and not a universal Ghanaian practice | [Smithsonian](https://africa.si.edu/collection/object/nmafa_2004-2-1) |

**Implementation question (optional):** "Do you have any family tradition, favourite song, reading, prayer, food, place, anniversary or celebration you would like to include?" Provide Skip, Not sure, Write my own and Explore traditions. Allow languages/scripts. No faith auto-selection.

### Free-first photo restoration and animation; no compilation

| Tool | Reality | Source |
|---|---|---|
| PhotoDemon | Free/open source Windows portable ZIP application, edits offline without installation, no compiling | https://photodemon.org/download/ |
| GIMP | Free open-source packaged desktop builds Win/macOS/Linux, heal/clone, manual repair | https://www.gimp.org/downloads/ |
| Upscayl | Open-source Windows/macOS/Linux installers, local AI upscaling, suitable Vulkan GPU needed, output may hallucinate | https://github.com/upscayl/upscayl |
| Canva | Browser image restoration and colorizing, some free and some paid/Pro features, uploaded images go to service | https://www.canva.com/features/photo-restoration/ |
| CapCut | Browser old-photo restoration including scratches and colorization, marketed free, check actual tier and privacy | https://www.capcut.com/tools/old-photo-restoration |
| MyHeritage Deep Nostalgia | The remembered **2021** animation technology: blink, turn head, smile; free trials limited with account/potential subscription and cloud processing | https://blog.myheritage.com/2021/02/new-animate-the-faces-in-your-family-photos/ |

Best process: scan original at high quality (UK National Archives photo preservation suggests ~600 PPI minimum), preserve an untouched scan; create copies labelled restored, colourised (inferred colours), or AI-animated (simulated motion). Family selects what is public. Keep originals. Do not present synthetic speech as genuine final words. References: https://www.nationalarchives.gov.uk/information-management/manage-information/preserving-digital-records/digitisation/ and https://blog.myheritage.com/2021/02/new-animate-the-faces-in-your-family-photos/.

### Family history: PAF, GEDCOM and GEDZIP

- Historical LDS Personal Ancestral File (PAF) was discontinued in 2013; to move historical records, use a migration-capable third-party program to export GEDCOM. https://www.familysearch.org/en/help/helpcenter/article/can-i-get-a-copy-of-personal-ancestral-file-paf
- GEDZIP 7 is ZIP-based but NOT arbitrary ZIP: required file **gedcom.ged**, plus locally referenced attachments. The optional memorial.md must be properly referenced through GEDCOM or be in a parallel standard family-backup ZIP; test compatibility. https://github.com/FamilySearch/GEDCOM/blob/main/specification/gedcom-4-gedzip.md
- [Topola Viewer](https://pewu.github.io/topola-viewer) supports loading GEDCOM / GEDZIP in browser, states it keeps user-supplied files local. [Gramps Web](https://www.grampsweb.org/) is open source but its hosting/setup needs more technical skill. Avoid recommending software that ordinary users must compile.
- https://www.familysearch.org/en/help/helpcenter/article/how-do-i-use-familysearch-memories-to-preserve-my-ancestors-life-stories provides an optional external link for ancestor records, stories, photos and audio; https://www.familysearch.org/en/gettingstarted/ offers free tutorials and centres.
- For RIP-UK: optional verified FamilySearch person URL, external family-tree URLs, GEDCOM/ZIP URL, related RIP IDs, source references, evidence confidence, living-relative privacy. Do not auto-merge people based on names alone.

### Optional books, gifts and resources

- Free-first genealogy classes: https://www.familysearch.org/en/rootstech/getting-started
- National Archives shop catalogue includes How to Get The Most from Family Pictures and Sharing Your Family History Online, and location-specific ancestry guides; link based on genuine interests and consider library lending before shops: https://shop.nationalarchives.gov.uk/collections/for-beginners-family-history
- Optional gift guides: family-created book of stories, photo album, acid-free archival sleeves, clearly labelled restored print, or local printed recipe collection. Family’s explicit charity/beneficiary link takes precedence. Keep gifts/affiliate items OFF the memorial’s emotional reading surface; use RIP-UK-rsc.htm with plain disclosures.
- Do not imply recommendations are items the deceased owned/loved unless family said so.

## Implementation acceptance gates

1. A name and a two-line description is sufficient to create a memorial; all other sections can be empty.
2. Tone/event are distinct optional fields; affectionate humour uses family-supplied facts and is always previewed.
3. The family hosts Markdown and media and holds ZIP backups; RIP UK keeps only minimal registry index/locator data.
4. Public Google Drive/OneDrive URL validation must check raw file access vs browser preview and CORS; never claim untested working embeds.
5. Imported GEDCOM/GEDZIP files require privacy filtering for living relatives and archive security tests (path traversal and zip bombs).
6. Original photos are kept and AI-altered images labelled visibly; keep the private originals. No auto-generated speaking avatar claiming genuine deceased words.
7. Legal/privacy review for living-person references, copyright, contact details and consent still required even for a pointer-only register.
8. Do not commit/publish the private Dinesh Gohil example without family authorisation.
9. Preserve existing ChatGPT-built RIP UK styling and eight-step flow until the PC ZIP is supplied and inspected.
10. Follow [Aletheia Improve](https://github.com/KarstenEvans/aletheia-app/blob/main/aletheia-improve/aletheia-improve.md): refresh source, read files, propose, test, publish only with approval.
