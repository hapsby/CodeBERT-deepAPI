# CodeBERT for deepAPI

This is a fork of the [CodeBERT](https://github.com/microsoft/CodeBERT) project.  The project is modified to run the
Deep API experiment as described in [Deep API Learning Revisited](https://arxiv.org/abs/2205.01254).  The main
difference is that `"nl"` and `"code"` are swapped in the function `read_examples`, so that the model is trained to
input natural language and output code.  Additionally, you can specify the argument `--randomize_params` which resets
the parameters of the model, thus discarding the pre-training, which is useful for measuring the impact of the 
pre-training.

For more information, see the [Deep API Learning Revisited](https://github.com/hapsby/deepAPIRevisited) repository.