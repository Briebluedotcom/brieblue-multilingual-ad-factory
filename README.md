# Brieblue Multilingual Ad Factory

> Created Oct 26, 2026, during the Meta Global AI Developer Hackathon
> (Oct 26 – Nov 4, 2026), under the Briebluedotcom GitHub account.

**Repo name:** `brieblue-multilingual-ad-factory`

## What this is

One master advertisement in, localized versions out — for a
one-person importer selling to customers in their own languages.
A micro business should be able to address every customer in their
own language, starting with one singular language advertisement and
eventually producing a global advertising campaign.

Sequence, in Ed's words: **1 Diwali, 2 Asian Festival, 3 the world.**
- **Diwali = the completed model** (pre-existing, see below).
- **Asian Festival = the project in motion** (May 2027 festival;
  expanding to all supported Asian languages).
- **The world = the eventual horizon** — access to the entire global
  economy for micro businesses around the world. Not a demoed claim.

Audience: San Antonio's heritage-language communities, and marketers
in Southeast Asia targeting multicultural linguistic citizens living
in different regions — including Asian marketers who currently use
English even in Asia, because everyone speaks a little of it. That
produces errors and lost messages. This is what the factory changes.

## Accessibility, demonstrated not claimed

Every localized version ships with:
- **Alt text** in the same language (for feed versions; Instagram
  reels have no manual alt-text field, so the descriptive wording
  goes in the caption), and
- **A spoken-audio version** in the same language, for customers who
  receive by ear, including illiterate customers.

Roots: Ed's blind uncle is behind the accessibility design, and he
already ships alt text on Brieblue's anniversary post.

## What is PRE-EXISTING (not hackathon-new, not demoed as new)

The following were built before Oct 26, 2026, and are inputs and
references only. The demo video must NOT present them as built
during the hackathon:

- **Diwali completed model** — for the Nov 7, 2026 Diwali San Antonio
  event: 10 Indian languages, each with a selected song (Hindi —
  "Jai Ho"; Bengali — "Le Paglu Dance"; Telugu — "Naatu Naatu";
  Marathi — "Zingaat"; Tamil — "Arabic Kuthu"; Gujarati — "Dholida";
  Urdu — "Pasoori"; Kannada — "Party Freak"; Malayalam —
  "Jimikki Kammal"; Punjabi — "Mundian To Bach Ke"). The Hindi ad
  itself was approved as final Oct 6, 2026, and stays in the
  organic / in-app licensed-audio lane for paid use.
- **Production-10 factory** — the original one-master-to-10-localized-
  versions pipeline (Vietnamese, Simplified Chinese, Tagalog,
  Korean, Thai, Hindi, Tamil, Telugu, Urdu, Japanese).
- **Song finder v1** — the fixed-source lookup (index, Freesound
  CC0/BY, public-domain melodies, Internet Archive secondary,
  AI fallback) and the music-bed database seed.
- **Demucs** — Meta's open-source stem-separation model
  (htdemucs), already in production in Ed's mixes; the audio
  parallel of SAM's picture isolation.

## What is HACKATHON-NEW (Oct 26 – Nov 4, 2026)

Work built during the hackathon window, and only this work is
demoed in the 3-minute demo video:

- **Factory v2** (`factory-v2-skeleton.py`, then
  `factory-v2-hindi.py`) — a model-agnostic pipeline: master ad in,
  localized versions out, each with alt text + spoken-audio script,
  behind a paid-use license gate. No version is releasable for paid
  use unless its music bed is verified.
- **Hindi license work** (`hindi-license-check-2026-10-26.md`,
  `hindi-license-verification-2026-10-26.md`) — Hindi is the gate.
  No Hindi bed is cleared for paid use until one candidate is
  verified end to end against the ingredient bar below.
- **Stress-test plan** (`stress-test-plan-2026-10-26.md`) — scale,
  music-finder coverage + license pass rate, rights audit, demo
  integrity, and production hold-up.
- **Asian language expansion list**
  (`asian-language-expansion-list-2026-10-26.md`) — the verified
  16-language union of the production 10 and the Diwali 10. This is
  NOT yet a claimed complete "all supported Asian languages" list;
  a Tier 3 check (Ads Manager pull + per-language fluency tests)
  is still required before that claim can be made.

## Music licensing — the ingredient bar (Ed, Oct 26)

A paid-use music bed must pass ALL of these. A site tag or a
marketing claim is never proof; the license/terms page must be read
and filed, per track:

- License is **PD, CC0, or CC BY only** — never CC BY-NC.
- Derivative works allowed AND commercial / paid-ad use allowed.
- Never a famous copyrighted performance. A public-domain
  composition in a famous recording still fails — the recording
  must also be free (obscure/CC0 version, or a re-performance
  we own).
- Remix does not erase recording rights.
- A usable unit is a familiar traditional fragment / melody / loop /
  stem, not a famous finished song.
- Vocal-on-vocal and mood/season mismatch are separate usability
  failures, even if a license passed.

**Status at Oct 26, 2026: 0 Hindi beds verified for paid use.**
See `hindi-license-verification-2026-10-26.md` for per-candidate
verdicts. Nothing expands on top of Hindi until one bed is verified.

## Models and credits used

Built on Meta's models via the Meta Model API (Muse Spark series;
Muse Wonder, Muse Image, SAM 3.1, Muse Voice Transcribe as the
kit allows), plus Meta open weights (Muse Glimmer, Muse Spark Open)
where they fit. Heavy generation runs on Meta Model API + partner
credits (their compute), not on Ed's Muse budget. No video model
and no music model is in the kit; Meta MusicGen output is CC BY-NC
and is OUT for paid ads.

## Submission

- Track: Startups Track (to be selected at submission; not
  pre-assigned — the submission form offers Indie Developer Track
  vs Startups Track as a choice).
- Problem statement: Build for Your World.
- Submission due: Wed Nov 4, 2026, 9 PM ET / 8 PM CT, via the
  Cerebral Valley submit form. One submission per team.
- Demo: 3-minute video, hackathon-new work only.
- Most Viral consideration (separate bonus, optional): post the
  project on X and include the X post link in the submission form.

## Status and limits (honest, as of Oct 26, 2026)

- Public repo: created Oct 26, 2026, under Briebluedotcom, starting with this README.
- Meta Model API live check: succeeded Oct 26, 2026 with the replacement credential (Meta Model Api V2), returning 9 models including muse-wonder-1.0, muse-spark-1.3, muse-image-1.0, sam-3.1, and muse-voice-transcribe-1.0. No generation call has been made and nothing has been spent yet.
- Spend Limit setting: not verified from the billing screenshot.
- Whether the $150 credits cover Wonder calls: not verified.
- Real master ad text: not yet supplied by Ed; the factory files
  use a clearly-marked SAMPLE invitation string only.
- Hindi music: 0 beds verified for paid use (see above).
