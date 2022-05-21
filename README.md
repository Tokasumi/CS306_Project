# CS306_Project

---

**Group Member: **

**Liu JieWen, Zhou MinTao, Li JiaJun, Shao GuanFang, **

**Guo Hui, He ChenRui, Lan ChenXi, Zeng HanYang**

**Course: SUSTech CS306 DataMining**



how to run demo:

* `git clone https://github.com/Uncle-Road/CS306_Project.git`

* make sure your computer has **annoconda envirment**

  * Interpreter setting in pycharm:

    *(suggest you make new conda envirment first by conda `create -n cs306 python==3.7` )*

    click File -> Settings -> Project: Project_name-> Python Interpreter -> choose conda envirment.

  * Terminal setting in pycharm:

    click File -> Settings -> Tools -> Terminal -> Shell path -> paste_content

    and you should paste *the softeware* of Anaconda Prompt (anaconda)'s attribute(属性) 's target(目标) from cmd.exe"/........

  * Envirment:

  ```
  (if you not create conda envirment)
  conda create -n cs306 python==3.7 
  
  conda activate cs306
  conda install pytorch==1.7.1 torchvision==0.8.2 torchaudio==0.7.2 cudatoolkit=10.1 -c pytorch
  pip install torchsummary
  pip install torch-summary
  pip uninstall scikit-learn
  conda install --user-local scikit-learn-0.24.2-py37hf11a4ad_2.tar.bz2
  ```

​		using `conda list` check packages version is right .make sure python == 3.7 and **scikit-learn == 0.24.2** 

* run code by terminal:

````
cd model
python pred_GraphWaveNet.py --epoch 1 --gpu 0
````

You can modify the parameters though **--aaa  b**, or get help using `--help` or see code in `pred_GraphWaveNet.py.`

