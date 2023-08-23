# LaTeX Model

This repository contains the work in progress of a language model which is attempting to generate LaTeX code that compiles into realistic looking algebraic geometry. 

The model is essentially a small scale version (7M parameters) of the falcon model, built from scratch, with hyperparamaters tuned to keep the total model size less than the 6GB of memory that my personal GPU has. The Falcon is currently the top model on the LLM leaderboard, and this project is mostly just an attempt to understand why this model is so powerful. This version of the falcon is capable of being trained from scratch on my personal 1660 GPU. It currently has about 6 hours of training time, trained on the stacks project open source LaTeX source code.

I'm currently experimentingg with ways to extend the sequence length without going over 6GB of memory. 
