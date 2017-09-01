# Build summary does not show size diffs for chunks

See create-react-app [issue #3048](https://github.com/facebookincubator/create-react-app/issues/3048).

## Steps to reproduce

1. `git clone git@github.com:esturcke/cra-chunk-bundle-diff-bug.git`
2. `cd cra-chunk-bundle-diff-bug`
3. `yarn build`
4. Comment out the first line of src/content.js and uncomment the second
5. `yarn build`

The build size after the second build does not show a difference in size for the chunk.
