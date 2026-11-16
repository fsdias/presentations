# Managing and processing big data in ecology

**Slides:** [fsdias.github.io/presentations/bigdata](https://fsdias.github.io/presentations/bigdata/)

Journal Club talk, March 2023.

**Title:** How to manage and process big datasets in R: an example with eBird data

## Summary

The talk shows how to work in R with a dataset too large to load into memory, using [Apache Arrow](https://arrow.apache.org/docs/r/) with the tidyverse.

- **Data:** the eBird Basic Dataset for Portugal, covering every checklist up to December 2022 (a 7.2 GB `.txt` file with 8.89 million rows).
- **Workflow:** open the file with `arrow::open_dataset()`, convert it to Parquet with `arrow::write_dataset()`, then query it with `dplyr` verbs (`select()`, `filter()`, `group_by()`, `summarise()`) and `collect()` only the results.
- **Question:** how did the COVID-19 lockdowns affect birding in Portugal? The talk counts the eBird checklists and active birders per year from 2008 to 2022.
- **Scientific conclusion:** there were fewer active birders in 2020 and 2021, but those who stayed active birded more.
- **Technical conclusion:** with Arrow, each query and plot took seconds instead of minutes or hours.

The analysis grew into the Substack post [Portugal's birding awakening](https://fsdias.substack.com/p/portugals-birding-awakening-temporal). Its data and code are in [fsdias/blog_data](https://github.com/fsdias/blog_data/tree/main/birding).

The raw eBird data are not included here. You can request them free of charge from [ebird.org/data/download](https://ebird.org/data/download).

## Files

| Path | Content |
|---|---|
| `index.html` | The slides |
| `img/` | Figures, screenshots and memes used in the slides |
| everything else | The reveal.js framework (`dist/`, `css/`, `js/`, `plugin/`) and its examples and tests |
