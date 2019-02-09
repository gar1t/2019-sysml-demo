# Notes 2

- Include each step of the demo in the paper.

- Also include in the demo the ability to sync runs over SSH or S3.

## What is Guild AI?

Guild AI is an open souce toolkit for running, tracking, and comparing
machine learning experiments.

Guild runs experiment trials as separate operating system processes
and tracks results in separate run directories. Each run directory
contains the artifcats generated during the trial along with metadata
including model information, start and stop times, logs, and run
status. Run artifacts may include model checkpoints, prepared data
set, generated content such as images and audio, and logs.

Guild provides facilities to analyze and compare experiments. User can
report training and validation loss, accuracy and any other metric
that is recorded across all experiments. User can perform detailed
comparison across experiment inputs including changes in model
architecture, hyperparameters, data sets, and source code.

Guild's primary user interface is a CLI (command line interface),
however, Guild also provides a graphical, web based dashboard to
explore and analyze runs.

Guild is a command line application that runs externally to user
code. Guild also provides a complete Python API that optionally be
used to control Guild, but the API is not required for any of Guild's
core features.

Guild supports any command that generates experiment results - models
can be implemented in any language, framework, or software
library. Commonly supported libraries include TensorFlow, Keras,
PyTorch, MXNet, scikit-learn, and SGBoost. However, Guild supports
other Python libraries, pure Python, and languages such as R, Go, and
Java.



## Who uses Guild AI?

## What is similar?

## How is Guild AI different?
