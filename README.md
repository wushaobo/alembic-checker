# alembic-checker

## OS
Mac OS X

## Run
- with homebrew
- with source code

### With homebrew
#### Install
`brew tap wushaobo/tap && brew install alembic-checker`

#### Run

`Usage: alembic-rev-graph [PATH/OF/ALEMBIC/VERSIONS/FOLDER]`

The default path is `$PWD`.

### With source code
#### Install dependencies
`brew install graphviz`

#### Save source code to executable file
```
wget https://github.com/wushaobo/alembic-checker/blob/master/alembic-rev-graph && chmod +x ./alembic-rev-graph
```

#### Run

`/PATH/TO/alembic-rev-graph [PATH/OF/ALEMBIC/VERSIONS/FOLDER]`

The default path is `$PWD`.


## Result
Normally, a healthy list of alembic revisions is two synchronized single linked lists, by revision and file name.

If the graph shows something abnormal as the image below, you absolutely merged the revisions wrongly with other developers.

![alembic-revision-in-wrong-sort](https://github.com/wushaobo/alembic-checker/raw/master/alembic-revision-in-wrong-sort.png)
