# medical_NER
本项目数据集来自ccks2017任务二,任务是中文病例的命名实体识别
## 数据处理后主要类标
>"O"
>"B-body"
>"I-body"
>"E-body"
>"B-symp"
>"I-symp"
>"E-symp"
>"B-dise"
>"I-dise"
>"E-dise"
>"B-chec"
>"I-chec"
>"E-chec"
>"B-cure"
>"I-cure"
>"E-cure"
## 模型结构
采用bi-LSTM+CRF/transformer+CRF，此后会对模型进行优化,数据根据需求处理。<br>
1.dataset文件夹 原始数据<br>
2.LSTM_CRF.py bi-LSTM模型<br>
3.data_util.py 数据处理<br>
4.train.py main<br>
5.transformer_CRF transformer模型
## Requirements
python 3<br>
tensorflow 1.12
## 评价指标
microF1 打分函数precision_recall_fscore_support
