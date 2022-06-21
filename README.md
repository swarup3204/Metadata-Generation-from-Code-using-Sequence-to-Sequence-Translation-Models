## Metadata-Generation-from-Code-using-Sequence-to-Sequence-Translation-Models

Task Description: Metadata generation is essential to comprehend existing codes to help speed up software maintenance processes. In this task we need to implement a sequence to sequence translation architecture to generate summary string from code snippets.

# Dataset

We use a data set from the Code Search Net challenge github repository which has released around 2 million code and docstring pairs in 6 programming languages — go, python, php, ruby, java, javascript. Data is stored in jsonlines format. Each line in the uncompressed file represents one example (usually a function with an associated comment). A prettified example of one row is illustrated below.
