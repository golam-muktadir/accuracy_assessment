# GIS Accuracy Assessment Learning Laboratory

A static, browser-based learning platform for GIS and remote-sensing accuracy assessment. It includes ten learning modules, interactive accuracy/precision and sampling activities, a sample-size calculator, an editable confusion matrix, accuracy metrics, a practice map, a timed final quiz, local progress tracking, a same-device leaderboard, and printable certificates.

## GitHub-only deployment (GitHub Pages)

This project does not require Supabase, Firebase, a server, a database account, API keys, or a build step.

1. Download and extract this project ZIP.
2. Open the extracted `gis_accuracy_assessment-main` folder.
3. Upload **the contents of this folder** to the root of your GitHub repository. `index.html` must be at the repository's published root (not one folder deeper).
4. In GitHub, open **Settings → Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select your branch (usually `main`) and folder `/ (root)`, then click **Save**.
7. Wait for the Pages deployment and open the URL GitHub provides.

## How student names, progress and leaderboard work

- Students enter a name; no password or account is required.
- Progress, completed modules, points, quiz score and reflection are saved in the browser's `localStorage`.
- The leaderboard can show learners who have used the site in the **same browser on the same device**. Students can switch learner names on that device to demonstrate the class leaderboard.
- Data is not uploaded to GitHub and is not shared automatically between different students' phones/computers or browsers. GitHub Pages is static hosting and does not provide a writable shared database.
- Clearing browser data, using private/incognito mode, or changing browser/device can remove or separate saved progress.

This is suitable for low-stakes learning and classroom practice, not official grading or secure examinations. Name-only access is not identity verification.

## Certificates

Complete all ten modules and score at least 60/80 on the final quiz. Select **Download certificate / Print PDF**, then choose **Save as PDF** in the browser print dialog. The certificate is generated in the browser; no external certificate service is used.

## Internet and external assets

The learning content and local progress work as a static website. The interactive basemap uses Leaflet and public map tiles loaded from the internet; Google Fonts are also loaded externally. Those are visual assets, not accounts or databases. The practice map's sample points are illustrative and are not real field-verified reference observations.

## Notes for teaching

- The sampling grid and practice map points are synthetic learning examples.
- The sample-size calculator uses a simplified proportion formula and does not automatically account for stratification, unequal allocation, design effects, finite population correction, or class-specific precision.
- Interpret Kappa alongside the error matrix, overall accuracy, class-specific producer's/user's accuracy, sampling design and reference-data quality.
