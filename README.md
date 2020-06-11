# Sequential Data Analysis in Python

To model sequences, we need to:
1. Handle **variable-length** sequences
2. Track **long-term** dependencies
3. Maintain information about order
4. **Share parameters** acroos the sequence
****
## Why not using a simple ANN for sequence data?

If we use an ANN model for a long sequence, we can face the problem of vanishing/exploding gradients. To prevent this problem we can use a more complex recurrent unit with gates to control what information is passed through.

## 1. Recurrent Neural Network (RNN)

## 2. Long Short Term Memory (LSTM)
LSTM modules contain **computational blocks** that **control information flow**. LSTM cells are able to track inforamtion throughout many timesteps.

Information is **added** or **removed** through structures called gates.

Gates optionally let information through, for example via a sigmoid neural net layer and pointwise multiplication.

How LSTMs work? 
1) Forget, LSTMs **froget irrelevant** parts of the previous state.
2) Store, LSTMs **store relevant** new information into the cell state.
3) Update, LSTMs s**electively update** cell state values.
4) Output, The **output gate** controls what information is sent to the next time step.

## 3. RNN Applications

- Music Generation
- Sentiment Classification
- Machine Translation
