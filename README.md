# LRH-1 Structure-Based GNN Analysis

This repository contains a Graph Attention Network (GAT) analysis of LRH-1 protein structures, developed and presented as part of the Stanford AI Professional Program.

## Objective

To determine whether graph-based representations of protein structure can distinguish conformational states of LRH-1 associated with differences in stability (ΔΔG), and to identify residue-level features contributing to those differences.

## Approach

- Construct protein structure networks (PSNs) from LRH-1 PDB structures
- Represent each structure as a graph of residue-level interactions
- Train a Graph Attention Network (GAT) to classify structures based on ΔΔG
- Extract learned attention weights and attribution-based importance signals at the residue level

## Principal Result

The Graph Attention Network (GAT) distinguished high and low ΔΔG LRH-1 conformations and identified residues with elevated importance in the higher ΔΔG class, revealing localized network features associated with less stable structural states.

## Model Interpretation and Validation

To interpret model behavior, Integrated Gradients (IG) were applied to quantify residue-level importance across LRH-1 structures.

Group-averaged residue importance profiles revealed consistent differences between high and low ΔΔG conformations. Importantly, these learned importance patterns recapitulate previously observed structural features, including differences in interaction density near the ligand-binding region.

Statistical analysis across multiple graph construction parameters confirmed the robustness of these signals, indicating that the GAT captures stable, biologically meaningful features rather than artifacts of a single configuration.

## Key Insight

The model demonstrates that conformational instability in LRH-1 is associated with localized changes in residue interaction networks, particularly near the ligand-binding region, rather than uniform global structural differences.

## Methods

- Protein Structure Network (PSN) construction from PDB data
- Graph representation of residue interactions
- Graph Attention Network (GAT) architecture
- Supervised classification based on ΔΔG
- Attribution via Integrated Gradients (IG) for residue-level importance

## Status

Research prototype developed for structural analysis and demonstration. Code is being refined for clarity and reproducibility.

## Context

This work complements prior PSN-based analyses by introducing a learnable, graph-based model capable of identifying localized structural features associated with thermodynamic differences.

## Reference

Presented at the Stanford AI Professional Program Show-and-Tell Series
