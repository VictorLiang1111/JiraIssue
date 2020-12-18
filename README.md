# 取得JIRA單

### 配置

設置目錄內的climbIssue.ini配置

```
[DEFAULT]
server=https://sample.atlassian.net \\ jira的server路徑
user_name=                          \\ jira的使用者信箱
api_key=                            \\ jira的使用者API key
finish_text=Done                    \\ 完成的key word
```

### 開始測試
1. 主要檔案為climbIssue.py

2. 執行
```
py climbIssue.py
```

3. 依序填入專案名稱,專案spring,issue被指派人

```
Please enter project(ZRSH):
Please enter Sprint(openSprints()):
Please enter assignee people(self):
```

4. 完成後便會將jira issue寫入在同目錄底下的output.txt檔案

5. 修改完檔案後,使用pyinstaller指令打包成exe檔
```
pyinstaller -F climbIssue.py
```

### exe檔案操作
1. 拿到.exe檔案後，設置目錄內的climbIssue.ini配置

```
[DEFAULT]
server=https://sample.atlassian.net \\ jira的server路徑
user_name=                          \\ jira的使用者信箱
api_key=                            \\ jira的使用者API key
finish_text=Done                    \\ 完成的key word
```

2. 點擊.exe檔案,並依序填入專案名稱,專案spring,issue被指派人

```
Please enter project(ZRSH):
Please enter Sprint(openSprints()):
Please enter assignee people(self):
```
