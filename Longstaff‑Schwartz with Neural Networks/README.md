
This project implements two variants of the Longstaff‑Schwartz algorithm to price an American put option:

1. Linear LS : continuation value approximated by polynomial regression (basis 1, S, S², S³).
2. FNN‑LS : continuation value approximated by a feedforward neural network.

We compare both methods and perform an hyperparameter study on the FNN variant: number of scenarios, number of epochs, batch size, normalisation (MinMax / Normal / none), learning rate, network size, activation function (ReLU, Tanh, Sigmoid, LeakyReLU), optimiser (Adam, SGD, SGD+momentum, RMSprop).

Both methods converge to essentially the same price. The FNN is considerably slower. Hyperparameters have little influence on this simple one‑dimensional problem; the advantage of neural networks would likely emerge in higher dimensions where polynomial bases become impractical. Normalisation, particularly standard scaling, improves stability and accuracy.

<img width="945" height="337" alt="image" src="https://github.com/user-attachments/assets/abdb0e97-4cd9-43f6-a40f-5b9b7e182de1" />


**Reference:** Longstaff, F.A. & Schwartz, E.S. (2001). *Valuing American options by simulation: a simple least‑squares approach*. Review of Financial Studies.

The report and source code can be provided upon request.
