# Progress - survey_explorer_1

Last visited: 2026-09-15T18:15:00Z

## Status
Actively parsing and extracting data from `SNTP_Assignment01_Master.ipynb`. 
Completed Part A mapping (raw 1490 nodes, 19090 edge blocks, 65 duplicates removed -> 19025 edges; 3 self-loops, 266 isolates removed; 1222 LWCC nodes, 19021 edges, density 0.012748, 420 SCCs with largest 793, in/out degree mean 15.565, median 3 in / 7 out, max 337 in / 256 out).
Proceeding through Part B (Centrality rankings and correlations), Part C/D (Louvain community detection across seeds 0-4, Modularity, Centrality removal attack experiment), Part E (NMI, ARI, Purity, Confusion matrix with ground truth), and Part F (Reproducibility & Reflection).

## Tasks
- [x] Initial dispatch and workspace setup
- [x] Initialize BRIEFING.md
- [x] Inspect files in `e:\sntp_a1\` (notebook structure, outputs folder, data files)
- [x] Extract Part A (Network construction, preprocessing log, graph stats, degree distributions)
- [ ] Extract Part B (Centrality selection, top blogs per metric, Spearman correlation, boundary spanners, HITS)
- [ ] Extract Part C & D (Community detection, Louvain seeds 0-4, modularity, attack/robustness experiment)
- [ ] Extract Part E (Evaluation against ground truth, confusion matrix, NMI, ARI, Purity)
- [ ] Extract Part F (Reproducibility & reflection)
- [ ] Synthesize all quantitative findings into `survey_notebook.md`
- [ ] Write `handoff.md`
- [ ] Send completion message to parent
