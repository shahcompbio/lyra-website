---
id: load-analysis
title: Loader: Analysis
sidebar_label: Analysis
---

For each analysis, a YAML file must be present with the appropriate metadata:

- analysis_id = unique identifier for analysis
- jira_id = JIRA ticket identifier associated with analysis
- description = brief outline of analysis
- library_ids = list of libraries associated with this analysis
- sample_ids = list of samples associated with this analysis
- project = name of project associated with analysis
- files = file paths for each data file in analysis

## Sample YAML file

```yaml
analysis_id: <ANALYSIS_ID>
jira_id: <JIRA_ID>
library_ids:
  - <LIBRARY_ID_1>
  - <LIBRARY_ID_2>
  - <LIBRARY_ID_3>
sample_ids:
  - <SAMPLE_ID_1>
  - <SAMPLE_ID_2>
  - <SAMPLE_ID_3>
description: <DESCRIPTION>
project: <PROJECT>
files:
  tree: /exact/path/to/rooted_tree.gml
  tree_order: /exact/path/to/tree_order.tsv
  segs:
    - /exact/path/to/segs_01.csv
    - /exact/path/to/segs_02.csv
    - /exact/path/to/segs_03.csv
  bins:
    - /exact/path/to/bins_01.csv
    - /exact/path/to/bins_02.csv
    - /exact/path/to/bins_03.csv
  metrics:
    - /exact/path/to/metrics_01.csv
    - /exact/path/to/metrics_02.csv
    - /exact/path/to/metrics_03.csv
  h5:
    - base: /exact/path/to/h5_01.h5
      segs: path/in/h5/to/segs
      bins: path/in/h5/to/bins
      metrics: path/in/h5/to/metrics
    - base: /exact/path/to/h5_02.h5
      segs: path/in/h5/to/segs
      bins: path/in/h5/to/bins
      metrics: path/in/h5/to/metrics
```

NOTE: The other loader pages specify options that can be placed in the files section.
