# Fast Adaptation to Super-Resolution Networks via Meta-Learning

Source code for ECCV2020 "Fast Adaptation to Super-Resolution Networks via Meta-Learning" [paper](https://arxiv.org/abs/2001.02905)


## Requirements

Check [requirements.txt](requirements.txt) to install all requirements.

```
conda install --file requirements.txt
```
or
```
pip install -i requirements.txt
```

## Usage

#### Training with Urban100 dataset

* Download Urban100 dataset [here](http://vllab.ucmerced.edu/wlai24/LapSRN/)
* Set Urban100 dataset directory name to `Urban100` and run `./split_urban100.sh`
* Download IDN pretrained weights `checkpoint_x2` [here](https://github.com/Zheng222/IDN-tensorflow)
* Start training

```console
python main.py --param-restore-path checkpoint_x2 --param-save-path mlsr_test_parameter
```

* You can also train with other dataset by using `--train-dataset` flag.


## Citation

If you find MLSR helpful, please consider citing our paper:

```bibtex
@article{park2020fast,
    title={Fast Adaptation to Super-Resolution Networks via Meta-Learning},
    author={Park, Seobin and Yoo, Jinsu and Cho, Donghyeon and Kim, Jiwon and Kim, Tae Hyun},
    journal={ECCV},
    year={2020}
}
```

