# Arabic Newspaper OCR

## Overview

Arabic Newspaper OCR is a native Windows desktop application for extracting Arabic text from scanned newspapers, images, and PDF documents. Processing happens locally, so source documents are not uploaded to a web service.

## Problem

Scanned Arabic documents often need a review workflow rather than a single OCR command. Users need to move through PDF pages, compare the source with recognized text, retry difficult regions, correct right-to-left text, and export the reviewed result.

## What I Built

- A PySide6 desktop interface for opening images and PDFs
- Single-page and full-document OCR workflows
- Side-by-side source preview and editable right-to-left text
- Region selection for retrying difficult lines or columns
- UTF-8 text export
- Reproducible Windows packaging scripts and an installer definition

## Engineering Highlights

- Local-first processing with no account or browser-based service
- Separation between the Qt workflow, OCR core, and compatibility entry point
- Support for common image formats and multi-page PDFs
- Nuitka and PyInstaller build paths, plus a public Windows installer release
- A smoke test used by the release build workflow

## Architecture / Workflow

1. The desktop interface opens a supported image or PDF.
2. PDF pages are rendered for preview and navigation.
3. Tesseract performs Arabic OCR on a page or selected region.
4. Recognized text is placed in an editable right-to-left document workspace.
5. The reviewed document is exported as UTF-8 text.

## Tech Stack

- Python
- PySide6
- Tesseract OCR through `pytesseract`
- PyMuPDF
- Pillow
- Nuitka / PyInstaller / Inno Setup for Windows packaging

## Running / Release

The repository documents local setup with a Python virtual environment and requires a separate Tesseract installation with Arabic language data. A Windows installer is available from the project's release page.

- [Source repository](https://github.com/pqun7/arabic-newspaper-ocr)
- [Latest release](https://github.com/pqun7/arabic-newspaper-ocr/releases/latest)

## Limitations

- OCR quality depends on scan resolution, contrast, layout, and Tesseract's recognition quality.
- Tesseract and its Arabic language data must be installed separately.
- Extracted text should be reviewed against the source before archival or publication use.
- The repository currently has a smoke test but no visible GitHub Actions workflow; automated CI is a future improvement.

## Repository

[github.com/pqun7/arabic-newspaper-ocr](https://github.com/pqun7/arabic-newspaper-ocr)

