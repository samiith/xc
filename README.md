# xc

* Install dependencies: `conda install --yes --file requirements.txt`

* Parse and generate label graph from a file in the Dataset - `python utils/util.py <data_file_path> <label_file_path>`

Note: an example graph file is added already under `samples` to be viewed through [gephi](https://gephi.org)

[Gephi Tutorial](https://gephi.org/tutorials/gephi-tutorial-quick_start.pdf)

# Example graphs with different file formats:

1. [Zachary's Karate Graph](http://www.cise.ufl.edu/research/sparse/matrices/Newman/karate.html)
W. W. Zachary, An information flow model for conflict and fission in small groups, Journal of Anthropological Research 33, 452-473 (1977).
2. [Gnutella peer-to-peer network, August 8 2002](https://snap.stanford.edu/data/p2p-Gnutella08.html)
M. Ripeanu and I. Foster and A. Iamnitchi. Mapping the Gnutella Network: Properties of Large-Scale Peer-to-Peer Systems and Implications for System Design. IEEE Internet Computing Journal, 2002.
3. [BlogCatalog](http://leitang.net/social_dimension.html)
Lei Tang and Huan Liu. Relational Learning via Latent Social Dimensions. In Proceedings of The 15th ACM SIGKDD Conference on Knowledge Discovery and Data Mining (KDD'09), pages 817-826, 2009.

# To generate deepwalk output from any train or test file:

```
from exact_dxml import ExactDXML
ExactDXML().fit(<train_file_path>, <deepwalk_output_file_path>)
```
