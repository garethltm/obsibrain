- finding relevant documents in a search engine
- [[Term Frequency (tf)]]
- [[Inverse Document Frequency (idf)]]
- For query with terms t (eg: ("another","sample")) the best match document is:$$args\ max\ \Pi \tiny i\ \ \normalsize {tf(t\tiny i \normalsize,d)}\ \cdot \ idf(t\tiny i \normalsize,D)$$
- d∈D
- ${tf(t\tiny i \normalsize,d)}$ = increases the more times your term appears
- More often, we rank the documents, rather than take the best
	- you calculate through various pages
	- highest score = most relevant

[[Term Frequency (tf)]]-[[Inverse Document Frequency (idf)]] approximates the mutual information between each document & query (original search query)