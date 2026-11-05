# NEET Prep Tracker

A mobile-friendly NEET study tracker with a dedicated test planner and results record. It runs in the browser without an account or app backend.

## Run

Open `index.html` for the study tracker and `mock-tests.html` for the test planner, PDF imports, and performance insights.

## Planner and PDF imports

- Import a local planner PDF; the app suggests possible test names, types, and dates for review before adding them.
- Import a downloaded/printed result PDF, select its planned test, review extracted fields, then save marks, actual attempt date, rank, accuracy, and weak topics.
- Attach a separate syllabus PDF to a test. Review the extracted text because different test syllabi may differ.
- Track planned date separately from actual attempt date; inspect score/subject averages, score trend, delays, and repeated weak-topic notes.
- Export a CSV backup.

## PDF support and accuracy

Upload the actual `.pdf` file from your device; a Drive preview URL is not a file. The app checks that the file begins with a PDF signature, allows files up to 40 MB, and uses PDF.js with the worker disabled to avoid common local-file worker issues. It tries two CDN addresses for PDF.js, so internet is needed when first loading the PDF reader.

Extraction works best with selectable-text PDFs. Scanned/image-only files need OCR and cannot be read by the built-in text extractor. Extracted names, dates, scores, rank, accuracy, and syllabus text are only suggestions—verify before saving. PDF layouts vary and automatic results are not guaranteed. If the file still shows an error, note the exact error text, browser, and whether the file opens normally in a PDF reader.

## Data and privacy

Data stays in this browser's local storage; PDFs are read locally and are not uploaded to an app server. There is no PW account connection or cloud sync. Export backups regularly, because clearing browser data or changing devices can remove/hide records.

Gemini/Google AI Pro is separate from this app. An AI subscription does not automatically connect the website to Gemini; automated AI parsing would require a separately configured API and a secure server. Do not put an API key in this public client-side app.
