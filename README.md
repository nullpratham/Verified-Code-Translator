# Verified Code Translator

**Team:** forked.exe · **Course:** SCSE4041 · **Problem:** C7 · **Direction:** C++ → Python

## Academic details
- Team ID: PE-B49-15
- Batch: 63
- Faculty: Ankit Vijay Bansal
- Team leader: Pratham Raj (S24CSEU2199)

## Team
| Member | Enrollment |
|---|---|
| Pratham Raj | S24CSEU2199 |
| Tanvi Goyal | S24CSEU2250 |
| Aarna Verma | S24CSEU2297 |
| Yashvi Kaushik | S24CSEU2300 |
| Ojas Vats | S24CSEU2241 |
| Tanishka Singh | S24CSEU0593 |

## Workflow
1. Paste C++ source and generate the translation prompt.
2. Run the prompt manually in ChatGPT and obtain a Python candidate.
3. Paste the candidate into Stage 2.
4. Generate a separate verification prompt and run it in ChatGPT.
5. Review findings and execute code separately when evaluating behaviour.

## Run locally
Open `index.html` in a modern browser. No dependencies or installation are required.

## Scope and evaluation
This is a static HTML/CSS/JavaScript prompt-generation prototype. It does not call an AI API, execute user code inside the browser, persist checklist state, or formally prove semantic equivalence. ChatGPT interaction is manual; static verification is advisory.

The sample `findMaximum` C++ implementation and its Python translation were independently compiled/run and compared on ten non-empty input cases. All ten returned matching outputs. The test scope and boundary limitation are documented in [test results](test-data/TEST_RESULTS.md). These function-level checks do not constitute automated testing of the browser UI or proof of equivalence for arbitrary programs.

A separate set of workflow examples is labelled **Simulated** and must not be interpreted as app execution or measured results: [simulated workflow scenarios](test-data/SIMULATED_WORKFLOW_SCENARIOS.md).

## Contribution note
An equal split (approximately 16.67% per member) is proposed in the report, pending confirmation from all members. Ensure the final declaration reflects actual contributions and is agreed by the team.

## Reports
The committed PDFs are earlier versions. Replace them with the updated PDFs from the final M2 package before treating the repository as submission-ready. See [report replacement notes](docs/REPORTS_PENDING_UPLOAD.md).
