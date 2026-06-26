# VOI_RWE project

**Purpose:** Derive the Policy Indifference Bias (PIB) threshold at which RWE-based CED equals RCT-based CED in population expected net benefit; characterize the threshold via QBA (confounder associations) and sensitivity analysis (timing advantage, trial cost).

**Layout (non-standard):**
- `00_submission/` — SMDM abstract (Jan 2026)
- `01_data/` — empty; all data are simulation-generated (no raw data to protect)
- `02_code/` — entry point: `VOI_QBA.ipynb` (main), `VOU_QBA_Extend_20260225.ipynb` (PSA extension); Python / Google Colab
- `03_output/` — figures (`01_NB_Bias.pdf` … `04_Sensitivity_RR.pdf`), `Tab1_Model_parameters.docx`
- `04_docs/` — manuscript drafts; latest: `VOI+RWE_v4_clean.docx` (2026-03-02)

**Code notes:** runs on Google Colab (Drive mount at `/content/drive/MyDrive/Research/02_VOI_RWE_QBA/`); `lets-plot` for figures; `np.random.seed(2026)`.

**Status:** manuscript at v4 clean; SMDM abstract submitted — likely at pre-submission or journal submission stage.

**HEOR workflow:** `pre-submission-audit` before journal submission. QC = a **simulation / reproducibility audit** appropriate to this decision-science (VOI) analysis — seeds (`np.random.seed(2026)`), deterministic regeneration of every figure/table, PSA parameter documentation, and output traceability — via the `qc-reproducibility-auditor` (Verifier mode). Apply `hem-qc-checklist` **only if** an explicit health-economic decision model (e.g. a Markov / decision-tree CEA workbook with Excel↔engine parity) is actually in scope; the current VOI simulation does not require it.

(Remove this file to opt out of HEOR team context.)
