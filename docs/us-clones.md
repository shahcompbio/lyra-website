---
id: us-clones
title: User Stories: Clones
sidebar_label: Clones
---

## Loading data

As a user, I want to be able to include data that specifies what clone each cell belongs to

- Create loader for clonal data
  - Write documentation for clonal data
  - Write tests for loader
- GraphQL layer to pull clone data per cell
  - Update graphQL schema documentation
  - Write tests for resolver

As a user, I want to be able to include that specifies what time point each cell belongs to

- Create loader for time point data (what time point each cell is in)
  - Write documentation for data
  - Write tests for loader
- GraphQL layer to pull clone data per cell
  - Update graphQL schema documentation
  - Write tests for resolver

## Color by category

As a user, I want to be able to see which cells, both in the tree and the heatmap, belong to which clone or time point

- Add ability to select what category to color by
- Update UI to color tree by some category (nodes and clades)
- Update UI to include clone indicator for heatmap

## Fish plots

As a user, I want to see the trajectories of clones over time

- GraphQL layer to pull clone abundances per time point
  - Update graphQL schema documentation
  - Write tests for resolver
- UI for fish plot (or line graph) for all clones

As a user, I want to select what individual clone I want to see trajectory for

- Add interaction to highlight specific clone

As a user, I want to select a subset of cells and see the trajectory for that subset

- GraphQL layer to return abundance over time, given array of cell IDs or indices
  - Update graphQL schema documentation
  - Write tests for resolver
- Add interaction to select clade on tree as subset (maybe on different mode)
