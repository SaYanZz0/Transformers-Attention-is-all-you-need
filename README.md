# Transformer Model for Machine Translation

This repository contains a Transformer model implementation from scratch for building a machine translation system. The implementation follows the architecture described in the paper "[Attention Is All You Need](https://arxiv.org/abs/1706.03762)" by Vaswani et al.

## Table of Contents

- [Introduction](#introduction)
- [Architecture](#architecture)
  - [Multi-Head Self-Attention](#multi-head-self-attention)
  - [Encoder Block](#encoder-block)
  - [Decoder Block](#decoder-block)
- [Usage](#usage)
- [Requirements](#requirements)
- [Installation](#installation)
- [Training](#training)
- [Evaluation](#evaluation)
- [Contributing](#contributing)
- [License](#license)

## Introduction

This project implements a Transformer model for machine translation tasks. Transformers have proven to be highly effective for various natural language processing tasks due to their ability to handle long-range dependencies and parallelize training.

## Architecture

### Multi-Head Self-Attention

The Transformer model relies heavily on the self-attention mechanism, which allows the model to weigh the importance of different words in a sequence relative to each other. The multi-head self-attention mechanism helps capture various aspects of the relationships between words.

Multi-Head Self-Attention
![multi_head_self_attention](https://github.com/user-attachments/assets/214ede89-92e7-4a1c-8466-d167656c86a8)


### Encoder Block

The encoder block in the Transformer model consists of a multi-head self-attention mechanism followed by a feedforward neural network. Both layers have skip connections and layer normalization.

<img width="441" alt="encoder_block" src="https://github.com/user-attachments/assets/3106be7f-e39e-4839-9d39-9d6980e02b4a">


### Decoder Block

The decoder block is similar to the encoder block but includes an additional multi-head cross-attention mechanism that attends to the encoder's output.

<img width="564" alt="decoder_block" src="https://github.com/user-attachments/assets/40b4bedc-13d3-4f5c-be68-2d6561147b69">


## Usage

To use this model for machine translation, follow the instructions below.

## Requirements

- Python 3.x
- TensorFlow or PyTorch
- NumPy
- Matplotlib

## Installation

Clone the repository and install the required dependencies:

```bash
git clone https://github.com/SaYanZz0/Transformers-Attention-is-all-you-need.git
cd Transformers-Attention-is-all-you-need
pip install -r requirements.txt
