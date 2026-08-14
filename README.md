# Rice Leaf Disease Detection

CNN image classifier identifying rice leaf diseases from a small labeled
image dataset.

## Overview

119 RGB images across 3 disease classes (Leaf Smut, Brown Spot, Bacterial
Leaf Blight — ~40 images each). With a dataset this small, overfitting is
the central challenge, not raw accuracy.

Built a baseline CNN first, which overfit as expected (large train/val gap).
An improved version — data augmentation, batch normalization, dropout, and
early stopping — reduced that gap and gave more stable validation
performance, even though headline accuracy gains were modest.

## Tech Stack

TensorFlow / Keras · OpenCV

## How to Run

Extract the dataset zip, run all cells top to bottom. The baseline model
runs first; the augmented/regularized model and comparison come after.

## Note

This is a small-dataset proof of concept — the README is upfront about the
overfitting trade-offs rather than reporting a single headline accuracy
number, because on 119 images that number would be misleading on its own.
