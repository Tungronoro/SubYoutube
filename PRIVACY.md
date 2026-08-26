# SubYoutube Privacy Policy

**Last updated:** August 26, 2026  
**Extension name:** SubYoutube  
**Publisher:** Nguyễn Thanh Tùng (SubYoutube)

## 1. Scope

This Privacy Policy explains how the **SubYoutube** extension handles data when you use it on Microsoft Edge or a compatible Chromium-based browser.

## 2. Data the extension reads

After you intentionally open the extension on a YouTube video page and request a scan, SubYoutube may read the following information from the current page:

| Data type | Purpose |
|---|---|
| Transcript or subtitles | Display the transcript, create prompts, and export an SRT file. |
| Comments and expanded replies | Display, count, and create community-analysis prompts. |
| Current video URL and title | Identify the video and save results by video. |
| Interface language selection | Remember the VI or EN choice for the next session. |

SubYoutube does not request or collect passwords, verification codes, payment information, contacts, location data, health information, or YouTube login credentials.

## 3. How data is used

The data is used to display transcripts and comments in the extension popup, copy each section separately, create Vietnamese or English prompts, export transcript cues as an `.SRT` file, and restore saved results when the popup is reopened.

SubYoutube does not automatically send transcripts, comments, or prompts to a SubYoutube server, an external AI service, or another third party. You decide whether and when to copy data to another application or service.

## 4. Storage and retention

Scan results are stored temporarily in the browser or extension's local storage and associated with the video ID. Results older than 24 hours are automatically removed, and the extension retains no more than 10 recent video states. Data may remain in local browser storage until the automatic cleanup occurs or you remove the extension's stored data through the browser settings.

## 5. Data sharing

SubYoutube does not sell, rent, or share transcript data, comments, video URLs, or prompts with third parties. The extension does not operate a private server that receives user data.

If you intentionally copy content to an AI tool, any subsequent processing is governed by that tool's privacy policy. SubYoutube does not control or take responsibility for how an external service processes data after you choose to send it there.

## 6. Permissions and access

The extension uses access to the current tab, scripting, tabs, storage, and the necessary YouTube domains to provide the functions described in this policy. SubYoutube reads page content only after you open the extension and request a transcript or comments scan. The extension does not use remotely hosted JavaScript code.

The permissions are used as follows:

| Permission | Purpose |
|---|---|
| `activeTab` | Access the current tab after you intentionally open the popup and request a scan. |
| `scripting` | Run the extraction logic for transcripts and comments on the current YouTube page. |
| `tabs` | Read the current video URL and title so results can be identified and saved by video. |
| `storage` | Temporarily save transcripts, comments, prompts, and timestamps in the browser. |
| YouTube host permissions | Limit extension activity to the YouTube domains required for the feature. |

## 7. Children

SubYoutube is not designed to collect personal information from children and does not require personal information to use its primary features.

## 8. Changes to this policy

If the way SubYoutube handles data changes, this policy will be updated before or when the relevant new version is released. The latest update date is always shown at the top of this document.

## 9. Contact

To report a bug or ask a privacy question, please open a [GitHub Issue](https://github.com/Tungronoro/SubYoutube/issues) in the SubYoutube repository. Do not post passwords, one-time codes, phone numbers, addresses, or private transcript/comment content in an issue.
