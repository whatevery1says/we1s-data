# we1s-data

`we1s-data` a test/demo repository of file-side data for corpora and projects, using JSON files written according to the current WE1S Manifest system.

Example raw articles in the system have been "greeked" with lorem ipsum text, however the processed articles reflect real article word-bags.

The first prototype of the integrated WE1S frontend workspace and backend management system will be hosted in the workspace, and will perform interactions with corpora and projects using

1. first, the local filesystem 
2. later a separate fileserver
3. finally a MongoDB backend

This data mocks up the first two phases as a collection of JSON files stored in a directory heirarchy. Once this example data and directory heirarchy is correct in terms of the manifest schema, it can be used to test scripts written against:

1. conversion scripts (convert our current CSV stores into JSON equivalents)
2. ingest scripts (take output e.g. continuous raw text dumps from APIs and parse out per-article JSON pointing at per-article text resources.
3. conversion scripts (e.g. deconstruct the original text through word-bagging to avoid storing originals)
4. search scripts (that prototype crawling the heirarchy and finding a corpus/corpora or a project/projects according to criteria)
5. upload scripts (which mock sending corpora or projects to the remote system, e.g. MongoDB)
6. download scripts (which mock sending retrieving corpora / projects from the remote system, e.g. MongoDB)
