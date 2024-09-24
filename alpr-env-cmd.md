### To create a conda environment to run [alpr code](https://github.com/sergiomsilva/alpr-unconstrained)
  ```bash
  conda remove --name env_name --all
  conda create --name env_name python=2.7
  conda activate env_name
  conda install pip
  python -m ensurepip --upgrade
  conda install -c conda-forge opencv
  pip install keras==2.2.4
  pip install tensorflow==1.5.0
  ```
`python -m ensurepip --upgrade` was used to solve this issue:

  ```bash
  Traceback (most recent call last):
    File "/home/yeasar/anaconda3/envs/darknet_env2/bin/pip", line 6, in <module>
      from pip._internal.cli.main import main
  ImportError: No module named pip._internal.cli.main
  ```
