# NEET Prep Tracker

A mobile-friendly NEET study tracker with a dedicated test planner and performance record. It is a static browser app; no account or build setup is required.

## Run

Open `index.html` for the study tracker and `mock-tests.html` for tests, result imports, syllabus files, and performance insights.

## Planner and PDF imports

- Upload your test planner PDF. The browser extracts text and suggests likely test names, test type, and dates for a review-before-import list.
- Upload a printed/downloaded result or analysis PDF, choose a planned test, and extract likely marks/date/rank/accuracy. Review and correct extracted fields before saving.
- Attach a separate syllabus PDF to any test and save the extracted text with that test. Edit/correct the text when a particular test's syllabus differs.
- Track scheduled date separately from actual attempt date, including delayed attempts.
- See score averages/trend, subject averages, attempt delays, repeated weak-topic notes, rank, and accuracy where entered or recognized.
- Export a CSV backup, including syllabus and optional extracted report text.

## PDF extraction and accuracy

PDF files are read locally in the browser using PDF.js; the PDF contents are not uploaded to an app backend. The first extraction may load PDF.js from a CDN, so internet is needed once. This works best with selectable-text PDFs. Scanned/image-only documents need OCR, which is not included. Extraction is best-effort: PDF layouts vary, and every detected name, date, mark, rank, or accuracy must be checked against the original before saving. Unrecognized report details remain available in the extracted text for review.

Planner import identifies candidates heuristically and does not invent an official chapter list. Syllabus text describes the scope of a test; it cannot alone prove a strong or weak chapter. Repeated weakness conclusions require chapter-level analysis in the report or weak-topic notes you add.

## Data and privacy

Test records are kept in local browser storage on that device. The app has no cloud sync, no PW account integration, and does not ask for passwords or OTPs. Export CSV regularly; clearing browser data or switching devices can remove or hide records.
