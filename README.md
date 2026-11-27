# arch_smb

A tool for downloading research data to an SMB share. The repository currently contains only this README and a license; implementation details and operational behavior have not yet been documented.

## Project status

No usage command, supported source, file-integrity behavior, credential mechanism, or SMB mount workflow is documented. Do not assume that downloads are implemented or that a mounted share has been validated.

## Design and implementation handoff

Before implementation, document:

- approved data sources and their terms of use;
- download selection and resume behavior;
- checksum and provenance recording;
- partial-download handling and safe destination writes;
- SMB authentication and secret storage;
- mount validation, reconnect behavior, and failure reporting;
- local temporary storage, cleanup, and recovery expectations;
- tests using fixtures or a disposable share, with live-share acceptance recorded separately.

Keep credentials and sensitive research data out of source control. A successful transfer should be verifiable from source identity, destination, size, and checksum.

## Repository sweep policy

Documentation and maintenance passes follow the generalized [repository sweep decision-routing policy](https://github.com/pskeffington/agent_skills/blob/main/docs/REPO_SWEEP_DECISION_ROUTING.md). Add implementation claims only when supported by code and recorded validation.
