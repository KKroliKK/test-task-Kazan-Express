# Test-task KazanExpress
The specification of test task from KazanExpress is available [online](https://messy-mackerel-9e0.notion.site/KazanExpress-a1c88a25015041688c122b519ecb3078)<br>

My classificator is implemented as a tree of 245 small FCNNs.<br>
Dataset is represented as a tree structure which keeps products in leaf nodes and is able to submit correctly labeld data for each of 245 branch nodes categories FCNNs.<br>
I used two big dictionaries with word embeddings for Russian language: fasttext and wiki2vec. Each token is converted to concatenation of two embedding vectors (overall size 600).<br>
Solution with representation of product title as averege embeddings gave **hierarchical f1-score equal to 0.933**.
