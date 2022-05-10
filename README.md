Modified by me from the original, found at https://github.com/istepaniuk/gilded-rose-js-with-tests, in the following ways:

0. It's in Python 3 now.  So, really the only original content is the README from "Coding Dojo" on

## Installing

Clone the repo and cd to the project directory.
You should have [Python 3](https://www.python.org/downloads/) and  [pip](https://pip.pypa.io/en/stable/installing/) installed.  Making a new [virtualenv](https://virtualenv.pypa.io/en/stable/) is nice also :)

```bash
pip install -r requirements.txt
```

## Running the tests

This kata's test tools include

0. `nosetest` for running your Python tests from the command line
1. `rednose` for colorizing the test output and making it easier to read
2. `nosewatch` to re-run tests automatically as you change your code or tests
3. `coverage` to show you how much of your code is being tested.

```bash
./test.sh        // runs nosetests --cover-branches --with-coverage --rednose --with-watch --cover-erase --cover-html
```

The final test, which relates to a new feature, is skipped.  Remove the `@skip` annotation in `gilded-rose-test.py` to enable it.

Coding Dojo
===========

Note that this Kata has been slightly modified from [the original](http://iamnotmyself.com/2011/02/13/refactor-this-the-gilded-rose-kata/) by Terry Hughes and Bobby Johnson. Namely, in the original Kata the Brie Cheese does not behave exactly like the Backstage passes as this code does. I also think the original kata has a bug on purpose so you have to fix it. This version was used in the Madrid Software Craftsmanship meetup group, and we wanted to focus on refactoring. We had limited time, so the tests are already written and green. [This is a post in my blog about that meeting.](http://blog.istepaniuk.com/refactoring-dojo-the-gilded-rose-kata)

