# ACA4NMT
This is the code for our paper *Decoding History Based Adaptive Control of Attention for Neural Machine Translation*, https://arxiv.org/abs/1802.01812

***********************************************************

## Requirements
* Ubuntu 16.0.4
* Python3.5
* Pytorch 0.3.1

**************************************************************

## Preprocess
```
python3 preprocess.py -load_data path_to_data -save_data path_to_store_data 
```
Remember to put the data into a folder and name them *train.src*, *train.tgt*, *valid.src*, *valid.tgt*, *test.src* and *test.tgt*, and make a new folder inside called *data*

***************************************************************

## Training
```
python3 train.py -log log_name -config config_yaml -gpus id
```

****************************************************************

# Evaluation
```
python3 train.py -log log_name -config config_yaml -gpus id -restore checkpoint -mode eval
```

*******************************************************************

# Citation
If you use this code for your research, please cite the paper this code is based on: <a href="https://arxiv.org/abs/1802.01812.pdf"> Decoding History Based Adaptive Control of Attention for Neural Machine Translation</a>:
```
@article{decodinghistory,
  title   ={Decoding History Based Adaptive Control of Attention for Neural Machine Translation},
  author  ={Junyang Lin and Shumina Ma and Qi Su and Xu Sun},
  journal ={arxiv},
  year    ={2018},
  volume  ={abs/1802.01812}
}
```
