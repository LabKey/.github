# .github

## CodeQL model pack

`codeql/java-models` is the `labkey/java-models` model pack, which the organization's code scanning default setup applies to every Java analysis (Settings → Advanced Security → Global settings → Expand CodeQL analysis). Merging a change under that directory to `develop` publishes it to `ghcr.io/labkey/java-models`; bump `version` in `qlpack.yml` first, since an existing version can't be republished.

Barrier models name methods by package, class, and signature, so renaming a modeled method silently turns its model off.
