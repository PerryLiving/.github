# Perry

**Perimenopause, tracked. Privacy, non-negotiable.**

Perry is a perimenopause and HRT tracking app for iPhone. It records symptoms,
medications and hormone replacement therapy schedules, cycles, sleep, and labs —
then lines up what you felt against what your body was actually doing, and turns
that into something you can hand to a clinician.

No VC money. No ads. No wellness cosplay.

→ **[perry.living](https://perry.living)**

---

## What it tracks

- **Symptoms** — 54 curated symptoms across 8 groups, logged in seconds by tap or voice, with severity and backdating.
- **Medications and HRT** — gel rotations, patch schedules, oral and vaginal progesterone, cyclical and continuous regimens, luteal SSRIs. Dose logging and local reminders.
- **Cycles and periods** — cycle day, phase estimates, regularity as numbers with windows rather than verdicts.
- **Sleep and vitals** — from Apple Health, Apple Watch, Oura, or Whoop.
- **Labs** — entered by hand, imported from Apple Health Records, or read from a Mira home hormone report.
- **Journal** — free text or on-device dictation, kept as narrative rather than forced into a coded field.

Bring your history in from Apple Health, Samsung Health, Clue, Flo, or Natural Cycles:
**[perry.living/import](https://perry.living/import/)**

## Where the privacy line sits

Perry never asks your real name — a nickname is all it wants. What you track is kept
separate from who you are, and the appointment summary you hand a doctor carries no
name and no date of birth. Your data is never sold, never shared for advertising, and
never handed to data brokers, insurers, or employers.

- **[Privacy Notice](https://perry.living/privacy/)**
- **[Terms of Use](https://perry.living/terms/)**

## Built on

Clinical data is stored as a **FHIR R4** record in Google Cloud Healthcare, encrypted
in transit and at rest, in the user's own region. Coding is verified rather than
guessed — **SNOMED CT** for symptoms, **LOINC** for observations and labs, **RxNorm**
(and **dm+d**, **AEMPS CIMA**) for medications, **ICD-11/10** for conditions, **UCUM**
for units. The app talks to auth-gated Cloud Functions and never holds infrastructure
credentials itself.

The domain engine is a pure-Swift package with no UI, no clock, and no persistence, so
schedule and cycle logic can be tested exhaustively against DST shifts, month
boundaries, and cycle transitions.

## Reading

- **[Guides](https://perry.living/track/)** — what to track, and why it matters
- **[Lab reference](https://perry.living/labs/)** — estradiol, FSH, ferritin, thyroid, and the rest, in plain English
- **[FAQ](https://perry.living/faq/)** — perimenopause itself, plus how the app works
- **[Notes](https://perry.living/blog/)** — founder notes from the build

## Repositories

Perry's app and site repositories are private while it is in private beta.

## Contact

Perry is built and supported by one person.

- General and support — **eiei@perry.living**
- Data rights and privacy — **privacy@perry.living**
- **[Join the waitlist](https://perry.living/#waitlist)** for early access
