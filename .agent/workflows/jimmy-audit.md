---
description: Auditing and enforcing the Jimmy System structure
---

# Workflow: Jimmy System Structural Audit

Use this workflow to ensure the repository remains perfectly indexed.

## 1. Top-Level Scan
- Verify all folders start with `N_Name` (0-7).
- Flag any "loose" folders or files at the root (except `.agent`, `.github`, `README.md`).

## 2. Parent-Child Propagation
- For every sub-folder, ensure it follows `N.NN_Name`.
- Verify that the `N` matches the parent's number.
- Example check: Everything in `3_CL_ClearLine` must begin with `3.`.

## 3. Sub-Sub (Letter) Verification
- For three levels deep, use the `N.NN.letter_Name` format.
- Ensure letters are sequential (a, b, c, etc.) within their parent sub-folder.

## 4. Corrective Action
- If a folder is misplaced:
    1. Identify its content theme.
    2. Suggest the correct Jimmy Index move.
    3. Rename using dot-notation.
- If a file has no metadata:
    1. Apply the **Sentinelli Metadata Standard**.

## 5. Report
- Summarize any changes made to the tree.
- Confirm the total file count matches the expected Protocol Lexicon volume.
