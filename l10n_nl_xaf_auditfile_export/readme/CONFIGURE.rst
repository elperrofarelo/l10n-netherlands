The exporting feature is available to the users who have `Accountant` or `Adviser` rights for accounting.

To configure the default start and end dates of the actual fiscal year, go to `accounting`/`settings` and change the
last date of the year you want to export. Then in the form of the audit file export, by default the end-date will be set
accordingly and the start date will be 12 months before the end date.
Be aware that in case the OCA module `account_fiscal_year` is installed, then the calculus of the fiscal year dates is
overridden, taking by default the date range defined for the actual fiscal year (check `Settings`/`Date Ranges`).

This module works on huge amount of data, so there is a possibility to encounter out of memory exceptions. In this case. set the config parameter `l10n_nl_xaf_auditfile_export.max_records` to a value much lower than 10000.
