Modified by me from the original, found at https://github.com/matthewmorgan/gilded-rose-python-with-tests, in the following ways:

0. remove the unnecessary dependencies
1. add spanish version of kata description
2. update the README.md
3. better tests interface

## Installing

Clone the repo and cd to the project directory.


## Running the tests

```bash
python -m unittest gilded_rose_test.py
```

The final test, which relates to a new feature, is skipped.  Remove the `@skip` annotation in `gilded_rose_test.py` to enable it.
