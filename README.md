## Installation

```
docker build -t mkdocs .
```

## Run

(copy/paste the whole thing the `\` is just for line breaking)
```
docker run --rm -it \
    -v $(pwd)/docs:/app/docs \
    -v $(pwd)/mkdocs.yml:/app/mkdocs.yml \
    -v $(pwd)/overrides:/app/overrides \
    -p 8000:8000 \
    mkdocs
