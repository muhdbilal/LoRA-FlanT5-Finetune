# LoRA Flan T5 Finetune

This repo hosts an example of adding LoRA (Low Rank Adaptation) layers in Google's Flan T5 model and evaluates its performance for news summarisation.
The data set used is the  [CNN/Dailymail dataset](https://huggingface.co/datasets/abisee/cnn_dailymail)

### What are LoRA (Low Rank Adaptation)

Low Rank Adaptions allow us to finetune the weights of the model in a manner that the dimensions of the weights matrix is reduced. The weights matrix is transformed into a product of two matrices, each having a lower rank than the original weights matrix. This essentially number of parameters to fine-tune, allowing for faster training of large models.