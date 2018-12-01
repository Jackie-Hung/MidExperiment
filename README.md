# MidExperiment
It's the middle experiment for 地表最强队 !

## 任务分配

#### 黄俊
* 完成添加书籍信息到购物车（购物车可不用数据库保存）
* 完成登录用户查看购物车功能（购物车可删除商品和修改商品数量）

#### 吴洪杰
* 完成登录用户通过购物车提交订单功能
* 登录用户可查看自己的订单信息

#### 邹玉欣
* 完成书籍录入功能，（包括书籍类别和书籍信息功能）
* 后台用户信息查询

#### 吴伟正
* 后台查看全部用户订单功能（可按类型查询，初始订单、已完成订单）
* 服务端功能页面优化

#### 徐志雄
* 后台修改订单状态功能
* 客户端功能页面优化

## how to merge request
* http://www.cnblogs.com/WangYunShuaiBaoLe/p/WY.html
## git commit
* When you commit your Code,you have to write `commit message`;if not,your submission would be `failed`.

## Format of commit message
```bash
<type> (<scope>):<subject>#Header
#leave one blank line
<body>
#leave one blank line
<footer>
```
* Header is `necessary`,you can `ignore Body and Footer`.
* Any line must be less than `72` character in order to avoid automatic line changing.
### Header
* THere is only one line,which is consist of type`necessary`,scope`optional`,subject`necessary`.
#### type
* type is used to explain the category of commit,only contain :
 * `feat`:feature
 * `fix`:repair bug
 * docs:documentation
 * style:style (no code change)
 * refactor:restructure
 * test:increase the test
 * chore:change in the construction or anxiliary tools
* if type is feat or fix,and this commit must be in Change log.the others are recommended not to increase.

#### scope
* scope is used to explain the range of commit's effect,such as control layer,view layer.
#### subject
* subject is a brief decription of commt's purpose,less than `50` character.
* `warning`: Beginning with `verbs`,using the first person present tense.
* `warning`: like change,no changed or changes
* `warning`:first letter should be `lowercase` , Ending without  `. ` 
### Body
* None
### Footer
* None
### Reset
* Exceptional case:if this commit is used to revoke previous commit,you have to use `reset` 
```bash
#Revoke from tailend
git reset HEAD^
#commit again
```
## Change log
* If your all commit meet Angular format,change log can be built by script.
#document includes 
* New feature
* Bug fixes
* Breaking changes
```bash
#the code to build change log
$ npm install -g conventional-changelog
$ cd my-project
$ conventional-changelog -p angular -i CHANGELOG.md -w -r 0
```
## Merge Request
* You have to select master branch to submit for Source branch.
* Title: WIP:`your name`,like WIP:zbm
* `description`: you can write what you write in commit message.
* That's all.


