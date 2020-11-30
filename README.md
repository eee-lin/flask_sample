# flask_sample

## 実行の仕方
`python app.py`

### venvの導入
[venvについて](https://qiita.com/fiftystorm36/items/b2fd47cf32c7694adc2e)

`pip install virtualenv`

ここでうまくできなかった場合はpipがインストールされていないかアップデートされていない可能性もある。

`pip install -U pip`
virtualenvまでいけたら、`vitrual env`

```
(base) Yilin:flask zhouyilin$ virtualenv env
created virtual environment CPython3.7.6.final.0-64 in 1342ms
  creator CPython3Posix(dest=/Users/zhouyilin/Documents/Conv/flask/env, clear=False, no_vcs_ignore=False, global=False)
  seeder FromAppData(download=False, pip=bundle, setuptools=bundle, wheel=bundle, via=copy, app_data_dir=/Users/zhouyilin/Library/Application Support/virtualenv)
    added seed packages: pip==20.2.4, setuptools==50.3.2, wheel==0.35.1
  activators BashActivator,CShellActivator,FishActivator,PowerShellActivator,PythonActivator,XonshActivator
  ```

  `virtualenv env`  
  
  ```
  ├── templates
│   ├── base.html
│   └── index.html
├── env
└── app.py
```
