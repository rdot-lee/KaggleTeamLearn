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

###### Commit Message
https://wadehuanglearning.blogspot.com/2019/05/commit-commit-commit-why-what-commit.html