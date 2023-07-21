# Labyrinth Repository Search

[![SearchRepos](https://github.com/CERTCC/labyrinth/actions/workflows/repo_search.yml/badge.svg)](https://github.com/CERTCC/labyrinth/actions/workflows/repo_search.yml)
[![Update Summaries Daily](https://github.com/CERTCC/labyrinth/actions/workflows/update_summaries_daily.yml/badge.svg)](https://github.com/CERTCC/labyrinth/actions/workflows/update_summaries_daily.yml)

"Things are not always what they seem in this place, so you can't take anything for granted." - The Worm

This is an experimental project by the CERT/CC to find code that looks like it might be exploit code.
This project is creating an index with pointers to repositories of potential interest to vulnerabilty analysts and security researchers.

- Raw search results are placed into [`/results`](./results/), organized by year, month, and day.
- Then we periodically do a deep dive into the repositories found in our search results to see if any files contain strings that look like vulnerability identifiers.
Those results go int [`/data`](./data/), and are organized by repository IDs and vulnerabilty IDs.

