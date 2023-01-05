# Spectrum1
spectrum terraform repo
version: "~>0.1"
formatter: markdown table
sections:
  show:
    - requirements
    - inputs
    - outputs

output:
  file: README.md
  mode: inject
  template: |-
    <!-- BEGIN_TF_DOCS -->
    {{ .Content }}
    <!-- END_TF_DOCS -->

sort:
  enabled: true
  by: required

settings:
  indent: 4
  escape: false
  default: false
  required: false
  type: true
