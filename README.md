# AI-Powered-Sales-Presentation-Builder

## Overview

This Python project automates the creation of PowerPoint presentations by reading structured slide data from AI-generated JSON files. It recursively scans a directory for `.json` slide files, parses the content, replaces placeholders with actual values, and builds a fully formatted `.pptx` deck.

The solution is designed to be **robust, scalable, and highly transparent**, with ultra-granular logging to help debug and validate every step of the slide-building process. It gracefully skips malformed or incomplete slides without breaking the entire presentation build.

---

## Features

- **Recursive JSON File Loading:** Automatically discovers all `.json` slide files within a folder hierarchy.
- **Detailed Parsing and Validation:** Logs slide content field-by-field, checks for missing or malformed data.
- **Placeholder Replacement:** Supports dynamic replacement of placeholders (e.g., `<PRODUCT>`, `<FEATURE>`) with user-supplied values.
- **Robust PowerPoint Generation:** Creates slides with titles and body content using `python-pptx`.
- **Graceful Error Handling:** Skips broken or incomplete slides, logs warnings and errors without crashing.
- **Comprehensive Logging & Summary:** Outputs detailed debug information and a summary of processed vs skipped slides.

---

## Getting Started

### Prerequisites

- Python 3.7 or higher
- `python-pptx` library

Install dependencies with:

```bash
pip install python-pptx
