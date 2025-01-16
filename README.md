# literati


<!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->

Jupyter notebook combines prose with code in a notebook.
[`literati`](https://radekosmulski.github.io/literati/core.html#literati)
combines prose with code in a markdown file.

## Usage

Run
[`literati`](https://radekosmulski.github.io/literati/core.html#literati).
Create a `<file_name>.md` with your favorite editor.

Write code interwoven with markdown:

    > Time for some fair dinkum mischief...
    Accessing the mainframe to _compile some yarn_.
    ```python
    def hello():
        print("G'day, World!!")
    ```

Whenever you save your file,
[`literati`](https://radekosmulski.github.io/literati/core.html#literati)
transcribes your file to `py/<file_name>.py` stripping all the markdown.
Only the code remains.

Run `python py/<file_name>.py` to run your code.

### Options

- `literati --path /custom/path` - Monitor a different directory
- `literati --output-dir custom_output` - Use a different output
  directory

## The Why

I wanted to try the following pattern of working with LLMs:

- context is your code
- when you want to make changes or additions, provide the context to
  your LLM
- ask for modifications
- update the context to reflect the new information

Context and code, always in sync. For you and your LLM.

## Installation

Install latest from the GitHub
[repository](https://github.com/radekosmulski/literati):

``` sh
$ pip install git+https://github.com/radekosmulski/literati.git
```

or from [pypi](https://pypi.org/project/literati/)

``` sh
$ pip install literati
```

### Install literati in Development mode

``` sh
# make sure literati package is installed in development mode
$ pip install -e .

# make changes under nbs/ directory
# ...

# compile to have changes apply to literati
$ nbdev_prepare
```
