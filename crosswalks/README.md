# Crosswalks

Mappings from these controls to the frameworks an enterprise already runs. This
directory is empty on purpose: **the first crosswalk should not come from us.**

Everyone who drafted this works for a vendor in the space. A mapping written from
inside carries our reading of both documents; one written by somebody who runs the
target framework in anger does not. That is why CONTRIBUTING names this as the
contribution we need most.

| Framework | Status | File |
|---|---|---|
| NIST AI RMF | proposed | `nist-ai-rmf.yaml` |
| ISO/IEC 42001 | proposed | `iso-42001.yaml` |
| OWASP | proposed | `owasp.yaml` |
| CIS Controls | proposed | `cis.yaml` |
| in-toto Attestation Framework | proposed | `in-toto.yaml` |
| EU AI Act | proposed | `eu-ai-act.yaml` |
| SOC 2 | proposed | `soc2.yaml` |
| NIST SP 800-53 | proposed | `nist-sp-800-53.yaml` |
| ISO/IEC 27001 | proposed | `iso-27001.yaml` |
| MITRE ATLAS | proposed | `mitre-atlas.yaml` |
| NIST SSDF | proposed | `nist-ssdf.yaml` |

## Filing one

One pull request per framework. A row per mapping, citing the bare identifier on
our side and the framework's own identifier on theirs:

```yaml
framework: NIST AI RMF
version: "1.0"
mappings:
  - control: DIS-01
    entries: [GOVERN-1.2, MAP-1.1]
    note: partial — ours requires a stable identifier, theirs does not
```

Partial and contested mappings are more useful than clean ones. If a control has
no counterpart, say so: that gap is a finding about one document or the other.
