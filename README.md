# LRH-1 Structure-Based GNN Analysis

This repository contains a Graph Attention Network (GAT) analysis of LRH-1 protein structures, developed and presented as part of the Stanford AI Professional Program.

## Objective

To determine whether graph-based representations of protein structure can distinguish conformational states of LRH-1 associated with differences in stability (ΔΔG), and to identify residue-level features contributing to those differences.

## Approach

- Construct protein structure networks (PSNs) from LRH-1 PDB structures
- Represent each structure as a graph of residue-level interactions
- Train a Graph Attention Network (GAT) to classify structures based on ΔΔG
- Extract learned attention/importance signals at the residue level

## Principal Result

The Graph Attention Network (GAT) distinguished high and low ΔΔG LRH-1 conformations and identified specific residues with elevated importance in the higher ΔΔG class, revealing localized network features associated with less stable structural states.

## Interpretation

Unlike traditional classification approaches, the GAT provides residue-level interpretability, highlighting specific regions of the structure that contribute to conformational instability. This enables direct mapping from learned model behavior back to structural biology.

## Methods

- Protein Structure Network (PSN) construction from PDB data
- Graph representation of residue interactions
- Graph Attention Network (GAT) architecture
- Supervised classification based on ΔΔG
- Analysis of attention weights / node importance

## Status

Research prototype developed for structural analysis and demonstration. Code is being refined for clarity and reproducibility.

## Context

This work complements prior PSN-based analyses by introducing a learnable, graph-based model capable of identifying localized structural features associated with thermodynamic differences.
