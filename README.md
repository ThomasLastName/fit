# fit

## What:

Training pipeline for pytorch models, inspired by the `fit()` method of keras models.


## Why:

The function `fit` defined in the file `fit.py` enables a more convient and faster workflow of model prototyping when . Its purpose is analogous to [pytorch lightning](https://lightning.ai/docs/pytorch/stable/starter/introduction.html) but its implementaiton is much simpler, resulting on one hand in an improved workflow for basic use cases, but on the other hand a lack of support for some some advanced use cases. As a rule of thumb, `fit` tends to support custom model architectures, but may fail to support custom training logic.


## How:

The idea is: `fit( model, dataloader, loss_fn, optimizer, epochs=n )` trains that `model` for `n` epochs on that data (supplied in the form of the `dataloader`) according to that `optimizer` and `loss_fn`.

Until I set up documentation, **please see this [DEMO in Colab](https://colab.research.google.com/drive/1KQFv0z3JUV1C3ctORTvsvpPA-GJ_Ubur?usp=sharing)** and feel free to reach out to me at winckelman@tamu.edu with any questions.
