# Chunk boundaries decide retrieval quality more than the embedding model

Splitting on a fixed token count cuts through the middle of the fact being retrieved. Splitting on document structure (headings, paragraph, list item) with a small overlap keeps the answer intact inside a single chunk. Swapping to a better embedding model rarely recovers what bad chunking loses.
