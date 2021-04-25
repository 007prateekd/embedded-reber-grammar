# Embedded-Reber-Grammar
## What
The Reber grammar is an example of a simple finite state grammar and it has served as a benchmark for equally simple learning systems. It can be used for generating artifical data for the evaluation of recurrent neural networks (RNNs). The Embedded Reber Grammar is an extension of the "standard" Reber Grammar. In this case, the second character is always the same as the second last char character. This is an example of a long range dependency. 

## Why
These two grammars are ways of testing the ability of a RNN to learn long-range dependencies. Traditional RNNs are fine with Reber Grammars, but fail on Embedded Reber Grammars. If an RNN is purported to be able to learn long-range dependencies (such as an LSTM or GRU), the embedded Reber grammar is a good corpus generator and a good result checker.

## How
In this notebook, I chose a particular Embedded Reber Grammar, then trained an RNN (GRU to be precise) to identify whether a string respects that grammar or not. After just 20 epochs of training, we see that our model learned to identify the long-term patterns in the Embedded Reber Grammar.
