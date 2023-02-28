# GROQ

An self challenge to write GROQ (Graph-Relational Object Queries) tooling.

I aim to cover formatting and querying. Formatting will cover both removing all
white-space (eg for transmitting to the server) and pretty formatting (for human
readability). Querying will cover running GROQ strings against JSON objects.

Eventually I aim to be able to make this into a Sanity mirror server-app
constantly syncing from a Sanity dataset. In this scenario, it would be helpful
for the server admin to be able to specify indexes so that particular queries
can run faster. A simple index might be `*[_id == $id]` or `*[_type == $type]`
(syntax TBD). A more complicated index might be `*[references($ref)]`. Possibly
pre-sorting will be supported `*[_type == "film"] | order(releaseYear)`.

## Links

[GROQ specifications](https://sanity-io.github.io/GROQ/)

[Sanity GROQ documentation hub](https://www.sanity.io/docs/groq)
