# Runbook: Funding

This board uses the shared STEMEd+ pipeline. For how every board works and the common fixes, see the [stemedplus-theme runbook](https://github.com/stemedplus/stemedplus-theme/blob/main/RUNBOOK.md).

| | |
|---|---|
| **Site** | stemedplus.github.io/stemed-funding |
| **Repository** | stemedplus/stemed-funding |
| **Updates** | Daily at 11:41 UTC, on push, and by hand (`update.yml`) |
| **Sources** | Federal calls from the Grants.gov API, chosen by keywords and agencies in `config/federal.json`; foundation, society, and state programs as files in `opportunities/` |
| **Check / build** | `python -m stemed_funding --validate`, then the build |
| **Add or fix** | **Suggest an opportunity** and **Update an opportunity** issue forms |

**A federal call is missing or shouldn't be there:** adjust the keywords, agencies, or `drop` lists in `config/federal.json`.

**Add a foundation or society program:** add a file in `opportunities/` that passes the schema in `schema/`.

_Written November 2026. Review with the yearly December review._
