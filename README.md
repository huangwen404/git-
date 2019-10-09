###  git rebase 和 git merge
git rebase翻译过来叫变基,即改变起始节点,
举例:master分支1-2-3,1处switch一个dev分支,产生3个commit:4-5-6,
当前最新节点为master3,当你在dev执行git rebase master,会将dev最近的共同节点1之后的456取消挪到3之后,成为新的commit,
原来的基点是1,现在变为3,这就叫变基;
使用merge,如果存在冲突或者选择--no-ff参数,则会在3后面增加一个commit7


### git revert 和 git reset
后者会丢失commit历史一般不推荐
