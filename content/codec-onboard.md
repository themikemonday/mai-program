# Codec — Onboarding Sequence

The zones captured during the initial codec onboarding, in order. Invoked when the MAICODEC skill is called with `/MAICODEC onboard` (typically by MAISETUP as its final step).

---

## Sequence

1. **Identity** — `codec-identity.md`
2. **Capabilities** — `codec-capabilities.md`
3. **Environment** — `codec-environment.md`

Each zone runs through the standard zone-capture workflow (see the MAICODEC skill's `references/workflow.md`) in **Quick** mode.

After each zone completes, the skill offers: "Continue now, or pick this up later?" If the user chooses later, the remaining zones are preserved as unpopulated in the codec status table. The user can resume by running `/MAICODEC onboard` again or by invoking a specific zone directly with `/MAICODEC <zone>`.

---

## Zones not in onboarding

The following zones exist but are not part of the initial sequence:

- **Behaviour** — captured passively by the Revealed observer over session use.
- **Cognition** — observed from session content; not asked at onboarding.
- **Meaning** — captured in a follow-up session (heavier question set; not on the onboarding path).
- **Emotion** — captured in a follow-up session using Plutchik's four opposing pairs.

These can be worked on any time via `/MAICODEC <zone>` once their content files exist.
