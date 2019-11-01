
# zh Segmentation

### Unigram, bigram, trigram implementation with Jelinek Mercer smoothing and Stupid Backoff smoothing

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

* `data/count_1w.txt` -- unigram word counts 
* `data/count_2w.txt` -- bigram word counts
* `data/count_3w.txt` -- trigram word counts
* `data/count_3w.txt` -- trigram word counts
* `data/train.txt.bz2` -- dataset used to extract unigrams, bigrams and trigrams
* `data/input` -- input files `dev.txt` and `test.txt`
* `data/reference/dev.out` -- reference output for the `dev.txt` input file

