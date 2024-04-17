# ColBERT requirements

## ColBERT checkpoint download
Public checkpoints for colbert

### colbertv2.0
- colbertv2, PLAID
- epoch: 150000 
- download by
```
cd encoder_checkpoints
wget https://downloads.cs.stanford.edu/nlp/data/colbert/colbertv2/colbertv2.0.tar.gz 
tar -xvf colbertv2.0.tar.gz
```

### msmarco.psg.l2
- colbertv1
- epoch: 300000
- download by
```
cd encoder_checkpoints
wget https://public.ukp.informatik.tu-darmstadt.de/thakur/BEIR/models/ColBERT/msmarco.psg.l2.zip 
unzip msmarco.psg.l2.zip 
```

## ColBERT dataset download
MS MARCO, Vaswani 

### MS MARCO
```
cd data/MSMARCO
wget https://msmarco.z22.web.core.windows.net/msmarcoranking/triples.train.small.tar.gz
tar -xvf triples.train.small.tar.gz
wget https://msmarco.z22.web.core.windows.net/msmarcoranking/top1000.dev.tar.gz
tar -xvf top1000.dev.tar.gz
wget https://msmarco.z22.web.core.windows.net/msmarcoranking/qrels.dev.tsv
tar -xvf qrels.dev.tsv
wget https://msmarco.z22.web.core.windows.net/msmarcoranking/collection.tar.gz 
tar -xvf collection.tar.gz 
wget https://msmarco.z22.web.core.windows.net/msmarcoranking/queries.tar.gz 
tar -xvf quries.tar.gz
```

### Vaswani
```
cd data/Vaswani
wget https://ir.dcs.gla.ac.uk/resources/test_collections/npl/npl.tar.gz
tar -xvf npl.tar.gz
rm npl.tar.gz
```

## ColBERT index
Vaswani -171MB  
MS MARCO - 163GB