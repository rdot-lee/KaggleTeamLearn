###### 下載repo
```Terminal
git clone git@github.com:Rich627/xx.git

```

###### 同步已下載的repo
```Terminal
git pull  git@github.com:Rich627/xx.git
```

###### 創建branch
```Terminal
git branch -m branch_name
```

###### 切換branch
```Terminal
git checkout branch_name
```

###### 合併branch過程
```Terminal
git checkout branch_name
#切換回主分支下
git checkout main/master
git merge branch_name
git push
```

###### 改branch名字
```Terminal
git branch -m old_name new_name 
```

###### 創建branch並切換過去
```Terminal
git checkout -b branch_name  
```

###### 查看這個資料夾有幾個branch
```Terminal
git branch 
```

###### 刪掉該brnach
```Terminal
git branch -d branch_name 
```
###### 查看所有url
```Terminal
git remote -v 
```

###### 添加url(名字可以打預設origin)
```Terminal
git remote add name url 
```

###### 更改url
```Terminal
git remote set-url name url
```

###### 推上github步驟
```Terminal
cd ..
git add .
git commit -m 'x'
git branch -M main
git branch add origin git@github.com:Rich627/xx.git
git push -u origin main
```


###### 與團隊協作GitHub
```Terminal
A是開repo的人,B是協作者
1.A先在github開一個repo
2.B去開A的repo下按fork(就會跑到自己的repo下)
3.Ｂ下`git clone SSH`SSH從Ｂ的repo下找
4.B在終端機下創一個branch`git branch branch_name`
--------------------------
B想要加檔案
1.`git checkout branch_name` branch_name是剛剛自己創的
2.coding
3.git add .
4.git commit -m 'message'
#推之前要同步
5.先在B的repo下主分支按`Sync fork`
6.`git pull origin main/master(主分之的名稱)`
7.git push -u origin branch_name
8.確認推上去後在B的repo下create pull requests
9.等待同意後就搞定了下次要加檔案再重新一次
```
###### Commit Message
https://wadehuanglearning.blogspot.com/2019/05/commit-commit-commit-why-what-commit.html