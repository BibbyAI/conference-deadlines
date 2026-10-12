# Conference Deadlines

Open, PR-maintained YAML of academic conference deadlines across **CS / AI / ML, neuroscience, physics and math**. Submission, rebuttal, notification and camera-ready dates, with timezones that are actually correct.

**Browse it with filters and live countdowns: [trybibby.com/conference-deadlines](https://trybibby.com/conference-deadlines)**

Found a wrong date? [Open an issue](../../issues/new/choose) or send a PR, see [CONTRIBUTING.md](CONTRIBUTING.md).

## Use the data

**Calendar (auto-updates):** subscribe in Google Calendar / Apple Calendar / Outlook via "Add calendar from URL":

| Calendar | URL |
|---|---|
| Everything | `https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/all.ics` |
| CS / AI / ML | `https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/cs.ics` |
| Neuroscience | `https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/neuro.ics` |
| Physics | `https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/phys.ics` |
| Math / Theory | `https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/math.ics` |

**JSON:** `dist/conferences.json` (all) and `dist/upcoming.json` (future only), one object per deadline:

```bash
curl -s https://raw.githubusercontent.com/OWNER/conference-deadlines/main/dist/upcoming.json \
  | jq '.[] | select(.tags | index("ML")) | "\(.deadline)  \(.name)  \(.deadlineLabel)"'
```

**YAML:** `data/<field>/<id>.yaml`, one file per conference series. Schema: [`schema/conference.schema.json`](schema/conference.schema.json).

```yaml
id: iclr
name: ICLR
field: CS
tags: [ML, AI]
tier: A*
editions:
- year: 2027
  title: Int'l Conf. on Learning Representations
  venue: California, USA
  dates: Apr/May 2027
  url: https://iclr.cc/
  deadlines:
  - {label: Abstract, date: '2026-09-18T23:59:59-12:00'}
  - {label: Full Paper, date: '2026-09-25T23:59:59-12:00'}
```

## Tags

`AI` artificial intelligence, `ML` machine learning, `CV` computer vision, `NLP` language, `RO` robotics, `SP` speech and signal processing, `DM` data mining and IR, `DB` databases, `HCI` human-computer interaction, `PL` programming languages and SE, `SEC` security and crypto, `SYS` systems and architecture, `GFX` graphics, `NEURO`, `PHYS`, `MATH`.

## Upcoming deadlines

Rebuilt daily by CI from `data/`. Times are UTC. AoE (anywhere on earth) deadlines show as 11:59 the next day in UTC.

<!-- DEADLINES:START -->
_114 upcoming deadlines, updated 2026-10-12 UTC._

| Deadline (UTC) | Days | Conference | What | Field | Tier |
|---|---:|---|---|---|---|
| 2026-10-12 11:59 | 0 | [ACM WebConf 2027](https://acmweb2027.org/) | Abstract | CS | A* |
| 2026-10-12 11:59 | 0 | [EACL 2027](https://2027.eacl.org/) | Commit | CS | A |
| 2026-10-13 11:59 | 1 | [CoRL 2026](https://www.corl.org/contributions/instruction-for-authors) | Camera-Ready | CS | A |
| 2026-10-13 11:59 | 1 | [NAACL 2027](https://2027.naacl.org/) | ARR Commit | CS | A* |
| 2026-10-14 11:59 | 2 | [KDD 2027](https://kdd.org/) | Rebuttal Ends R1 | CS | A* |
| 2026-10-16 11:59 | 4 | [ICDE 2027](https://icde2027.github.io/) | Round 2 *(tentative)* | CS | A* |
| 2026-10-16 11:59 | 4 | [NeurIPS 2026](https://neurips.cc/Conferences/2026/Dates) | Rebuttal Ends | CS | A* |
| 2026-10-19 11:59 | 7 | [ACM WebConf 2027](https://acmweb2027.org/) | Full Paper | CS | A* |
| 2026-10-19 11:59 | 7 | [SIGMOD 2027](https://2027.sigmod.org/) | Round 4 | CS | A* |
| 2026-10-20 11:59 | 8 | [AAAI 2027](https://aaai.org/conference/aaai/aaai-27/paper-publication-and-conference-attendance/) | Feedback Opens | CS | A* |
| 2026-10-21 11:59 | 9 | [ROBOT 2026](https://robot2026.upc.edu/) | Final Paper | CS | B |
| 2026-10-22 21:00 | 10 | [APS Summit 2027](https://www.aps.org/events/2027/summit) | Abstract *(tentative)* | PHYS | A* |
| 2026-10-22 23:59 | 10 | [MRS Spring 2027](https://www.mrs.org/spring-meetings-exhibits) | Abstract *(tentative)* | PHYS | A |
| 2026-10-25 11:59 | 13 | [NeurIPS 2026](https://neurips.cc/Conferences/2026/Dates) | Camera-Ready | CS | A* |
| 2026-10-26 11:59 | 14 | [AAAI 2027](https://aaai.org/conference/aaai/aaai-27/paper-publication-and-conference-attendance/) | Feedback Closes | CS | A* |
| 2026-10-27 11:59 | 15 | [Humanoids 2026](https://2026.ieee-humanoids.org/) | Camera-Ready | CS | A |
| 2026-10-28 11:59 | 16 | [FAccT 2027](https://facctconference.org/2027/cfp.html) | Abstract | CS | A |
| 2026-10-31 11:59 | 19 | [IAAI 2027](https://aaai.org/conference/aaai/aaai-27/) | Notification | CS | A |
| 2026-10-31 11:59 | 19 | [MLSys 2027](https://mlsys.org/) | Paper *(tentative)* | CS | A |
| 2026-11-01 11:59 | 20 | [AAAI 2027](https://aaai.org/conference/aaai/aaai-27/journal-track-call-for-papers/) | Journal Track | CS | A* |
| 2026-11-02 04:59 | 20 | [CNS 2027](https://www.cogneurosociety.org/) | Abstract *(tentative)* | NEURO | A |
| 2026-11-03 11:59 | 22 | [WACV 2027](https://wacv.thecvf.com/) | Camera-Ready | CS | A |
| 2026-11-04 00:59 | 22 | [STOC 2027](https://acm-stoc.org/) | Paper *(tentative)* | MATH | A* |
| 2026-11-04 06:59 | 23 | [SPIE DCS 2027](https://spie.org/conferences-and-exhibitions/defense-and-commercial-sensing) | Abstract *(tentative)* | PHYS | A |
| 2026-11-04 11:59 | 23 | [FAccT 2027](https://facctconference.org/2027/cfp.html) | Full Paper | CS | A |
| 2026-11-05 07:59 | 24 | [ISMRM 2027](https://www.ismrm.org/) | Abstract *(tentative)* | NEURO | A |
| 2026-11-06 11:59 | 25 | [CHI 2027](https://chi2027.acm.org/) | Reviews Released | CS | A* |
| 2026-11-06 11:59 | 25 | [ICLR 2027](https://iclr.cc/) | Reviews Released | CS | A* |
| 2026-11-06 11:59 | 25 | [PLDI 2027](https://pldi27.sigplan.org/) | Round 1 *(tentative)* | CS | A* |
| 2026-11-08 07:59 | 27 | [CVPR 2027](https://cvpr.thecvf.com/) | Abstract Reg. | CS | A* |
| 2026-11-13 07:59 | 32 | [CVPR 2027](https://cvpr.thecvf.com/) | Full Paper *(tentative)* | CS | A* |
| 2026-11-15 11:59 | 34 | [KDD 2027](https://kdd.org/) | Notification R1 | CS | A* |
| 2026-11-15 23:59 | 34 | [IPCO 2027](https://ipco2027.github.io/) | Paper *(tentative)* | MATH | A |
| 2026-11-18 11:59 | 37 | [S&P 2027](https://sp2027.ieee-security.org/) | Cycle 2 Paper | CS | A* |
| 2026-11-19 07:59 | 38 | [Cosyne 2027](https://www.cosyne.org/) | Abstract *(tentative)* | NEURO | A |
| 2026-11-19 11:59 | 38 | [ICLR 2027](https://iclr.cc/) | Discussion Ends | CS | A* |
| 2026-11-20 07:59 | 39 | [CVPR 2027](https://cvpr.thecvf.com/) | Supplementary *(tentative)* | CS | A* |
| 2026-11-23 11:59 | 42 | [ISCA 2027](https://www.iscaconf.org/isca2027/submit/papers.php) | Paper *(tentative)* | CS | A* |
| 2026-11-25 23:59 | 44 | [ARVO 2027](https://www.arvo.org/annual-meeting/) | Abstract *(tentative)* | NEURO | A |
| 2026-12-01 11:59 | 50 | [AAAI 2027](https://aaai.org/conference/aaai/aaai-27/paper-publication-and-conference-attendance/) | Final Notification | CS | A* |
| 2026-12-03 05:00 | 51 | [VSS 2027](https://www.visionsciences.org/) | Abstract *(tentative)* | NEURO | A |
| 2026-12-04 11:59 | 53 | [CHI 2027](https://chi2027.acm.org/) | Revise & Resubmit | CS | A* |
| 2026-12-05 11:59 | 54 | [MobiSys 2027](https://www.sigmobile.org/mobisys/2027/) | Paper *(tentative)* | CS | A* |
| 2026-12-08 22:00 | 57 | [CLEO 2027](https://www.cleoconference.org/) | Paper Summary *(tentative)* | PHYS | A |
| 2026-12-09 11:59 | 58 | [OSDI 2027](https://www.usenix.org/conference/osdi27) | Paper *(tentative)* | CS | A* |
| 2026-12-11 11:59 | 60 | [ACM WebConf 2027](https://acmweb2027.org/) | Results | CS | A* |
| 2026-12-13 11:59 | 62 | [ACM WebConf 2027](https://acmweb2027.org/) | Rebuttal Opens | CS | A* |
| 2026-12-15 04:59 | 63 | [OHBM 2027](https://humanbrainmapping.org/) | Abstract *(tentative)* | NEURO | A |
| 2026-12-15 11:59 | 64 | [AAAI 2027](https://aaai.org/conference/aaai/aaai-27/paper-publication-and-conference-attendance/) | Camera-Ready | CS | A* |
| 2026-12-16 04:59 | 64 | [SIAM AN 2027](https://www.siam.org/conferences/) | Abstract *(tentative)* | MATH | A |
| 2026-12-16 11:59 | 65 | [ICME 2027](https://2027.ieeeicme.org/) | Paper *(tentative)* | CS | A |
| 2026-12-17 11:59 | 66 | [ICLR 2027](https://iclr.cc/) | Reviewer/AC Ends | CS | A* |
| 2026-12-17 11:59 | 66 | [ICLR 2027](https://iclr.cc/) | Final Decisions | CS | A* |
| 2026-12-20 11:59 | 69 | [ACM WebConf 2027](https://acmweb2027.org/) | Rebuttal Ends | CS | A* |
| 2026-12-22 11:59 | 71 | [AAMAS 2027](https://www.aamas-conference.org/) | Notification | CS | A |
| 2026-12-24 11:59 | 73 | [COLING 2027](https://2027.coling-iccl.org/) | ARR Commit | CS | A* |
| 2027-01-16 11:59 | 96 | [CCS 2027](https://www.sigsac.org/ccs/CCS2027/) | Cycle 1 Paper *(tentative)* | CS | A* |
| 2027-01-16 11:59 | 96 | [CSCW 2027](https://cscw.acm.org/2027/) | Winter Cycle *(tentative)* | CS | A |
| 2027-01-16 11:59 | 96 | [MIDL 2027](https://2027.midl.io/) | Paper *(tentative)* | CS | A |
| 2027-01-16 11:59 | 96 | [MobiCom 2027](https://www.sigmobile.org/mobicom/2027/cfp.html) | Cycle 2 Paper *(tentative)* | CS | A* |
| 2027-01-17 11:59 | 97 | [CEC 2027](https://cis.ieee.org/conferences/conference-calendar) | Full Paper *(tentative)* | CS | B |
| 2027-01-19 11:59 | 99 | [NAACL 2027](https://2027.naacl.org/) | Notification *(tentative)* | CS | A* |
| 2027-01-20 11:59 | 100 | [IJCAI 2027](https://www.ijcai.org/) | Paper *(tentative)* | CS | A* |
| 2027-01-21 22:00 | 101 | [SIGGRAPH 2027](https://s2027.siggraph.org/) | Stage 1 Paper | CS | A* |
| 2027-01-23 11:59 | 103 | [SIGIR 2027](https://sigir2027.org/) | Paper *(tentative)* | CS | A* |
| 2027-01-23 11:59 | 103 | [USENIX ATC 2027](https://www.usenix.org/conference/atc27) | Paper *(tentative)* | CS | A |
| 2027-01-23 11:59 | 103 | [CCC 2027](https://computationalcomplexity.org/) | Paper *(tentative)* | MATH | A |
| 2027-01-27 11:59 | 107 | [USENIX Security 2027](https://www.usenix.org/conference/usenixsecurity27) | Cycle 2 Paper | CS | A* |
| 2027-01-28 23:59 | 108 | [SIGCOMM 2027](https://conferences.sigcomm.org/sigcomm/2027/) | Paper *(tentative)* | CS | A* |
| 2027-01-29 11:59 | 109 | [ICML 2027](https://icml.cc/) | Paper *(tentative)* | CS | A* |
| 2027-02-01 11:59 | 112 | [ACM WebConf 2027](https://acmweb2027.org/) | Final Version | CS | A* |
| 2027-02-01 11:59 | 112 | [ICDAR 2027](https://icdar2027.org/call-for-papers) | Abstract | CS | A |
| 2027-02-01 11:59 | 112 | [RSS 2027](https://roboticsconference.org/) | Paper *(tentative)* | CS | A* |
| 2027-02-01 23:59 | 112 | [JSM 2027](https://ww2.amstat.org/meetings/jsm/2027/) | Abstract *(tentative)* | MATH | A |
| 2027-02-02 11:59 | 113 | [ICIP 2027](https://2027.ieeeicip.org/) | Paper *(tentative)* | CS | A |
| 2027-02-04 06:59 | 115 | [SPIE OP 2027](https://spie.org/conferences-and-exhibitions/optics-and-photonics) | Abstract *(tentative)* | PHYS | A |
| 2027-02-05 11:59 | 116 | [COLT 2027](https://learningtheory.org/) | Paper *(tentative)* | CS | A* |
| 2027-02-05 22:00 | 116 | [APS DAMOP 2027](https://www.aps.org/units/damop/) | Abstract *(tentative)* | PHYS | A |
| 2027-02-06 11:59 | 117 | [UAI 2027](https://www.auai.org/uai2027/) | Paper *(tentative)* | CS | A |
| 2027-02-09 11:59 | 120 | [ICSE 2027](https://conf.researchr.org/home/icse-2027) | Cycle 2 Paper *(tentative)* | CS | A* |
| 2027-02-11 11:59 | 122 | [CCN 2027](https://ccneuro.org/) | Paper *(tentative)* | NEURO | A |
| 2027-02-13 11:59 | 124 | [ICALP 2027](https://www.eatcs.org/) | Paper *(tentative)* | MATH | A |
| 2027-02-15 23:59 | 126 | [Neuromatch 2027](https://neuromatch.io/) | Abstract *(tentative)* | NEURO | B |
| 2027-02-16 11:59 | 127 | [ACL 2027](https://www.aclweb.org/) | ARR *(tentative)* | CS | A* |
| 2027-02-21 11:59 | 132 | [ICDAR 2027](https://icdar2027.org/call-for-papers) | Full Paper | CS | A |
| 2027-02-26 07:59 | 137 | [MICCAI 2027](https://miccai.org/) | Paper *(tentative)* | CS | A |
| 2027-03-02 11:59 | 141 | [IROS 2027](https://www.iros.org/) | Paper *(tentative)* | CS | A |
| 2027-03-04 11:59 | 143 | [INTERSPEECH 2027](https://www.isca-speech.org/) | Paper (est.) *(tentative)* | CS | A |
| 2027-03-06 07:59 | 145 | [ICCV 2027](https://iccv.thecvf.com/) | Paper *(tentative)* | CS | A* |
| 2027-03-14 11:59 | 153 | [ASPLOS 2027](https://www.asplos-conference.org/asplos2027/cfp/) | Fall Paper *(tentative)* | CS | A* |
| 2027-03-16 11:59 | 155 | [AutoML 2027](https://2027.automl.cc/) | Paper *(tentative)* | CS | A |
| 2027-03-16 11:59 | 155 | [RLC 2027](https://rl-conference.cc/) | Paper *(tentative)* | CS | A |
| 2027-03-31 11:59 | 170 | [COLM 2027](https://colmweb.org/) | Paper *(tentative)* | CS | A |
| 2027-04-06 23:59 | 176 | [FOCS 2027](https://focs.computer.org/) | Paper *(tentative)* | MATH | A* |
| 2027-04-09 11:59 | 179 | [ACM MM 2027](https://2027.acmmm.org/) | Paper *(tentative)* | CS | A* |
| 2027-04-09 11:59 | 179 | [UIST 2027](https://uist.acm.org/2027/) | Paper *(tentative)* | CS | A* |
| 2027-04-16 11:59 | 186 | [MICRO 2027](https://microarch.org/) | Paper *(tentative)* | CS | A* |
| 2027-04-16 11:59 | 186 | [OOPSLA 2027](https://2027.splashcon.org/) | Round 1 *(tentative)* | CS | A* |
| 2027-04-16 11:59 | 186 | [EPS-HEP 2027](https://www.eps-hepp.eu/) | Abstract *(tentative)* | PHYS | A |
| 2027-04-21 11:59 | 191 | [SSW 2027](https://www.isca-speech.org/) | Paper | CS | B |
| 2027-04-25 11:59 | 195 | [RecSys 2027](https://recsys.acm.org/recsys27/) | Paper *(tentative)* | CS | A |
| 2027-05-05 23:59 | 205 | [APPROX/RANDOM 2027](https://approxrandom2027.github.io/) | Paper *(tentative)* | MATH | A |
| 2027-05-16 11:59 | 216 | [NeurIPS 2027](https://neurips.cc/) | Paper *(tentative)* | CS | A* |
| 2027-05-22 11:59 | 222 | [CIKM 2027](https://cikm2027.org/) | Paper *(tentative)* | CS | A |
| 2027-05-29 11:59 | 229 | [CoRL 2027](https://www.corl.org/) | Paper *(tentative)* | CS | A |
| 2027-05-29 11:59 | 229 | [EMNLP 2027](https://2027.emnlp.org/) | ARR *(tentative)* | CS | A* |
| 2027-06-06 11:59 | 237 | [ICDM 2027](https://icdm2027.org/) | Paper *(tentative)* | CS | A* |
| 2027-06-09 21:00 | 240 | [SfN 2027](https://www.sfn.org/) | Abstract *(tentative)* | NEURO | A* |
| 2027-06-16 11:59 | 247 | [AACL-IJCNLP 2027](https://www.aacl2027.org/) | ARR *(tentative)* | CS | A |
| 2027-06-24 23:59 | 255 | [MRS Fall 2027](https://www.mrs.org/meetings-events/fall-meetings-exhibits) | Abstract *(tentative)* | PHYS | A |
| 2027-07-07 23:59 | 268 | [SODA 2028](https://www.siam.org/conferences/cm/conference/soda28) | Paper *(tentative)* | MATH | A* |
| 2027-07-14 21:00 | 275 | [APS DPP 2027](https://www.aps.org/units/dpp/meetings/) | Abstract *(tentative)* | PHYS | A |
| 2027-07-30 21:00 | 291 | [APS DFD 2027](https://dfd-meeting.aps.org/) | Abstract *(tentative)* | PHYS | A |
| 2028-01-15 23:59 | 460 | [FENS Forum 2028](https://forum2028.fens.org/) | Abstract *(tentative)* | NEURO | A* |
<!-- DEADLINES:END -->

## Local

```bash
pip install -r requirements.txt
python scripts/validate.py   # schema + sanity checks
python scripts/build.py      # dist/*.json, dist/*.ics, README table
```

## Disclaimer

Dates change. Always confirm on the official conference site before you submit. `tentative` means estimated or not yet announced.

## License

Data: [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/), credit this repo if you reuse it. Code: MIT. See [LICENSE](LICENSE).

Maintained by [Bibby AI](https://trybibby.com), the LaTeX-native AI research writing platform.
