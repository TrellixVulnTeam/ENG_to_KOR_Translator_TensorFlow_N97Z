[![tag][a]][1]
[![release][b]][2]
[![download][c]][3]
# Table of Contents <a name="anchor_main"></a>
---
1. [Running Environment](#anchor_1) <br></br>
2. [data](#anchor_2) <br></br>
3. [checkpoints](#anchor_3) <br></br>
4. [scripts](#anchor_4) <br></br>
5. [References](#anchor_ref) <br></br>

## Running Environment <a name="anchor_1"></a> [up](#anchor_main)
Virtualenv Python 2.7 with TensorFlow on it with following packages:

* pip install --upgrade jupyter
* pip install --upgrade pillow
* pip install --upgrade scikit-learn
* pip install --upgrade matplotlib
* pip install --upgrade scipy
* pip install --upgrade xlrd
* pip install --upgrade python\_speech\_features
* pip install --upgrade nltk
* pip install git+http://github.com/kylebgorman/textgrid.git
* pip install --upgrade JPype1
* pip install --upgrade konlpy

## data <a name="anchor_2"></a> [up](#anchor_main)
| Data               | Token id                    | Word list       |
| :-------:          | :---:                       | :----:          |  
| training\_set.from | training\_set.from.ids20000 | vocab20000.from | 
| training\_set.to   | training\_set.to.ids40000   | vocab40000.to   |  
| testing\_set.from  | testing\_set.from.ids20000  | vocab20000.from | 
| testing\_set.to    | testing\_set.to.ids40000    | vocab40000.to   | 

## checkpoints <a name="anchor_3"></a> [up](#anchor_main)
* checkpoints/checkpoint file sould be altered in a way: 
	
	```
	model_checkpoint_path: "/Your/path/to/translate.ckpt-27200"
	all_model_checkpoint_paths: "/Your/path/to/translate.ckpt-26400"
	all_model_checkpoint_paths: "/Your/path/to/translate.ckpt-26600"
	all_model_checkpoint_paths: "/Your/path/to/translate.ckpt-26800"
	all_model_checkpoint_paths: "/Your/path/to/translate.ckpt-27200"
	```
	
## scripts <a name="anchor_4"></a> [up](#anchor_main)
1. See upper part of translate.py, since everything can be controled from there.
2. data\_utils.py & seq2seq\_model.py are helper class & model creation class respectively.
3. To run, type "python translate.py" on TensorFlow activated terminal, or run on IDLE like Pycharm (interpreter as TensorFlow in this case).

## References <a name="anchor_ref"></a> [top](#anchor_main)
My [blog][4] <br></br>
Email: <kwb425@icloud.com>

<!--Links to addresses, reference Markdowns-->
[1]: https://github.com/kwb425/ENG_to_KOR_Translator_TensorFlow/tags
[2]: https://github.com/kwb425/ENG_to_KOR_Translator_TensorFlow/releases
[3]: https://github.com/kwb425/ENG_to_KOR_Translator_TensorFlow/releases
[4]: http://kwb425.github.io/
<!--Links to images, reference Markdowns-->
[a]: https://img.shields.io/badge/Tag-v1.2-red.svg?style=plastic
[b]: https://img.shields.io/badge/Release-v1.2-green.svg?style=plastic
[c]: https://img.shields.io/badge/Download-Click-blue.svg?style=plastic
