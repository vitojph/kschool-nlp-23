# Download models and word vectors

## spaCy models for English and Spanish

    python -m spacy download en_core_web_md
    python -m spacy download es_core_news_md

## word2vec embeddings for Spanish (computed from Spanish Wikipedia)

Download the word vectors directly using [this Google Drive link](
https://drive.google.com/file/d/13_wOzznlWJATHDaVtsCOMqOqI3Q_hH93/view?usp=sharing) and save it inside your `data/` directory:

Or try to download them from a terminal using command line tools:

    [ -d data ] || mkdir data
    cd data
    wget -O eswiki-300.tar.gz https://vitojph.keybase.pub/eswiki-300.tar.gz?dl=1

## fastText word vectors for English and Spanish

    [ -d data ] || mkdir data
    cd data
    
    wget https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.en.300.vec.gz
    wget https://dl.fbaipublicfiles.com/fasttext/vectors-crawl/cc.es.300.vec.gz

