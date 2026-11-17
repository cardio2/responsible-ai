# Responsible AI at Cardio2

How the AI in [Cardio2](https://cardio2.info) is designed: what it does, what it does not do and the rules we follow.

**AI that explains. Rules that protect.**

> **Stage:** Cardio2 is in development. It is not yet certified as a medical device (no CE marking yet) and cannot be used for treatment yet. This document describes how we are designing the product, not a finished, certified system.
>
> In an emergency, call **112**.

Cardio2 is an AI companion for people recovering at home after a heart attack, a stent, heart surgery or a heart failure diagnosis. We keep two jobs strictly apart. AI reads documents, explains and motivates. A separate set of fixed medical rules, tested like any medical software, decides when something is dangerous. These rules run before the AI and always give the same result.

## What the AI does

| Capability | What it means | Stage |
| --- | --- | --- |
| Reads discharge letters | Text recognition and AI turn a photo or PDF into a clear list of diagnoses, medicines and restrictions, which a nurse then confirms. | In the first version |
| Explains in plain language | Turns medical guidelines into short, calm answers that are easy to read, in the patient's own language. | In the first version |
| Writes the doctor's report | Sums up a month of measurements, events and medicine-taking on one page. Every figure can be traced back to the original measurement. | In the first version |
| Adapts the programme | Adjusts walking and exercise to check-in answers, heart rate and how hard it feels, within the limits set by the doctor. | Planned |
| Supports healthy habits | Proven motivation techniques for medicines, activity, food and quitting smoking, at the moments when people usually give up. | Planned |
| Spots worsening early | An early-warning model for heart failure, based on changes in weight, pulse and activity. It will be tested and validated before any use in care. | In research |

## What the AI does not do

These are safety rules we will never give up:

- The AI never starts, stops or changes a medicine or a dose.
- Danger signs are handled by fixed rules, never by AI.
- An answer without a source that can be checked is never shown.
- Every AI update must pass a test of more than 1,000 real clinical situations, reviewed by cardiologists.
- Every AI answer is recorded so it can be checked later, as required for medical devices.
- AI services run on servers in the EU under data protection contracts. Patient data is never used to train other companies' AI.

Cardio2 is also:

- **Not an emergency service.** In an emergency, call 112.
- **Not a diagnosis tool.** It does not tell people what illness they have.
- **Not a replacement for the cardiologist.** It supports the treatment plan the doctor has set.

## How each piece of information is handled

1. **Input:** check-in answers, data from devices, a photo of the discharge letter or a question.
2. **Safety check:** fixed rules approved by our clinical advisory board are checked first.
3. **AI with sources:** the AI answers only from a checked medical library based on official guidelines.
4. **Safety limits:** every answer must name its source. Off-topic or unsupported answers are blocked.
5. **Medical team:** nurses and doctors approve plans and review warning alerts.

If a danger sign appears, the person sees an emergency screen with a button to call 112, the family contact is notified and the AI chat pauses.

### Four levels of response

| Level | Examples of triggers | What happens |
| --- | --- | --- |
| Red | Chest pain lasting more than 5 minutes, sudden severe breathlessness, fainting, signs of a stroke | A full-screen "Call 112 now" message, a one-tap call button, and the family contact is notified. The AI chat pauses. |
| Orange | In heart failure: weight up 2 kg in 3 days. Blood pressure or resting pulse outside the limits set by the doctor | A nurse or doctor is notified the same working day. The patient gets clear instructions on what to do until they call. |
| Yellow | Medicines missed for 2 days or more, low mood, stopped exercising | Gentle encouragement, an offer to talk to a specialist, and a note in the doctor's report. |
| Green | Everything is going to plan | Encouragement and the next step of the programme. |

The limits are set by the patient's own doctor and approved by our clinical advisory board.

## Who decides

- **Clinical advisory board:** cardiologists, rehabilitation specialists and a patient representative approve all medical rules and limits. We are forming this board now.
- **People in charge:** a nurse approves every recovery plan and responds to orange alerts. Only the patient's doctor can change medicines.
- **Ongoing safety checks:** every alert and every AI answer is recorded and regularly reviewed for problems.
- If in doubt, a person decides. Always.

## Data and consent

- Health data in the Cardio2 app will be processed only with the patient's explicit consent or for the care they receive (GDPR Art. 9).
- Data is stored in the EU, encrypted, and only what is necessary is collected.
- The patient, the medical team they choose and, only with the patient's permission, their family can see the data.
- We do not sell data or advertising. Patient data is never used to train other companies' AI.

## Rules we are building for

| Rule or standard | Our goal |
| --- | --- |
| EU MDR 2017/745 | Certification as Class IIa medical software, checked by an independent certification body, with CE marking |
| EU AI Act | Requirements for high-risk AI built in from the first version: data quality checks, human oversight, transparency and record-keeping |
| ISO 13485 | Quality management system |
| IEC 62304 · ISO 14971 · IEC 62366 | International standards for building medical software, managing risks and making it easy to use |
| GDPR · ISO 27001 | Data protection by design; ISO 27001 information security certification planned |
| HL7 FHIR | Data exchange compatible with the European Health Data Space |

## Quality goals for the AI

- 1,000+ clinical test situations reviewed by cardiologists before every update
- 100% of medical answers show their source; otherwise they are not shown at all
- 0 medicine or dose changes made by AI
- Below 5% false emergency alerts, as a target for the first clinical study

These are goals, not results yet.

## Contact

Questions or suggestions about this document: open an issue in this repository or email [contact@cardio2.info](mailto:contact@cardio2.info). Please never include real personal or health data.

Website: [cardio2.info](https://cardio2.info)

## Licence

This document is licensed under [Creative Commons Attribution 4.0 International (CC BY 4.0)](LICENSE). You may share and adapt it, including commercially, as long as you credit Cardio2 and link to this repository.

The Cardio2 name and logo are not covered by this licence. See [brand-assets](https://github.com/cardio2/brand-assets).
