# manageiq-lxca-docs
Repository for generating documentation for the Lenovo XClarity Administrator provider for ManageIQ

## Compile into PDF
. Edit [main.adoc](./nuage_provider_configuration/main.adoc) and remove comments from the appropriate variable set (either ManageIQ or CloudForms).

. Install [`asciidoctor-pdf`](https://asciidoctor.org/docs/asciidoctor-pdf) gem.

. Compile the Configuration Guide:
+
```bash
bundle exec asciidoctor-pdf physical_infra_provider_configuration/main.adoc -o ./PREVIEW.pdf
```
+
. Compile the API Guide:
+
```bash
bundle exec asciidoctor-pdf physical_infra_provider_rest_api/main.adoc -o ./PREVIEW.pdf
```
+

Command above will create file `./PREVIEW.pdf` that can be used as documentation preview.