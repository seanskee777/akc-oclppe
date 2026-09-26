# AKC-OCLPPE

**A**KC · **O**rphan · **C**hild · **L**ibrarian · **P**arent ·
**P**rovenance · **E**xecutioner

Status: **skeleton. Nothing works yet.** This repo exists so the idea is not
lost, and so the thinking can be argued with in the open.

## The idea

Every file and folder gets a permanent, tamper-evident identity: who made it,
when, what it became, where it travelled. Not a watermark *inside* the file —
that dies with the file, the first time it is re-encoded or screenshotted. The
proof lives in a **log**, and the log is what cannot be altered.

- **AKC** — the pedigree. A mutt still has documented ancestry, and so does a
  street-dog file nobody claims. Ownership and origin are not the same thing.
- **OCLPPE** — the states a file passes through: orphaned, claimed, catalogued,
  attributed, provenanced, terminated.

## The one part that is genuinely hard

Not the cryptography. The **propagation rule.**

If each machine holds a little fragment, the whole thing works and nobody can
rub it out — but a fragment can be forged, and then the chain is worthless. A
single shared notary is trustworthy but becomes a target and a single point of
failure. Every design lands somewhere on that line, and where you land decides
whether the thing is real.

## What already exists, and is not a competitor

| Need | Existing |
| --- | --- |
| Code authorship | Git signed commits, code signing |
| Build provenance | SLSA, in-toto, Sigstore |
| See where things go | SBOM (SPDX / CycloneDX) dependency graphs |
| Detect tampering | AIDE, Tripwire, OSSEC |
| AI-content marking | C2PA Content Credentials |
| Steganography | printer tracking dots, Word document tags |

AKC-OCLPPE is not "the first watermark." It is an attempt at the thing none of
those do: **one identity that follows a file across every machine it touches,
and a kill switch that is recorded rather than silent.**

## Ground rules

1. **Private by default.** No public ledger of who took what. A registry naming
   alleged thieves is a legal liability for the people whose files leak.
2. **Observe, do not snitch.** See what happened to a file. Nobody gets reported
   because they got caught.
3. **Local first.** Everything verifiable must work with no network.

## Licence

MIT. See `notes/licence.md` for why, and how to change it.

