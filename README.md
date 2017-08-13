# alembic-checker

## OS
Mac OS X

## Dependencies
`brew install graphviz`

## Run

`Usage: alembic-rev-graph [PATH/OF/ALEMBIC/VERSIONS/FOLDER]`

The default path is `$PWD`.

## Result
Normally, a healthy list of alembic revisions is two synchronized single linked lists, by revision and file name.

If the graph shows something abnormal as the image below, you absolutely merged the revisions wrongly with other developers.

![alembic-revision-in-wrong-sort](https://github.com/wushaobo/alembic-checker/raw/master/alembic-revision-in-wrong-sort.png)
