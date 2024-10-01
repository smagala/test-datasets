Test data to be used for automated testing with the ph-core pipelines

> ⚠️ **Do not merge your test data to `master`! Each pipeline has a dedicated branch (and a special one for modules)**

## Introduction

ph-core is a collection of high quality Nextflow pipelines with an focus on public health, following the template established by the nf-core community and tools. This repository contains various files for CI and unit testing of ph-core pipelines and infrastructure.

The principle for ph-core test data is as small as possible, as large as necessary. Please see the [guidelines](https://nf-co.re/docs/contributing/test_data_guidelines) for more detailed information.

## Documentation

ph-core/test-datasets comes with documentation in the `docs/` directory:

01. [Add a new  test dataset](https://github.com/smagala/test-datasets/blob/master/docs/ADD_NEW_DATA.md)
02. [Use an existing test dataset](https://github.com/smagala/test-datasets/blob/master/docs/USE_EXISTING_DATA.md)

## Downloading test data

Due the large number of large files in this repository for each pipeline, we highly recommend cloning only the branches you would use.

```bash
git clone <url> --single-branch --branch <pipeline/modules/branch_name>
```

To subsequently clone other branches[^1]

```bash
git remote set-branches --add origin [remote-branch]
git fetch
```

[^1]: From [stackoverflow](https://stackoverflow.com/a/60846265/11502856)
