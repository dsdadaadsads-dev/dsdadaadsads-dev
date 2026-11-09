# Product export comparison - synthetic capability sample

[View the one-page comparison](product-export-comparison.pdf).

This original, AI-assisted demonstration compares two normalized product
exports. It shows changed prices and stock, keys present in only one export,
duplicate-key ambiguity and invalid values. No customer data was used and no
store was connected, corrected or updated. It is not paid client work or proof
of customer results.

The inputs are [before.csv](before.csv) and [after.csv](after.csv). The machine-
readable findings are in [report.json](report.json); [HASHES.json](HASHES.json)
binds the exact sample files. The sample contains 7 distinct SKU keys, 6 review
items and 1 unchanged key. A duplicate key or invalid value suppresses numerical
comparison; a currency mismatch produces no FX conversion or price delta.

The supported comparison schema is exactly `sku,price,currency,stock`, UTF-8
comma CSV, a shared literal SKU namespace, two files up to 100 KiB each and
1,000 combined records. SKUs are case-sensitive, 1-64 characters with no surrounding
whitespace/control characters. Prices support nonnegative plain decimals with
up to 9 integer and 4 fractional digits; stock supports nonnegative integers with
up to 9 digits. Currency is a three-uppercase-letter label, not a validated FX
code. Other platform formats require separately scoped mapping.

**Separate scope:** the existing $49 Upwork structural/duplicate-ID CSV audit does
not include this comparison. This sample is not an import certification,
accounting service, commercial quote, availability promise or upload tool. Any
custom paid comparison would need separate scope, privacy, timeline and price
qualification. The existing offer remains unchanged.

[Existing structural CSV audit and its actual terms on Upwork](https://www.upwork.com/services/product/development-it-a-professional-csv-export-report-with-duplicate-id-and-format-checks-2119040538064915396).
Use the Upwork workflow for applicable inquiries. Never post private exports,
customer records, credentials or financial information in GitHub issues.
