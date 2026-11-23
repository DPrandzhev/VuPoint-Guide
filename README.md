# RISCO VuPoint Settings Reference

A searchable reference for VuPoint camera and NVR remote-configuration settings. It combines explanations from RISCO user manuals with observations from device configuration pages.

**Last updated:** 23 November 2026.

## Open the reference

Open [`index.html`](index.html) in a browser, or visit the repository’s GitHub Pages URL after deployment. Search by setting name, purpose, or menu, then filter by device and evidence source. Expand a result to read its explanation and source-page links.

The page works without external JavaScript libraries or an internet connection when downloaded with its accompanying files.

## Publish with GitHub Pages

1. Upload the contents of this folder to your repository. Keep `index.html`, `settings-data.json`, and both PDFs in the same directory.
2. Open **Settings → Pages** in GitHub.
3. Select **Deploy from a branch**, choose the branch and directory containing these files, and save. For a simple setup, place the files at the repository root and select `/ (root)`.
4. Open the published URL shown by GitHub once deployment finishes.

If you prefer GitHub’s `/docs` publishing option, place all these files together in `/docs` and select that folder. The relative PDF links work for both repository sites and custom domains.

## Files

| File | Purpose |
| --- | --- |
| [`index.html`](index.html) | Searchable settings reference, model comparisons, and source links. |
| [`settings-data.json`](settings-data.json) | Structured settings, manual explanations, and comparison findings. |
| [`5IN3148-IP-Camera-User-Manual-WEB.pdf`](5IN3148-IP-Camera-User-Manual-WEB.pdf) | RISCO IP Camera User Manual. |
| [`5IN3149-RISCO-NVR-User-Manual-WEB.pdf`](5IN3149-RISCO-NVR-User-Manual-WEB.pdf) | RISCO NVR User Manual. |
| `README.md` | Repository overview and publishing instructions. |

PDF links include `#page=` references using PDF page numbers. Support for opening a specific page depends on the browser’s PDF viewer.

## Coverage

The reference covers image and illumination controls, video/audio encoding, recording and capture, storage, alarm inputs/outputs, event rules and linkage, thermal measurement, networking, integrations, users, maintenance, and statistics.

| Device | Model | Inspected firmware | Coverage |
| --- | --- | --- | --- |
| 32-channel NVR | RVNVR324K1RA | VC1.3.0-261118 | Main configuration menus and connected-camera controls. |
| Thermal camera | RVCM92A370RA | VC47.55.1.3.6-261116 | Main menus, optical analytics, thermal imaging and temperature measurement. |
| 4MP PT Wi-Fi camera | RVCM61W360RA | VC39.24.1.3.10-261117 | Selected menu differences, display/image, wireless and system pages. |
| 5MP varifocal bullet | RVCM52A350RA | VC31.35.1.3.6-261114 | Image, streams, audio, selected analytics, network, system and maintenance comparison. |
| 8MP fixed bullet | RVCM52A510RA | VC49.57.1.3.11-261105 | Main menus, additional analytics, Fall Detection, stream and model differences. |
| 5MP dome | RVCM32A330RA | VC31.35.1.3.6-261114 | Main menus and comparison with the 5MP bullet. |

The camera and NVR manuals also describe family-level and conditional settings that may not appear on these specific devices. The 4- and 16-channel NVRs were not independently enumerated for this reference.

## Evidence and limitations

- **Manual wording** preserves an explanation from the supplied manual, with a source-page link.
- **Explanation** provides a plain-language interpretation of an observed control and its configuration context. It is not necessarily a manufacturer-confirmed description of that exact firmware.
- Unresolved or inferred behavior is identified in the entry or comparison notes.
- A visible menu does not establish that the selected model implements every function. Some database pages reported that the feature was unavailable in the current state.
- Conditional controls requiring a setting change, disabled editors, and actual event/output behavior were not exhaustively tested. Exact effects of newer controls such as Result Box and Long Distance Mode still need confirmation.

This is a working companion to the manufacturer’s documentation, not an official RISCO publication or a guarantee of identical settings across models and firmware versions. It describes configuration controls; it is not a device configuration backup. Live network values, credentials, and remote-access session URLs are omitted from the reference.

The page also records an inspection exception: opening the thermal measurement-area **Add** control created a disabled row. Its cleanup was not confirmed. The later 5MP/8MP comparison used navigation only and did not change device settings.

## Updating the reference

Keep setting names tied to their menu, model and firmware. Distinguish observed controls from inferred behavior and tested results. Update `index.html` and `settings-data.json` together; the HTML embeds its content and does not automatically reload it from the JSON file.

Preserve the PDF filenames or update all corresponding links. Keep the source PDFs beside `index.html` when moving or deploying the folder.

## Sources and attribution

Source manuals are RISCO Group documents supplied with this reference. Product names and manufacturer documentation belong to their respective owners. This repository does not grant a license to the included manufacturer PDFs.
