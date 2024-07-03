# NC edited HiFi Full-length 16S analysis pipeline

(forked on 2024-06-28 from https://github.com/PacificBiosciences/HiFi-16S-workflow in order to slightly alter code and add custom scripts)

This file was added to describe the changes operated on the forked version

- Table of Contents
  * [Nextflox Edits](#nextflow-edits)
  * [Input Files](#input-files)
  * [bash wrapper](#bash-wrapper)
  * [Archive structure](#archive-structure)
  * [NextCloud transfer](#nextcloud-transfer)

## Nextflox Edits

Some extra config definitions were added to the original **nextflow.config** file manually then the resulting edited file was used to create apatch as shown next.

```
mkdir -p updates
diff -u nextflow.config nextflow.config.edit > updates/nextflow.config.patch
cp nextflow.config updated/nextflow.config.ori
patch nextflow.config < updates/nextflow.config.patch
```

Additionally, a secondary config file named **config.extra** was created in teh nextflow folder (and copied to **updates**)

## Input Files

## bash wrapper

## Archive structure

## NextCloud transfer
