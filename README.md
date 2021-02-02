# The Unit Test Quality of Deep Learning Libraries: A Mutation Analysis

## Project summary

We conduct an empirical study to analyze the unit test quality of deep learning libraries. Our study is built on mutation testing, an intensively studied technique to assess the quality of a test suite. Given a program with a test suite, mutation testing mutates the program with predefined mutation operators, and generate many mutants, i.e., buggy versions. Its basic idea is that a better test suite shall detect more mutants, and a detected mutant is considered as killed. With a mutation testing tool, we constructed 1,545 mutants, recorded the results of test cases and compared them with the result of clean versions.

### Our dataset

To ensure the representativeness of our study, we select three popular deep learning libraries such as TensorFlow, Theano and Keras.

### Our tools

In our study, we choose [mutmut](https://github.com/boxed/mutmut) to instrument bugs. We use [coveragepy](https://github.com/nedbat/coveragepy) to record all executed code lines in clean versions. When we generate buggy versions, we instrument only those executed code lines.

### Our summaries

The summaries can be found in [Theano_summary](https://github.com/fordataupload/testcase/tree/main/Theano_summary), [TF_summary](https://github.com/fordataupload/testcase/tree/main/TF_summary) and [Keras_summary](https://github.com/fordataupload/testcase/tree/main/Keras_summary) directories, and we store them in json files.
