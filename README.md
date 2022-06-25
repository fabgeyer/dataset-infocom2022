# Network Synthesis under Delay Constraints: The Power of Network Calculus Differentiability

This repository contains the dataset used for the paper [_"Network Synthesis under Delay Constraints: The Power of Network Calculus Differentiability"_](https://doi.org/10.1109/INFOCOM48880.2022.9796777) published at the [41th IEEE International Conference on Computer Communications (INFOCOM 2022)](http://infocom2022.ieee-infocom.org/). We refer to the paper for a full explanation of the methodology used for generating the dataset.


## Information

The dataset is comprised of two files:

- `dataset-eval-section5.pbz` is the dataset used for the evaluation in Section V,
- `dataset-eval-section6.pbz` is the dataset used for the evaluation in Section VI.

Additionally, [`dataset_structure.proto`](https://github.com/fabgeyer/dataset-infocom2022/blob/master/dataset_structure.proto) details the datastructure used for the dataset.

The dataset is stored as serialized protobuf messages using the Python library [pbzlib](https://github.com/fabgeyer/pbzlib-py).
Alternative programming languages may be used with `pbzlib` (e.g. [Java](https://github.com/fabgeyer/pbzlib-java), [Go](https://github.com/fabgeyer/pbzlib-go)).

This repository contains an [example python script](https://github.com/fabgeyer/dataset-infocom2022/blob/master/example.py) for parsing the files.
To get it and execute it:
```
$ git clone https://github.com/fabgeyer/dataset-infocom2022.git
$ cd dataset-infocom2022
$ pip3 install -r requirements.txt
$ python3 example.py dataset-eval-section6.pbz
```

## Citation

If you use this dataset for your research, please include the following reference in any resulting publication:

```bibtex
@inproceedings{GeyerBondorf_INFOCOM2022,
	author    = {Geyer, Fabien and Bondorf, Steffen},
	title     = {Network Synthesis under Delay Constraints: The Power of Network Calculus Differentiability},
	booktitle = {Proceedings of the 41th IEEE International Conference on Computer Communications (INFOCOM)},
	year      = {2022},
	month     = may,
}
```

## License

The data in this repository is licensed under [Creative Commons Attribution-ShareAlike 4.0 International (CC BY-SA 4.0)](http://creativecommons.org/licenses/by-sa/4.0).
