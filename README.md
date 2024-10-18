# BriteSearch

### Overview

**BriteSearch** is a tool that helps you navigate through the intricate web of enzyme-driven biochemical reactions, drawing from the **BRITE hierarchy** on [KEGG](https://www.kegg.jp/). By converting reaction data into a graph, where compounds are linked by enzyme-catalyzed reactions, BriteSearch allows you to discover how molecules transform and interact, and find the most efficient pathway from one compound to another.

### How It Works

1. **Extracting Data**: The program reads from the `brite.json` file and pulls out reaction information, sorting it by enzyme category.
2. **Building a Graph**: Compounds are treated as nodes, and reactions become the connections between them, creating a graph for easy navigation.
3. **Finding Reaction Paths**: Using the NetworkX library, the reaction lists are used as feeders for nodes in a graph and can identify the shortest route between any two compounds.
