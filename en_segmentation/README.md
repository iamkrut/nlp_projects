
# en Segmentation

## Installation

Setup virtual environment:

    python3 -m venv venv
    source venv/bin/activate
    pip install -r requirements.txt

## Create output.zip

To create the `output.zip` file do:

    python3 zipout.py

For more options:

    python3 zipout.py -h

## Check your accuracy

To check accuracy on the dev set:

    python3 check.py

For more options:

    python3 check.py -h

In particular use the log file to check output evaluation:

    python3 check.py -l log

## Test Set

The test set can be replaced with whatever file you want to segment at `data/input/test.txt`

## Data files

The data files provided are:

* `data/count_1w.txt` -- counts taken from the Google n-gram corpus with 1TB tokens
* `data/input` -- input files `dev.txt` and `test.txt`
* `data/reference/dev.out` -- the reference output for the `dev.txt` input file

