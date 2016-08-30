1) Make a git repo
2) make sure python is setup on computer

3) set `pip`, `python` and `git` in environment path on windows system

4) install deps
```
pip install python-crontab
```

5) Run first time
```
git config credential.helper store
```

6) create windows schtasks
```
schtasks /Create /ST 16:00 /ET 18:00 /TN FileBackerUpper /SC minute /MO 10 /TR "python C:\Users\Tom\Desktop\file_backup\file_backup\file_backup.py"
```

7) how to see schtasks
```
schtasks /Query /TN filebackerupper
```
