# Structural Anatomy of the Dark Web
## An Analysis of Hidden Service Connectivity

**Author:** Victor A. Capa

_Complex Networks Final Report_

>Reproducibility package for the report 'Structural Anatomy of the Dark Web'. This project characterizes the topological structure of the Dark Web, identifying oligarchic tendencies and ultra-small world properties using NetworkX, Powerlaw, and Gephi.

## How to run
### Prerequisites
- Python 3.10+
- Jupyter Notebook

### Installation
1. Clone this repository or download as a zip file.
2. Install dependencies:
```bash
pip install -r requirements.txt
```

### Execution
1. Open the notebook:
```bash
jupyter notebook DarkWebAnalysis.ipynb
```
2. Run all cells to reproduce the topology analysis, null models comparison and centrality calculations.

### Visualization
The network visualization was generated using **Gephi 0.10.1**
- **Layout:** ForceAtlas2
- **Settings:**
  1. Scalling 200.0
  2. Gravity 0.05 (Stronger Gravity)
  3. Dissuade Hubs enabled.
- **Appearance:** Nodes colored by Community (modularity class - greedy algorithm) and sized by PageRank.

## Data Origin
The dataset analyzed represents a snapshot of the Dark Web hidden services extracted via Tor2web.
- **Source:** [Griffith, V. et al. (2017). Graph Theoretic Properties of the Darkweb](https://arxiv.org/abs/1704.07525)
- **Format**: Directed weighted graph where nodes represent `.onion` domains and edges represent hyperlinks.
- **Processing:** Directions and weights were disregarded for the analysis.

## License
- **Code & Analysis:** The content of the notebooks and scrpits in this repository is realsed into the Public Domain. You are free to copy, modify, publish, use, compile, sell, or distribute this software, either in source code form or as a compiled binary, for any purpose, and by any means.

- **Data:** The dataset included is for educational reproducibility purposes. Rights regarding the dataset content belong to their original collectors/authors.
