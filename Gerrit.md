# 1    git clone "ssh://yangman@192.168.64.47:29418/arhud/2209/arhud" && scp -p -P 29418 yangman@192.168.64.47:hooks/commit-msg "arhud/.git/hooks/"
正克隆到 'arhud'...
remote: Counting objects: 7998, done
remote: Finding sources: 100% (7998/7998)
remote: Total 7998 (delta 3300), reused 7910 (delta 3300)
接收对象中: 100% (7998/7998), 417.24 MiB | 904.00 KiB/s, 完成.
处理 delta 中: 100% (3300/3300), 完成.
正在检出文件: 100% (3726/3726), 完成.
commit-msg                                    100% 2174    64.4KB/s   00:00  

# 2 cd arhud/

# 3    git status
位于分支 master
您的分支与上游分支 'origin/master' 一致。

无文件要提交，干净的工作区


# 4  git branch -vv
* master 01c0c0f [origin/master] add ARCommon and ARServer version

# 5  git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/master
  remotes/origin/predict


# 6  git checkout
您的分支与上游分支 'origin/master' 一致。


# 7  git checkout origin/predict
注意：正在检出 'origin/predict'。

您正处于分离头指针状态。您可以查看、做试验性的修改及提交，并且您可以通过另外
的检出分支操作丢弃在这个状态下所做的任何提交。

如果您想要通过创建分支来保留在此状态下所做的提交，您可以通过在检出命令添加
参数 -b 来实现（现在或稍后）。例如：

  git checkout -b <新分支名>

HEAD 目前位于 cdd990d initialize snpe
ym@ym:/media/ym/DATA1/AR-HUD/arhud_202


# 8  git status
头指针分离于 origin/predict
无文件要提交，干净的工作区


# 9  git branch -vv
  master                          01c0c0f [origin/master] add ARCommon and ARServer version
* （头指针分离于 origin/predict） cdd990d initialize snpe


# 10  git checkout predict
分支 'predict' 设置为跟踪来自 'origin' 的远程分支 'predict'。
切换到一个新分支 'predict'


# 11  git pull
已经是最新的。


# 12  git status
位于分支 predict
您的分支落后 'origin/predict' 共 1 个提交，并且可以快进。
  （使用 "git pull" 来更新您的本地分支）

尚未暂存以备提交的变更：
  （使用 "git add <文件>..." 更新要提交的内容）
  （使用 "git checkout -- <文件>..." 丢弃工作区的改动）

	修改：     AR_Creator/src/ARCommon/src/ProcessLine.cpp
	修改：     AR_Creator/src/ARCommon/src/ProcessObj.cpp
	修改：     AR_Creator/src/ARCommon/src/VirtualRegHandle.cpp


# 13  git reset --hard HEAD
HEAD 现在位于 cdd990d initialize snpe


# 14   git status
位于分支 predict
您的分支落后 'origin/predict' 共 1 个提交，并且可以快进。
  （使用 "git pull" 来更新您的本地分支）

无文件要提交，干净的工作区

# 15 git log
ommit 37fc2de24001c9d147c8371ab58b6caaa02c34f9 (HEAD -> predict, origin/predict)
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 17:14:03 2023 +0800

    update line prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: I2afb3d0f7d365c52e6c58f9dd1ed7cc035172fd3

commit e4290b3298fe3771684c020e055601ec5210c967
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 12:07:46 2023 +0800

    update object prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: Iee93902a301f148626ba0d3598727a466f06f599
:...skipping...
commit 37fc2de24001c9d147c8371ab58b6caaa02c34f9 (HEAD -> predict, origin/predict)
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 17:14:03 2023 +0800

    update line prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: I2afb3d0f7d365c52e6c58f9dd1ed7cc035172fd3

commit e4290b3298fe3771684c020e055601ec5210c967
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 12:07:46 2023 +0800

    update object prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: Iee93902a301f148626ba0d3598727a466f06f599

commit cdd990da3c759ed8acb50608fc081b20cfe5b850
commit 37fc2de24001c9d147c8371ab58b6caaa02c34f9 (HEAD -> predict, origin/predict)
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 17:14:03 2023 +0800

    update line prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: I2afb3d0f7d365c52e6c58f9dd1ed7cc035172fd3

commit e4290b3298fe3771684c020e055601ec5210c967
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Mon Feb 6 12:07:46 2023 +0800

    update object prediction
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: Iee93902a301f148626ba0d3598727a466f06f599

commit cdd990da3c759ed8acb50608fc081b20cfe5b850
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Fri Feb 3 18:28:38 2023 +0800

    initialize snpe
    
    Signed-off-by: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
    Change-Id: I5ba1b3e21023ccc153865647813034832c017f36

commit 995f25f7aa46538fdc19cc1de24abb34f1dbd356
Author: zhaoyanzhi <zhaoyanzhi@hangsheng.com.cn>
Date:   Fri Feb 3 16:16:44 2023 +0800

    predit
    
    Change-Id: I23d7a10217aa6df87230569545b4d25bc6afa9ab

commit 7bebd7b09babd0329eb67b807d43823ddb7bfdbe
Author: Jiaxin Zhou <zhoujiaxin@hangsheng.com.cn>
Date:   Tue Jan 31 09:36:07 2023 +0800
:

# git st
git：'st' 不是一个 git 命令。参见 'git --help'。
最相似的命令是
	status
	reset
	stage
	stash



# ---------------------------------------    上传代码     -----------------------------------------------------
git log 按住q结束
git add .
git commit -m 新增模型

git push origin HEAD:refs/for/predict


git checkout origin/develop
git push origin HEAD:refs/for/develop


git reset HEAD~3 回退到倒数第三个版
git commit --amend




git reset --hard HEAD~1

 git diff > 0211_11.diff

rm AR_Creator/0211_11.diff

git add .
git commit --amend   ctrl + X   新增修改的文件

git checkout -- AR_Creator/src/ 恢复目录下所有文集

git commit -s -m 'update 0214 final'



git fetch ssh://yangman@192.168.64.47:29418/arhud/2209/arhud refs/changes/08/9708/1 && git cherry-pick FETCH_HEAD





ssh bob@112.74.60.165
passwd： 3个空格键

