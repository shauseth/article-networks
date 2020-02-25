# Visualizing connections between Research Papers using Network Graphs

If an research article mentions that Staph grow more rapidly in patients with oxidative stress and another research article outlines the factors that increase oxidative stress in the body, the fact that those factors will affect the severity of a Staph infection won't be known until someone connects the dots.

This script literally connects the dots by taking pmids as input and creating a network graph showing how the article are related. Each pair of articles is given a score using a similarity function which compares the keywords, titles and abstracts of the articles. The network graph thus created shows indirect relationships between artciles that would otherwise be hidden.

[Pubmed Parser](https://titipata.github.io/pubmed_parser/) was used for extracting the articles.
[NetworkX](https://networkx.github.io/documentation/stable/) was used for creating the network graphs.
