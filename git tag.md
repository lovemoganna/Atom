[详细链接](http://caibaojian.com/github-create-tag.html)

主要就是三步:

```
## 列出所有的标签
$ git tag
v0.1.1

##删除搞错的标签
Administrator@XTM-01702051132 MINGW64 /e/Article/dubboparent (master)
$ git tag -d v0.1.1
Deleted tag 'v0.1.1' (was 7012287)

//列出最近一次的提交
Administrator@XTM-01702051132 MINGW64 /e/Article/dubboparent (master)
$ git log --oneline
126401b (HEAD -> master, origin/master) springboot集成dubbo

//新建标签
Administrator@XTM-01702051132 MINGW64 /e/Article/dubboparent (master)
$ git tag -a v0.0.1 -m 'first version'

//将标签添加到最近的提交上面

Administrator@XTM-01702051132 MINGW64 /e/Article/dubboparent (master)
$ git tag -a v0.0.1 126401b
fatal: tag 'v0.0.1' already exists

//远程提交标签
Administrator@XTM-01702051132 MINGW64 /e/Article/dubboparent (master)
$ git push origin --tags
Counting objects: 1, done.
Writing objects: 100% (1/1), 163 bytes | 54.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0)
To github.com:lovemoganna/dubboparent.git
 * [new tag]         v0.0.1 -> v0.0.1


```
