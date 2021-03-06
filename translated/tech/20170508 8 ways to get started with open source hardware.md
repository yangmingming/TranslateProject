8 种方式开始使用开源硬件
============================================================

### 制造自己的硬件比以往任何时候都更容易，更便宜。以下是你需要设计，构建和测试你的第一块电路板。


![8 ways to get started with open source hardware](https://opensource.com/sites/default/files/styles/image-full-size/public/images/life/hardware_hammer_sign.jpg?itok=vh76LBib "8 ways to get started with open source hardware")
>图片提供： Thomas Hawk on [Flickr][11]. [CC BY-NC 2.0][12]. 由 Opensource.com 修改

著名的计算机科学家 Alan Kay 曾经说过：“认真对待软件的人应该制造它们自己的硬件。” 我认为今天就如 1982 年他所说的一样真实。然而，现在和那时之间的变化是硬件变得越来越快，越来越小，最重要的是：更便宜。 现在可以用 5 美元购买一台完整的电脑。

随着大公司降低自己产品的价格，它发展了一个能够生产生产级硬件的制造业生态系统，它的成本足够便宜，并且达到了普通人都可以接受的程度。这种可用性以及可负担性正在帮助推动诸如众筹和制造商运动之类的事情，但他们也让更多的个人能够通过开源硬件参与开源。

探索开放硬件

*   [什么是开放硬件？][1]

*   [什么是树莓派？][2] 

*   [什么是 Arduino？][3]

*   [我们最新的开放硬件文章][4]

什么是或者不是开源硬件有很多区别，但是开源硬件联盟（OSHWA）定义了一个大多数人同意的定义，如果你熟悉开源软件，这不会听上去太奇怪：


> “开源硬件（OSHW）是有形人工机器、设备或者其他物理东西的术语-其设计像公众发布，任何人可以制造、修改、分发并使用那些。”

周围已经有很多开源硬件了。你可能没有注意到你在使用的主板可能实际上是开放的硬件。从[低调]但通用的[Arduino][13]，一直到像 [BeagleBone][14] family 和 [C.H.I.P.][15] 计算机这样的完整功能的电脑，这有很多开放硬件的例子，还有更多的在设计中。

硬件可能很复杂，对初学者而言为什么设计需要这些有时不太明显。但开源硬件使你不仅可以看到工作示例，还可以更改这些设计，或者在你自己的设计中复制所需的部分，就如复制和粘贴一样简单。

### 我该如何开始？

我们先要指出硬件很难，它很复杂，有时是深奥的，你可能用到的工具并不总是最人性化的。任何一个玩微处理器的时间足够长的人都可以证明有一种可能：你会烧坏一些东西，看到神奇的烟雾在某个时刻冒出来。没关系，我们都做过，有些人还会反复做，因为我们在做一件事情的前 100 次时都不会得到教训，但不让让这阻碍你：当做错事情时，你会学到教训，而且你将来还会有有趣的故事告诉别人。

### 建模

首先要做的是开始使用现有的电路板，跳线、面包板以及你要连接的任何设备来建模你想要做的事情。在许多情况下，最简单的事情就是在板上添加更多的 LED，并以新颖的方式让它们闪烁。这是一个很好的出原型的方式，也是一个很常见的事情。它看上去不漂亮，你可能会发现你的线接错了，但这些都是原型 - 你只是想证明硬件可以工作。当硬件不工作时，一定要仔细检查一切，不要害怕寻求帮助 - 有时第二双眼睛会发现你奇怪的接地短路。

### 设计

当你弄清楚你想要构建的硬件，现在是时候把你的想法从跳线和面包板变成实际的设计了。这时事情会变得让人气馁，但是从小的开始，事情上，可以从熟悉加工和流程这样非常小的开始，所以为什么不制作一块带有 LED 和电池的印刷电路板？认真地说，这可能听起来过于简单，但在这里有很多新的基础要了解。

1.  **找到一个电子设计自动化（EDA）工具来使用。** 这有很多好的开源软件可以选择，但是它们并不总是用户友好的。[Fritzing][5]、[gEDA][6] 还有 [KiCad ][7] 都是开源的，并以可用性升序排序。如果你想要尝试更多的商业软件，那么还有一些其他的选择。Eagle 有受限的免费版本使用，有许多的开源硬件是用它设计的。

2.  **在 EDA 工具中设计你的电路板。** 依据你选择的工具，这可能会非常快，或者可能是学习如何设计的很好的练习。这是我建议从小的硬件开始的原因之一。一个带 LDED 的电路可以如一块电池、一个电阻、一个 LED 一样简单。电路图非常简单，并且布局也会非常小、非常简单。

3.  **为制造导出设计。** 这与列表中的下一件事情紧密相连，但如果你以前没有这样做，这也可能是一个令人困惑的过程。当你在导出时，你会有很多细节需要调整，并且需要以某种方式导出以便电路板工厂能确切知道你要做的。

4.  **找到一个电路板工厂。** 有许多电路板工厂可以制作你的设计，并且一些比其他更加友好及有帮助。一个特别棒的地方是 [OSH Park][8]，这些人非常友好并支持开源硬件。他们也有一个非常扎实的流程来确认你发送给它的就是会被制造的，所以他们值得一试。还有很多其他选择; 看看 [PCB Shopper][9]，它可以让你比较不同实体 PCB 商家的价格、周转时间等等。

5.  **等待。** 这或许是在制造你自己的电路板中最难的一部分了，因为它会花费时间将数字部分变成物理产品。计划好两周时间来拿到你的电路板。这是你继续下个项目的绝好时间，确保或获取你当前制造的所有部分，或者通常上尝试不要担心。你的第一块电路板是艰难的 - 你现在非常想要，但是保持耐心。

6.  **修补并提升。** 一旦拿到你的板子，是时候上电测试了。如果你是以 LED 电路开始，那么它很容易调试，并且你会得到一些可以工作的东西。如果你有更复杂的电路，那么需要有条理并且有耐心。有时候电路不会工作，并且你需要用你的调试技能来追踪问题。

7.  **最后，如果你做的是开源硬件，那就发布它。*** 我们谈论的是开源硬件，因此确保包含了一个许可，但是发布它、共享它，把它放在人们可以看见你所做的地方。你或许会想写一篇博客并提交到如 Hackaday 上面。

8.  **最重要的是，玩得开心。** 坦白说，如果你在说一些事但是你不开心，你应该停止这样做。开源硬件可以很有趣，虽然有时是困难而且复杂的。但是不是一切都会正常。见鬼，我已经设计了一半的电路不工作，或者我（意外地）在电源和接地之间造成了 12 次短路。这些电路板是双层板：是的。我在这个过程中学到了一些东西：非常多，并且我不会再犯同样的错误。我会做出新的板子，但不是这些。（我会支持并盯着这些板子和它们的错误，悲伤的是，它们不会在我盯着它们时感到难受）。

build the hardware that they want—not the hardware they can get.
现在有许多的开源硬件，以及从中可以查看、复制、衍生，并且有很多信息使制造硬件变得简单。这就是开源硬件：一个社区的人们制造它们，共享它们，这样每个人可以制作他们自己的东西并构建他们想要的硬件 - 而不是他们可以得到的硬件。

--------------------------------------------------------------------------------



作者简介：

John 'Warthog9' Hawley - John 在 VMWare 的开源项目办公室为上游开源项目工作。在以前的生活中，他曾在 MinnowBoard 开源硬件项目上工作，领导了 kernel.org 上的系统管理团队，并在桌面集群变得很酷之前构建了它们。为了乐趣，他构建了多个明星项目，一个受欢迎的英国电视节目 K-9 的复制品，在无人机的飞行计算机视觉处理中完成，设计并制作了一堆自己的硬件。

-------------------------------------

via: https://opensource.com/article/17/5/8-ways-get-started-open-source-hardware

作者：[John 'Warthog9' Hawley ][a]
译者：[geekpi](https://github.com/geekpi)
校对：[校对者ID](https://github.com/校对者ID)

本文由 [LCTT](https://github.com/LCTT/TranslateProject) 原创编译，[Linux中国](https://linux.cn/) 荣誉推出

[a]:https://opensource.com/article/17/5/8-ways-get-started-open-source-hardware
[1]:https://opensource.com/resources/what-open-hardware?src=open_hardware_resources_menu
[2]:https://opensource.com/resources/what-raspberry-pi?src=open_hardware_resources_menu
[3]:https://opensource.com/resources/what-arduino?src=open_hardware_resources_menu
[4]:https://opensource.com/tags/hardware?src=open_hardware_resources_menu
[5]:http://fritzing.org/home/
[6]:http://www.geda-project.org/
[7]:http://kicad-pcb.org/
[8]:https://oshpark.com/
[9]:http://pcbshopper.com/
[10]:https://opensource.com/article/17/5/8-ways-get-started-open-source-hardware?rate=jPBGDIa2vBXW6kb837X8JWdjI2V47hZ4KecI8-GJBjQ
[11]:https://www.flickr.com/photos/thomashawk/3048157616/in/photolist-5DmB4E-BzrZ4-5aUXCN-nvBWYa-qbkwAq-fEFeDm-fuZxgC-dufA8D-oi8Npd-b6FiBp-7ChGA3-aSn7xK-7NXMyh-a9bQQr-5NG9W7-agCY7E-4QD9zm-7HLTtj-4uCiHy-bYUUtG
[12]:https://creativecommons.org/licenses/by-nc/2.0/
[13]:https://opensource.com/node/20751
[14]:https://opensource.com/node/35211
[15]:https://opensource.com/node/24891
[16]:https://opensource.com/user/130046/feed
[17]:https://opensource.com/users/warthog9
