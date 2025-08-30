# (npm) install

Does some basic stuff

- `$> npm run setup:ci` (if present)
- `$> npm install`

## Motivation

Sometimes we want to add some pre-setup stuff in the package that we want gets picked up by CI.

Things like packages being recommended being installed globally (i.e. `yarn`). Or some other setup w/ python `pip install -r requirements.txt`

## FAQs

### What is the difference w/ (pre|post)install

When developing locally, sometimes you want to run `npm run setup(:ci)` only 1x. Whereas `npm install` is executed more often when maintaining dependencies.
