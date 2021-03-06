# 线材、调音台与效果总线

平衡/非平衡线缆

## 调音台的架构

调音台最基本的作用都是接入多个外部乐器并提供调整每种乐器音色的界面。
这些信号在调音台内被混合后送给监听音箱和录音机并输出最终的混音。

- 通道条
- 增益控制旋钮(Trim/Gain)
- "Pad"(衰减)按钮
- 幻象供电(pantom Power)开关、浮地(Ground Lift)开关以及反相(Phase Reverse)开关
- 哑音(Mute)开关
- 插入总线(Insert Bus)
- 推子前(Pre-Fader)母线
- 辅助(Aux)母线
- 音量推子(衰减器Fader)
- 声像(Pan)母线
- 编组(Subgroup)母线
- 主推子

## 连接效果器和处理器

所有的效果器都包含干湿比(Dry/Wet)参数("湿"是指加了效果的信号，"干"则代表原始信号)，用来调整原始信号与效果信号的比例，混响就是很好的例子。

## 辅助总线

基本上所有的调音台的辅助总线都在均衡之后，这是因为一般认为辅助效果器的添加是混音的最后一道工序。

辅助总线需要两条独立地信号线。其中一条负责将调音台的信号引入效果器，而另一条将效果返回给调音台。

混音更倾向使用推子后发送。使用推子后发送，当衰减通道推子时也会同时减少辅助发送量，从而免去了每次改变音量都要再次调整辅助发送电平的烦恼。

## 插入总线

与辅助总线不同，插入总线位于均衡前，它的设计更适合处理器而不是效果器。
这是因为处理器需要完整的信号，而且也没有理由只让压缩或噪声门仅处理信号的一部分。

### 门 > 压缩 > 均衡 > 效果器

### 门 > 压缩 > 效果器 > 均衡

前半部分保持信号的自然，而降均衡放在效果器之后是为了用它来修饰效果器产生的音色。

### 门 > 压缩 > 均衡 > 效果器 > 效果器

失真、混响、镶边等效果的排列组合

### 门 > 效果器 > 均衡 > 效果器 > 压缩

在第一个效果器之后放入均衡，可以调整音色成分，避免不需要的频率进入下一个效果器使声音浑浊

此外，在尾端放上压缩器，任何镶边、失真或类似效果带来的峰值都可以受到控制。

### 压缩 > 均衡 > 效果器 > 门

在这种排列中，压缩器用来在均衡和效果之前控制音色的动态。
但是，减噪声门放在效果器之后意味着门效果的使用。

在常用的技术是在低鼓或Trance/Techno/House的主奏音色上加混响，然后再用后面的门去掉混响音尾。
这种效果能加厚声音，而不会让音相互叠加导致浑浊。

### 门 > 效果器 > 压缩 > 均衡

尽管压缩通常都是在效果之前，但是这样也是有它的道理的。
比如，如果使用滤波效果来提升某些频率并通过合唱或镶边，就很有可能出现过载，因此需要在用均衡调整音色之前压缩控制电平。

效果器的顺序并没有定律，最好的效果往往来自于实践。

## 自动化

调音台上最后一个重要部分是自动化混音。

随着音乐的进行改变音色。在音序器里录制好参数改变数据，在回放时调音台会根据新的设置而变化。

混音自动化有两种形式： VCA 和马达推子。