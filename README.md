# Metadata-Generation-from-Code-using-Sequence-to-Sequence-Translation-Models

Task Description: Metadata generation is essential to comprehend existing codes to help speed up software maintenance processes. In this task we need to implement a sequence to sequence translation architecture to generate summary string from code snippets.

## Dataset

We use a data set from the Code Search Net challenge github repository which has released around 2 million code and docstring pairs in 6 programming languages — go, python, php, ruby, java, javascript. Data is stored in jsonlines format. Each line in the uncompressed file represents one example (usually a function with an associated comment). A prettified example of one row is illustrated below.

repo: the owner/repo
path: the full path to the original file
func_name: the function or method name
original_string: the raw string before tokenization or parsing
language: the programming language
code: the part of the original_string that is code
code_tokens: tokenized version of code
docstring: the top-level comment or docstring, if it exists in the original string
docstring_tokens: tokenized version of docstring
sha: this field is not being used [TODO: add note on where this comes from?]
partition: a flag indicating what partition this datum belongs to of {train, valid, test, etc.} This is not used by the model. Instead we rely on directory structure to denote the partition of the data.
url: the url for the code snippet including the line numbers
