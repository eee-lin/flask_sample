# flask_sample

## 実行の仕方
`python app.py`

### venvの導入
[venvについて](https://qiita.com/fiftystorm36/items/b2fd47cf32c7694adc2e)

`pip install virtualenv`

`pip3 install virtualenv`

ここでうまくできなかった場合はpipがインストールされていないかアップデートされていない可能性もある。

`pip install -U pip`
virtualenvまでいけたら、`vitrual env`

```
(base) 〇〇:flask 〇〇$ virtualenv env
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

### DBの導入
`source env/bin/activate`

```
(env) (base) Yilin:flask zhouyilin$ python3
Python 3.7.6 (default, Jan  8 2020, 13:42:34) 
[Clang 4.0.1 (tags/RELEASE_401/final)] :: Anaconda, Inc. on darwin
Type "help", "copyright", "credits" or "license" for more information.
>>> from app import db
/Users/zhouyilin/Documents/Conv/flask/env/lib/python3.7/site-packages/flask_sqlalchemy/__init__.py:834: FSADeprecationWarning: SQLALCHEMY_TRACK_MODIFICATIONS adds significant overhead and will be disabled by default in the future.  Set it to True or False to suppress this warning.
  'SQLALCHEMY_TRACK_MODIFICATIONS adds significant overhead and '
>>> db.create_all()
>>> quit()
```
