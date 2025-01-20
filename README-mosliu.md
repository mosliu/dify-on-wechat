## 来源

本项目fork自 https://github.com/hanfangyuan4396/dify-on-wechat.git

## 更新方式 

### 从上游更新

#### 设定上游
```BASH
git remote add upstream https://github.com/hanfangyuan4396/dify-on-wechat.git
```

#### 从上游仓库更新代码的命令

获取上游仓库的更新

```BASH
git fetch upstream
合并上游代码到你的分支（通常是 main 或 master）
```
假设你的分支是 main，可以执行：

```BASH
git checkout main
git merge upstream/main
```
解决冲突（如果有的话）
根据提示解决冲突后，保存并继续合并：

```BASH
git add .
git commit
```
将合并后的代码推送到你自己的 fork 仓库

```BASH
git push origin main

```

## 设定代理

### 设定git代理

```BASH
git config --global http.proxy http://127.0.0.1:7890
git config --global https.proxy http://127.0.0.1:7890
```

### 取消git代理

```BASH
git config --global --unset http.proxy
git config --global --unset https.proxy
```

### 设定 cmd 或 powershell 代理

```BASH
set http_proxy=http://127.0.0.1:7890
set https_proxy=http://127.0.0.1:7890
```