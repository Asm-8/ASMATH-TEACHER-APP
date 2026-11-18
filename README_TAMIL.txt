ASMATH TEACHER – QUESTION PAPER MAKER (Android Studio project)
Version 1.2 – PDF text extraction + review workflow

CONFIRMED QUESTION PAPER PATTERNS

10th Science – 75 marks
- 12 x 1 mark = 12
- 7 x 2 marks = 14
- 7 x 4 marks = 28
- 3 x 7 marks = 21 (all three compulsory)

11th / 12th Physics – 70 marks
- 15 x 1 mark = 15
- 9 x 2 marks; answer any 6 = 12 (one compulsory numerical included within the 6)
- 9 x 3 marks; answer any 6 = 18 (one compulsory numerical included within the 6)
- 10 x 5 marks; answer any 5 = 25 (no compulsory numerical in this section)

FEATURES
- Tamil / English question bank entry and filters
- Separate class, mark, chapter and difficulty filters
- Compulsory numerical tagging restricted to 2- and 3-mark questions in XI/XII Physics
- Displays all questions in the generated paper and indicates the compulsory numerical questions
- Answer key toggle, print / Save as PDF, saved papers, JSON backup import/export
- Upload and keep textbook PDFs locally in IndexedDB
- Extract selectable text from uploaded PDFs using PDF.js
- Heuristic question splitting, guessed mark value, editable review list, and selective import into Question Bank
- Original PDF files remain stored on the device

IMPORTANT LIMITATIONS
- PDF extraction requires an Internet connection to load PDF.js from cdnjs the first time / when cache is empty.
- It extracts selectable text PDFs. Scanned/image-only PDFs do not contain a text layer and need OCR; OCR is not included in this build.
- Question splitting and mark detection are heuristic. It may split/merge questions incorrectly or guess a mark incorrectly. Teacher review and correction are required before adding to the bank.
- Chapter/unit is editable during review; it is not reliably inferred from every textbook layout.
- No complete verified bilingual textbook question bank is bundled. The teacher uploads the official PDFs and approves extracted questions.

BUILD APK
1. Open this project folder in Android Studio.
2. Allow Gradle sync (Android Gradle Plugin 8.7.3; compileSdk 35; Java 17 or newer).
3. Select Build > Build Bundle(s) / APK(s) > Build APK(s).
4. Debug APK output: app/build/outputs/apk/debug/app-debug.apk
5. Transfer the APK to the Vivo Android phone and install it. If Android asks, allow installation from that file manager/source.

BUILD STATUS
This project source has been updated and JavaScript syntax checked. This environment does not contain Android SDK, Gradle, or android.jar, so an installable APK has NOT been compiled or device-tested here. This ZIP is source code, not an APK.

AUTOMATIC APK BUILD (GitHub Actions)
1. Create a GitHub repository and upload the contents of this project folder to the repository (main branch).
2. Open the repository > Actions > Build ASMATH Teacher APK > Run workflow.
3. Wait for the workflow to finish successfully.
4. Open the completed workflow run and download the artifact named ASMATH-TEACHER-debug-apk.
5. Extract the ZIP; install app-debug.apk on the Vivo phone. Allow installation from the browser/file manager if Android asks.
Note: This produces a debug APK for personal testing, not a Play Store signed release APK.
