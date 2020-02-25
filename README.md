# Visualizing connections between Research Papers using Network Graphs

If a research paper mentions that staph grow more rapidly in patients with oxidative stress and another outlines the factors that increase oxidative stress in the body, the fact that those factors will affect the severity of a staph infection won't be known until someone connects the dots.

[This script](/12_final.ipynb) literally connects the dots by taking pmids as input and creating a network graph showing how the article are related. Each pair of articles is given a score using a similarity function which compares the keywords, titles and abstracts of the articles. The network graph thus created shows indirect relationships between artciles that would otherwise be hidden.

![Network Graph](/graph.png)

The solid lines show that the keywords match between the artciles and the dashed lines show that the keywords in one article were present in the title or the abstract of the other or vice versa. Nodes that are closer have more similarity. In this case, article 1 and 2 were about staph, 3 was about phage therapy, 4 was about pollution and 5 about diet.

[Pubmed Parser](https://titipata.github.io/pubmed_parser/) was used for extracting the articles.

[NetworkX](https://networkx.github.io/documentation/stable/) was used for creating the network graphs.
