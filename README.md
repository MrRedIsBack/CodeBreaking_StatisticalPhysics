# Cryptography-Deciphering-Jupyter-Notebook

## Overview
This repository contains a Jupyter notebook (`main.ipynb`) implementing cryptographic techniques to decipher substitution cipher messages. Starting with brute-force permutations, it advances to frequency analysis using Moby Dick text, bigram scoring, and culminates in the Metropolis algorithm for probabilistic optimization.

## Features
- **Permutation Brute-Force**: Tests all 27 rotations (A-Z + space) to identify viable decryptions.
- **Frequency Analysis**: Maps cipher letter frequencies to English norms from Gutenberg texts (Moby Dick); includes interactive swapping for refinement.
- **Bigram Score Function**: Computes log-probability of letter pairs against reference corpus for English-likeness evaluation.
- **Metropolis Algorithm**: MCMC optimization swaps letters probabilistically based on score improvements, annealing via T sequence (10.0 to 0.1); deciphers complex messages.
- ##Examples:** Some example messages have been left in, change the message within the variable `message`.

## Setup and Usage
1. Clone repo: `git clone <repo-url>`
2. Open `main.ipynb` in Jupyter: `jupyter notebook main.ipynb`
3. Run cells sequentially:
   - Downloads Gutenberg texts (Moby Dick, etc.) automatically.
   - Test permutations on sample messages.
   - Refine via frequency mapping and manual swaps.
   - Apply Metropolis for final decryptions.

## Files
| File | Description |
|------|-------------|
| `main.ipynb` | Core notebook with all methods and examples |
| `moby.txt`, etc. | Auto-generated Gutenberg corpora for analysis |
- Simple ciphers solved via permutations.
- Complex ones via Metropolis yield coherent English, e.g., "SHERLOCK HOLMES PRESERVED HIS CALM..." [file:39].

## License
MIT License – feel free to fork and extend for educational use.

