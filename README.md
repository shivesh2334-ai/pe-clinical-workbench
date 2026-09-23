# PE Clinical Workbench

A static, responsive adult pulmonary embolism clinical decision support application. Open `index.html` locally or deploy the repository to Vercel with **Framework Preset: Other**, **Root Directory: /**, and no build command. The app has no runtime API keys, patient persistence, analytics or backend.

## Workflow

Record presentation and vital signs; enter imaging, D-dimer, RV and biomarker findings; flag anticoagulation modifiers, APS, connective tissue disease, family history and recurrence. The UI calculates the three-tier Wells score and sPESI, describes incomplete evidence, suggests next investigations and differential diagnoses, and supplies treatment duration and follow-up prompts. Shock and bleeding prompts override routine pathways. The search panel performs local lexical retrieval against short, attributed guideline summaries and links to publisher guidance. It is retrieval, **not** a generative LLM or full-text UpToDate index; no copyright-protected article is bundled.

## Clinical safeguards and limitations

Adult-only and clinician-facing. No prescription is auto-issued. D-dimer thresholds, dose selection, renal adjustment, thrombolysis eligibility, APS confirmation and discharge eligibility need clinician review and local protocol. Wells is pretest probability; sPESI is prognostic only for diagnosed PE. The simplified risk tier is not the full 2026 AHA/ACC category implementation; mixed or missing RV/biomarker findings must be interpreted clinically. Vitals defaults are examples, not a patient. The application has not been clinically validated and should undergo clinical governance review before patient use.

## Evidence

- [2026 AHA/ACC multisociety acute PE guidance](https://professional.heart.org/en/science-news/2026-guideline-for-the-evaluation-and-management-of-acute-pulmonary-embolism-in-adults/top-things-to-know)
- [2019 ESC/ERS acute PE guidance](https://www.escardio.org/guidelines/clinical-practice-guidelines/all-esc-practice-guidelines/acute-pulmonary-embolism/)
- [ASH 2023 thrombophilia testing](https://www.hematology.org/education/clinicians/guidelines-and-quality-care/clinical-practice-guidelines/venous-thromboembolism-guidelines/thrombophilia)
- [ASH 2020 VTE treatment](https://ashpublications.org/bloodadvances/article/4/19/4693/463998/American-Society-of-Hematology-2020-guidelines-for)
- [EULAR antiphospholipid syndrome recommendations](https://ard.bmj.com/content/78/10/1296)

The supplied UpToDate excerpt informed scope but is not redistributed. Evidence summaries were curated 23 September 2026; update the entries in `app.js` after guideline review.
