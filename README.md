# Transformer Circuit Discovery

Empirical investigation of transformer circuits using activation patching and
mechanistic interpretability techniques.

## Research Question

Can internal transformer components responsible for specific token-prediction
behaviors be identified and causally evaluated using activation patching?

## Motivation

Large language models exhibit complex behaviors that emerge from interactions
between attention heads, MLPs, residual streams, and other internal components.

This project investigates whether specific components can be linked to
particular model behaviors and whether those relationships can be tested
causally rather than inferred only from correlations.

## Current Focus

- Induction heads
- Indirect object identification
- Attention pattern analysis
- Activation patching
- Causal effect measurement

## Models

- GPT-2 Small

## Tools

- Python
- PyTorch
- TransformerLens
- Einops
- NumPy
- Pandas
- Matplotlib

## Methodology

The project follows an experimental workflow:

1. Construct controlled prompts.
2. Run clean and corrupted inputs through the model.
3. Identify candidate internal components.
4. Inspect attention and activation patterns.
5. Perform activation-patching interventions.
6. Measure changes in model behavior.
7. Compare intervention effects across components.

## Status

In progress.

Results will be added as experiments are completed and independently
validated.

## Repository Structure

```text
src/            Core analysis utilities
experiments/    Reproducible experiment scripts
notebooks/      Exploratory analysis
results/        Experimental outputs
figures/        Generated visualizations
tests/          Unit tests