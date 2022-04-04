# AAGCN-ACSA

  
**Beta Distribution Guided Aspect-aware Graph for Aspect Category Sentiment Analysis with Affective Knowledge**


## Usage

* Install [SpaCy](https://spacy.io/) package and language models with
```bash
pip install spacy
```
and
```bash
python3 -m spacy download en
```


## Training
* For non-BERT implementation. Please train with command, optional arguments could be found in [train.py](/train.py)
```bash
./train.sh
```
* For BERT-based implementation. Please train with command, optional arguments could be found in [train_bert.py](/train_bert.py)
```bash
./train_bert.sh
```

## See also
* The process of graph generation could be found at [./dataset/generate_graph.py](/dataset/generate_graph.py).
* The source of [SenticNet](https://sentic.net/) could be found at https://sentic.net/downloads/.
* The source of [ConceptNet](https://www.aaai.org/ocs/index.php/AAAI/AAAI17/paper/viewFile/14972/14051) could be downloaded ate https://github.com/commonsense/conceptnet5.


```
#原来的14运行结果，github上新版的重写了14的运行命令
python train_bert.py --model aagcn_bert --dataset 14_sen
#我的sem_all
python train_bert_sem.py --model aagcn_bert --dataset sem_all_sen
