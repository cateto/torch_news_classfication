

# KoBERT-news-classfication

- KoBERT를 이용한 언론 주제 분류(Document Classfication)
- **현재 모델 업로드 안되있음**
- u2skind@gmail.com



#### Requirements

- Python >= 3.6
- PyTorch >= 1.7.0
- MXNet >= 1.4.0
- gluonnlp >= 0.6.0
- sentencepiece >= 0.1.6
- onnxruntime >= 0.3.0
- transformers >= 3.5.0



#### How to install

```console
pip install mxnet
pip install gluonnlp pandas tqdm
pip install sentencepiece
pip install transformers==3
pip install torch

pip install git+https://git@github.com/SKTBrain/KoBERT.git@master
```



#### Prediction

```console
python main.py --input_file {INPUT_FILE_PATH} --model_dir {SAVED_CKPT_PATH}

[for custom setting]

OR

python main.py

[for default setting]
model dir : './model/20210802/model.pt'
input file : './data/predict_lucy.csv'
```



#### Results

83% of accuracy



#### Structure

```console
├── bert                       # python class for load bert model
├── data             		   # data for predict
├── model                      # pytorch pretrained model
│   └── 20210802               
├── notebook                   # all source code made by colab
├── output                     # predicted data (csv)
├── main.py                    
├── predict.py
├── README.md
└── utils.py
```



