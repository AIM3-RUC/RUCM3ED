# RUCM3ED
M3ED: Multi-modal Multi-scene Multi-label Emotional Dialogue Database. ACL 2022

We have released the annotations, text and speech info. and the visual features(copy-right issues).

## label-info:
{'Happy':0, 'Neutral':1, 'Sad':2, 'Disgust':3, 'Anger': 4, 'Fear': 5, 'Surprise':6}

## Feature Extractions (Utterance-level):
### Text Modality:
https://huggingface.co/hfl/chinese-roberta-wwm-ext
    1. sen_avg_roberta: extract the word-level features and use the mean pooling to get the utterance-level features.
    2. finetune_cls_roberta: Finetuned on M3ED and extract the high-level emotional features.
    
### Audio Modality:
https://huggingface.co/jonatasgrosman/wav2vec2-large-xlsr-53-chinese-zh-cn
    1. sen_is10: OpenSmile 抽取句子级别的 IS10 情感特征，需要做 z-norm
    2. sen_avg_wav2vec: 帧级别的wav2vec特征直接平均作为句子特征
    3. finetune_cls_wav2vec: 在M3ED数据集上Finetune之后抽取的句子级别的情感特征。

### Visual Modality:
    1. sen_avg_affectdenseface

### M3ED Features（Have same format with DialogueRNN）
链接: https://pan.baidu.com/s/1xip42FAEBeBteSMUNYtHtQ 提取码: y95k 

### M3ED audio clips：
链接: https://pan.baidu.com/s/1JvaTabyKoQiWx2GtAIhpdw 提取码: 6b5q

## Different Models (DialgueRNN, DialogueGCN, MMGCN, MDI):

### DialgueRNN

### DialogueGCN
### MMGCN

### MDI
