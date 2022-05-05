- 概率论专业，不是程序员
- 自创玢璃哲学，《渡劫攻略One》《晨花研究史》作者
- zero980531@163.com但是不常上
- 
- latex中文优化头文件『玢辣』文档作者
- 辣得爽也好，辣眼睛也好，『玢辣』，让你第一次用就比axmath快
- 转载声明：唯一限制为标注出处，这样方便使用者更新。


- fenla编码示例：
- 存在：\cunzai；α：\alf或\alp（非数学环境为\alf\*或\alp*）；≠：\bd；→：\yjt或\qy（趋于）；
- 盒子：\hezi；花体A：\Ah（A花；非数学环境为\Ah*）；红色字体：\hs；
- 有序列表：\begin{yxlb}（只有begin和end不准备拼音化）。


- 2022/03/27更新1.1版本，完善了矩阵代数/颜色/系统自带常用功能的翻译和编码
- 2022/03/29更新1.2版本，修复方程组大括号功能，追加页面底色/图片
- 2022/04/01更新1.2.1版本，增加了适合中文用户的希腊字母三字简码规则；现在，希腊字母、英文字母（含花体和空心体）、数字、趋于符号四类经常出现在正文中的符号可以免去美元符号直接输入了（建议使用单个字符）
- 2022/04/01更新1.2.2版本，增加ppt功能（实际上是beamer引擎）（试用版；将在下个版本完善）（预计会出一个用户手册）
- 2022/04/11更新1.2.5版本，完善了ppt功能，制作了fenla专属的ppt模板。
- 2022/04/？？更新1.2.6版本，新增『加字』功能可以自定义符号、各种收敛的整体认读、缺乏的正体符号、长等号、等问号等；新增『Bilibili』平台发布的用户手册第一期，搜索『玢辣』。
- -----------------------------------------------------------------
- 2022/05/04更新1.2.7大版本『云夜之家』。
- 1. 修复了『加字』功能与『矩阵』功能冲突的bug。因使用率，取消『加字』简码留给矩阵。
- 2. ！统一了『矩阵』『行列式』和『数组』的写法，统一为『环境』。（但部分适合函数+环境双编码的仍会保留。特殊规则：环境名用该用的编码，函数名用fl+简码，以避免重名）。
- 3. ！重制了环境和函数双版本的『数学八股文』（实际为11股：问题（环境：wenti；函数：flwt；下面同理）、假设、定义、性质、命题、引理、定理、证明、推论、注释、例子）。
- 4. ！设置了『云夜之家』版本主题的页面背景图片（在fenla.sty的37、39行手动开启）；开放页面背景图功能（刚打开VS环境后编译第2次后生效！）。
- 5. ！设置了章、节、小节、小小节4级标题及其效果。
- 6. 勉强修复了因德式字体而无法在数学模式为字母添加汉语拼音2-4声的头顶符号的bug（效果一般，自己做了3个）。
- 7. 新增\fen式的偏导数功能：\pd{f(x,y)}+\pd{f(x,y)}{y}。
- 8. 新增更多颜色。
- 9. 有序/无序列表现在有了更明显的标志。
- 10. ！现在，玢辣支持texlive内核+VS Code编辑器的写作系统，！！！！附带支持**windows中文用户名的简易配置方式！！！！**：
- 使用https://zhuanlan.zhihu.com/p/166523064 的方法，但**不使用他的『windows中安装texlive时不支持中文用户名导致的乱码问题』的解决方案**。转而使用https://blog.csdn.net/weixin\_44397732/article/details/121025366 【若链接失效，在CSDN搜：一种用户名含有中文的texlive2021安装方案（win10）】 中的第1步-第3步解决『windows中安装texlive时不支持中文用户名导致的乱码问题』。强调：**一旦安装完成，必须按照第2个链接内附的办法撤回第1步和第2步的修改，否则将会导致其它许多软件出现网络上无法查询到的错误**。
- ---------------------------------------------------------------
- 2022/05/05更新1.2.8。
- 1. ！增加开源字体『heiti=思源黑体简体版』。因你站文件大小限制，请单独下载，其它文件都在zip包里。
- 2. ！拆分『玢辣fenla』为多个子包，尤其是核心功能数学编码和外观分离，显著优化『在需要使用其它模板的外观时使用fenla的体验』（但还未能完全分离，不久后才能实现『其它模板上加玢辣』），显著优化『每次写文前的复制粘贴的复杂度和逻辑』。
- 3. ！导数/微分/偏导数算符优化，使之和『积分』的逻辑和表现变得相对一致，并且更自然。比如$\jf f(x,y)\wf x$；$\jfjf f(x,y)\wf x$；$\ds f(x)$；$\pds f(x,y)$；$(\pds{y}) f(x,y)$；$\pds{y}^2 f(x,y)$；$\fen{\pwf f(x,y)}{\pwf x}$；$\fen{\pwf^2 f(x,y)}{(\pwf x)^2}$。wf即『正体d』，如果懒可以打普通体（在玢辣使用的字体里不会太斜）也就是d。如果不想这样整体认读，可以用\fen、\pwf之类手动打。为了与积分更一致，下次会做高阶导数和偏导数。
- 4. ！优化并重新规划了『zt字体、zh字号、ys颜色』word三大功能。他们都是『开关式』指令，即在最近一个环境或大括号之内全都有效，类似开关，一旦打开，若在本环境/大括号内无下次指令，则一直保持新的字体/字号/颜色。比如如果你想只增大这2个字，应打{\zh{1} 示例}。可和下一条对比。
- 5. ！优化并重新规划了『换笔』功能的内在哲学。为模仿实际写字，玢辣设计了换笔功能（hs换红色，zd换重点，zdzd/qd其它两个重点笔）。所有换笔均不是开关式的而是函数式的，比如你想标记2个字作为重点，应打\zd{示例}。可和上一条对比。每一个玢辣开放的颜色均设置成可以这样用的『换笔函数』，同时也支持以第4条的方式『开关』：比如为得到同样效果，应打{\ys{hs} 示例}。
- 6. 改进有序/无序列表视觉效果，增加相应接口并修复bug。
