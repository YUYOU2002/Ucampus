## 程序说明

程序目的主要还是练手自动化  ~~*顺便偷懒*,~~

~~答案接口：https://uexercise.unipus.cn/itest/t/clsExam/rate/detail?%s%s%s' % (exercise, sign, sid) sid是登录之后页面pagesource里的studentid:~~



迫于总是有人不会手动获取sid然后私信的无奈，增加了自动获取sid,现在只需要填写账号密码了

不过还请手动配置 <a href="https://npm.taobao.org/mirrors/chromedriver/" target="__blank">chromedriver</a>

选择自己谷歌相应版本的chromedriver然后把exe文件移动到chromedriver文件夹下，**并改成相应格式的名字**



**支持的 course：**

*新四级强化辅导课程，新视野大学英语的单元测验部分*

~~*有时间的人其他课程可以试一试，万一也可用呢？（如果可用还请告诉我一声）*~~

**支持题型：**

(暂不支持自动填写作文翻译😂，但是仍可用)

* **纯填空**: 复合式听写|仔细阅读|长篇阅读
* **选词填空**:词汇理解...~~（功能匮乏~~
* **选择题**:短对话，长对话，新闻报道

**环境配置：**

win10 x64

## 使用说明

### 配置文件

* 第一次使用需要你配置config中你的用户名，密码~~(可以在config里直接改)~~之后是默认你第一次的配置

  如果你想改配置：

  可以在config.ini里面直接改

  也可以在程序里按照提示输入相应指令

### 配置参数说明：

* is_auto_submit=1 代表自动提交|不建议，所以默认为0 (待优化，还未能使用)
* is_close_answerwindow=1 代表关闭出现的答案窗口|自行决定
* username 登录账号
* password 登录密码
* studentId sid
* auto_fill_answer=1 代表自动答题 默认1
* v_chromedriver 谷歌版本号
* wtmax 间隔最大时间 /second 默认0.3s
* wtmin 间隔最小时间 /second 默认0.3s

### 自动答题

**进入需要完成的test，确认开始后即可自动**，自动答题中**不要**切换窗口以防终止答题

##  一些常见issue：

* **自动填写并未填写完**：可到关闭测验再执行一遍，因为有时候答案数据未加载出来，具体可以在答案页面看见
* **有黑方框但是程序登录页面打不开**:**检查本程序是否支持你的谷歌版本**，或者是账号密码错误
* **答案页面显示不了答案**:务必检查一下sid是否正确，如果还是显示不出来可以私聊我
* **如果黑方框闪退**：~~这个原因挺多~~ 先看一下是不是下载的压缩包，不要单独下载exe，也有可能是杀毒软件的锅

**（提交时若显示你有题未作答是因为U校园系统没有来得及保存，不用管直接提交就好了）**

最后记得退出程序



## 特别感谢

* [ 85853444](https://github.com/858534444)

* zhou1024

**对本程序的支持，以及陪我耐心的调试**

## 本程序仅供学习交流，欢迎开issue讨论

使用本程序一切后果，本人概不负责