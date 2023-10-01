# Example Chroma vector embeddings

This is the companion code repository for [my blog post on vector embeddings with Chroma](https://stephencollins.tech/posts/how-to-use-chroma-to-store-and-query-vector-embeddings).

## Getting Started

I've written some very simple bash scripts purely for convenience for this example project. Assuming you have git installed, just:

```bash
sh pull.sh
```

to clone the chroma core repo and then:

```bash
sh start.sh
```

to run chroma in server mode in a _foreground_ process for easier testing with `app.py`.

## Run the Example

To run the example `app.py` Python application, install the requirements.txt file for `app.py`. And assuming you have a modern Python 3 version installed simply:

`python app.py`

This will do the following:

1. Create a Chroma client
2. Print a Chroma server heartbeat
3. Create or get a chroma collection
4. Add documents to the collection
5. Query the collection using Cosine Distance
6. Print the results including Cosine Similarity scores\*

_NOTE: Cosine Similarity = 1 - Cosine Distance_
