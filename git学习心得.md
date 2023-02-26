#### P2 02 版本控制器的方式

![image-20230225090315473](git学习心得.assets/image-20230225090315473.png)



![image-20230225090627606](git学习心得.assets/image-20230225090627606.png)









![image-20230225090520336](git学习心得.assets/image-20230225090520336.png)

![image-20230225090600495](git学习心得.assets/image-20230225090600495.png)







#### P4 04 git工作流程简述

![image-20230225090948573](git学习心得.assets/image-20230225090948573.png)







#### P5 05 git环境配置与安装



git bash 是个linux命令行



设置用户名和信息



![image-20230225091611773](git学习心得.assets/image-20230225091611773.png)



![image-20230225091857754](git学习心得.assets/image-20230225091857754.png)











#### P6 06 获取本地仓库



* 先 git init建立本地仓库





#### P7 07 git常用指令

![image-20230225092458735](git学习心得.assets/image-20230225092458735.png)



> touch + 文件名 创建文件

> git status 查看文件状态

![image-20230225093100857](git学习心得.assets/image-20230225093100857.png)



* untracked 未跟踪的状态



* git add + 文件名 或者通配符 . （即全部文件）
* 然后提交

> git commit -m "注释"





查看日志

> git log 





![image-20230225093720514](git学习心得.assets/image-20230225093720514.png)



![image-20230225093742272](git学习心得.assets/image-20230225093742272.png)







* 再次修改，就会再次进入工作区

![image-20230225093922031](git学习心得.assets/image-20230225093922031.png)



![image-20230225094348930](git学习心得.assets/image-20230225094348930.png)





![image-20230225094700873](git学习心得.assets/image-20230225094700873.png)



![image-20230225094817906](git学习心得.assets/image-20230225094817906.png)

、、、、、、、













* 版本回退

![image-20230225102312242](git学习心得.assets/image-20230225102312242.png)



* 下面的只在git bash官方提供的命令行才可以用

* 选中默认就是复制
* 按住滚轮就是黏贴

![image-20230225102825603](git学习心得.assets/image-20230225102825603.png)





* git reflog查看已经删除的记录



* .gitignore忽略管理文件













#### P9 09 git分支 常用指令

![image-20230225103633746](git学习心得.assets/image-20230225103633746.png)

![image-20230225103756044](git学习心得.assets/image-20230225103756044.png)









* head指向谁，谁就是当前分支，并且你切换分支，相应的本地仓库文件也会变



![image-20230225104505259](git学习心得.assets/image-20230225104505259.png)



* 把dev01合并到master分支上来

![image-20230225105153409](git学习心得.assets/image-20230225105153409.png)















#### P10 10 解决冲突



* 如果两个改了同一行代码，会要你来解决这个冲突

![image-20230225105656886](git学习心得.assets/image-20230225105656886.png)









* 手动更改之后，再add和commit



![image-20230225110148723](git学习心得.assets/image-20230225110148723.png)







![image-20230225110224294](git学习心得.assets/image-20230225110224294.png)













#### p11 11 分支使用流程

![image-20230225110301733](git学习心得.assets/image-20230225110301733.png)



![image-20230225110451070](git学习心得.assets/image-20230225110451070.png)









#### P13 强制删除分支

![image-20230225110742481](git学习心得.assets/image-20230225110742481.png)

* 这种就是可以强制删除了

![image-20230225110956900](git学习心得.assets/image-20230225110956900.png)







#### P15 合并的快进模式

* 想让master主分支，直接到最新状态，那就直接快进
* git merge dev（dev是最新分支名

![image-20230225111808915](git学习心得.assets/image-20230225111808915.png)











#### P16 16 仓库托管 注册 创建仓库 配置公钥



![image-20230225112726988](git学习心得.assets/image-20230225112726988.png)







![image-20230225113319355](git学习心得.assets/image-20230225113319355.png)



* 连接gitee

  ![image-20230226103935254](git学习心得.assets/image-20230226103935254.png)







#### P17 远程仓库添加  查看 推送



* 在本地仓库要告诉是远程仓库的哪个库

> git remote add origin  ssh地址(这里origin是名字)

> git remote 查看远程仓库

> git push origin master   将master分支的内容推送到远程仓库origin

![image-20230225114307117](git学习心得.assets/image-20230225114307117.png)





![image-20230225114419654](git学习心得.assets/image-20230225114419654.png)



* -f 强制覆盖，如果远端仓库 有相同的会冲突，一般不用 

* 推送的时候 还是要注意推送关系   本地分支:远端分支



* 下面设置完直接就能推

![image-20230225114922388](git学习心得.assets/image-20230225114922388.png)







#### P19 clone

![image-20230225115055806](git学习心得.assets/image-20230225115055806.png)



* 可以在最后设置名字



![image-20230225115222652](git学习心得.assets/image-20230225115222652.png)









#### P20 20抓取和拉取

![image-20230225115434135](git学习心得.assets/image-20230225115434135.png)





* 右边拉取，查看git log然后再合并，



![image-20230225115638598](git学习心得.assets/image-20230225115638598.png)



* git pull  拉取+合并







#### P21 远程解决冲突

![image-20230225120408671](git学习心得.assets/image-20230225120408671.png)



* 经验

* 在push之前，先pull 拉取下来合并在本地解决冲突，解决完再push上去

![image-20230225120539733](git学习心得.assets/image-20230225120539733.png)

![image-20230225120627580](git学习心得.assets/image-20230225120627580.png)









#### P23 23 -idea配置 本地基本操作 push



![image-20230225121242297](git学习心得.assets/image-20230225121242297.png)





* idea弱化了 暂存区 add，想commit的就勾选就行











#### P24 idea克隆更新 更新 解决冲突



![image-20230225122113533](git学习心得.assets/image-20230225122113533.png)



* idea有提供自己的解决冲突的功能，修改完成之后就提交推送

* 右键文件是有add选项的









#### P25 分支操作

![image-20230225122456721](git学习心得.assets/image-20230225122456721.png)

* 查看本地分支远程分支





![image-20230225122639560](git学习心得.assets/image-20230225122639560.png)

* 直接右键创建分支就行了







#### P26 26 idea快速操作入口



![image-20230225122910125](git学习心得.assets/image-20230225122910125.png)



![image-20230225124339820](git学习心得.assets/image-20230225124339820.png)

![image-20230225124255686](git学习心得.assets/image-20230225124255686.png)







#### P28 28 几条铁令 idea集成gitbash



* 切换分支 先提交本地修改
* 代码即使提交，提交过了就不会丢
* 

![image-20230225124622523](git学习心得.assets/image-20230225124622523.png)

![image-20230225124644654](git学习心得.assets/image-20230225124644654.png)