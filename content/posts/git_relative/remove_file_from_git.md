---
title: "Remove File from Git"
date: 2022-11-06T13:54:15+08:00
draft: false
tags: ['git']
categories: ['git']
---

git雖然非常好用，但如果不小心讓git追縱到有帳號跟密碼的檔案或不必要的檔案，絕對是一件非常麻煩的事。所以剛建立專案時，要下第一個commit時，都會確定有建立`.gitignore`檔，並確定把不需要追縱的檔案加入其中。

昨天在逛自己的`github`時，無意間發現自己的某一個專案，不小心把Dataset讓git追縱到，於是寫一下筆記記錄如何完整刪除被git追縱的檔案。


## Method

在`git`中的`filter-branch`，可以利用指定的指令來覆寫所有的Git的所有commit，像是刪除git每個commit中的檔案。

使用`filter-branch`來刪除所有commit中的檔案，其中的`-f`參數可以用來強制覆寫`filter-branch`的備分點
```shell
git filter -f --tree-filter "rm -f <file name>"
```

刪除備份點
```shell
rm refs/orignal/refs/heads/<branch>
```

使得Reflog立刻過期
```shell
git Reflog expire --all --expire=now
```

啟用資源回收機制將垃圾載走
```shell
git gc --prune-now
```


## 參考資料

- [【冷知識】怎麼樣把檔案真正的從 Git 裡移掉？](https://gitbook.tw/chapters/faq/remove-files-from-git)
- [Day26｜【Git】 從 Git 中移除重要個資或徹底清除檔案 - git filter-branch](https://ithelp.ithome.com.tw/articles/10279857?sc=rss.iron)


