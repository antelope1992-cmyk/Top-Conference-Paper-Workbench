# Top-Conference Paper Workbench

Free GitHub foundation edition of a Codex skill for building evidence-traced research paper packages.

This skill helps turn a research topic, technical system, proposal, paper list, or project notes into:

- a protocol
- a reproducible search log
- an evidence matrix
- a manuscript outline
- a draft
- a QA report
- an optional Word-ready deliverable

It is designed for top-conference-style workflows such as system papers, method papers, benchmark papers, workshop submissions, literature reviews, and internal research deliverables.

## What This Is

This is a workflow skill, not a magic acceptance machine.

It helps with:

- structuring research claims
- separating public evidence, assumptions, and measured results
- reducing unsupported claims
- organizing citations and evidence
- preparing paper packages for expert review
- running a basic smoke test before delivery

It does not:

- guarantee conference or journal acceptance
- fabricate experiments, citations, or measured results
- replace domain experts, authors, or reviewers
- turn public demos into your own project data

## Installation

Copy the skill folder into your Codex skills directory:

```text
top-conference-paper-workbench/
```

Typical Windows path:

```text
%USERPROFILE%\.codex\skills\top-conference-paper-workbench
```

The `SKILL.md` file must be directly inside the skill folder.

## Usage

Example prompt:

```text
Use $top-conference-paper-workbench to turn this topic into a top-conference-style paper package with protocol, evidence matrix, manuscript outline, draft, QA report, and Word-ready deliverable. Separate public evidence, project assumptions, and measured results.
```

Provide as much context as possible:

- target venue
- paper type
- source links
- existing notes
- datasets
- experiment logs
- figures or tables
- claims that need checking

## Package Structure

The skill expects paper work to be organized like this:

```text
paper-package/
  protocol/protocol.md
  search/search_log.md
  extraction/evidence_matrix.csv
  draft/review_draft.md
  qa/qa_report.md
  exports/
```

## Smoke Test

Run:

```bash
python top-conference-paper-workbench/scripts/smoke_test_review_package.py <paper_package_dir> --strict
```

Passing the smoke test means the package has a minimum auditable structure. It does not mean the paper is accepted, novel enough, or experimentally complete.

## Free vs Pro Roadmap

This free edition includes:

- core skill workflow
- protocol template
- evidence matrix template
- extraction form template
- draft skeleton
- QA gate
- smoke test script
- optional PubMed helper for biomedical topics
- Word manual

Possible future Pro content:

- venue-specific paper packs
- reviewer QA gates
- rebuttal templates
- real case libraries
- domain-specific workflows
- enterprise/lab customization

## License

MIT License. See [LICENSE](LICENSE).

