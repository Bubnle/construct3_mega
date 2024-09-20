# construct3_mega

## 目录
- 1.[游戏背景](#游戏背景)
- 2.[游戏在线编程工具](#游戏在线编程工具)
- 3.[游戏实现步骤](#游戏实现步骤)
- 4.[游戏可拓展的思路](#游戏可拓展的思路)
- 5.[游戏demo展示链接](#游戏demo展示链接)

## 1.游戏背景
<a name="游戏背景"></a>
在荒废的邪恶古堡深处，阴冷的空气中弥漫着死亡的气息。哥布林群在黯淡的火把下，准备着他们的下一次阴谋。然而，一位神秘的法师悄然出现在古堡的长廊尽头，斗篷在微风中轻轻飘扬，手中的法杖闪烁着炽热的火焰。他低声念诵着古老的咒语，脚下的石砖仿佛在他的力量下微微震动。古堡的天空乌云密布，雷声隐隐。哥布林们感受到一股危险的气息，发出尖锐的叫声，挥舞着生锈的武器冲向法师。
就在这一刻，法师果断挥动法杖，一颗巨大的火球从天而降，划破夜空，狠狠砸向最前方的敌人。炽热的火焰瞬间吞噬了冲锋的哥布林，烧灼的气浪席卷整个大厅。剩余的哥布林惊慌失措，四散而逃，但他们的退路早已被封锁。随着法师最后一句咒语的落下，火光渐熄，邪恶的古堡再次陷入了寂静。

## 2.游戏在线编程工具
<a name="游戏在线编程工具"></a>
https://www.construct.net/

## 3.游戏实现步骤
<a name="游戏实现步骤"></a>
### 1) 新建项目
点击页面的新建项目，开始创建！

![start]()

接下来出现设置具体的场景属性设置，我们不对预设尺寸等属性进行更改。

![start]()

### 2) 添加对象
#### i.添加游戏的背景
为了契合游戏的背景选择了以像素风的石砖作为背景。
<div align="center">
    <img src="images/ground.webp" alt="游戏截图" />
</div>

具体操作就是双击布局来创建，选择常规中的平铺图

<div> </div>

接下来就是将这个石砖铺满整个布局，于是点击在布局中对应的图像，在右侧的属性栏中更改坐标和大小
我们改为（0，0）坐标和 1921x1084 的大小使得铺满整个页面

<div> </div>

#### ii.添加其他对象

- 1.法师（玩家）
  <div align="center">
    <img src="images/wizard.webp" alt="游戏截图" />
</div>
- 2.哥布林
  <div align="center">
    <img src="images/goblin.webp" alt="游戏截图" />
</div>
- 3.火球
  <div align="center">
    <img src="images/spell.webp" alt="游戏截图" />
</div>
- 4.闪耀特效
  <div align="center">
    <img src="images/spark-flash.webp" alt="游戏截图" />
</div>
添加方法和上面类似双击布局，选择常规中的精灵模块进行添加，注意不同的对象应该有不同的名字。
<div></div>

### 3)添加行为
需要对添加的对象进行行为的添加~
8方向移动：这允许您使用方向键移动对象。这对玩家的移动有好处。
子弹移动：使对象以当前角度向前移动。适用于哥布林，和火球的移动方式。
镜头跟随：使屏幕在对象移动时跟随对象移动。
绑定到布局：这将阻止对象离开布局区域。这对玩家也很有用，这样他们就不能在游戏区域外徘徊了！
出界销毁：这不是阻止对象离开布局区域，而是销毁它。离开布局后会销毁它们。
淡入淡出：使对象淡出，我们将在火花闪烁时使用

如何添加行为？
<div></div>
选择上面提到的行为对不同的对象进行添加！
<div></div>

### 4)创建更多的哥布林对象
为了保证游戏的合理性,以及具有一定的挑战性

## 4.游戏可拓展的思路
<a name="游戏可拓展的思路"></a>

## 5.游戏demo展示链接
<a name="游戏demo展示链接"></a>
