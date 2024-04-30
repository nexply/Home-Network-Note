# ⭐️ 路由网关

${GATEWAY_NETWORK}

## 家用网络为什么需要交换机

因为性价比高，不论是性能，还是成本，亦或者是稳定性。

有没有想过为什么大家总是会说路由器的性能不够，网络体验卡顿，需要不断的更新换代呢？

抛开外部网络环境不提，单看内网场景下，除了一些希望在不额外添加设备的情况下，进行个性化需要：

- 用路由器运行一些软件做虚拟组网
- 用路由器运行一些软件做广告过滤
- 用路由器进行脱机下载
- 用路由器提供游戏加速

我们日常对路由器性能要求最高的莫过于：**接入设备**的包转发负载、以及无线网络接入和处理。如果这些功能集成在一台设备上，最终这台设备的价格会变的相对比较高，且可能出现某块短板在几年内随着科技的发展显的特别突出（落后）。

### 千兆网络环境举例

以 2021 年，两千元中高端路由设备[ASUS AX88U](https://www.asus.com/Networking-IoT-Servers/WiFi-Routers/ASUS-Gaming-Routers/RT-AX88U/techspec/)为例：

先计算有线状态下的性能（都按照线性无阻塞计算）：

- 因为设备算上WAN口共计 9 个全千兆端口（双工 2000Mbps），无线网络极限为 1148+4804 Mbps，则如果该设备支持所有连接设备将其带宽跑满，该设备极限背板带宽为24G不到。
- 而文档中提到的，我使用了许多年的交换机的面板属性是16个端口，32G背板带宽，五年前购入价格498元。

简单的结论是，我们可以通过一台相对廉价的交换机，获取至少五年以上的家用高端设备在有线数据交换上的体验，成本只有其四到五分之一。

然后，接着来看无线状态下的性能：

- AX88U 标称无线网络极限带宽 1148+4804 Mbps。
- 同年产品，小米 AX6000 无线路由器标称无线带宽为 6000 Mbps，整台设备价格599元

简单结论是，无线 AP 功能部分也可以使用一台相对廉价的设备进行替换，成本也只有其四到五分之一。

### 更换更高效的无线网络

如果我们使用 2023～2024 年的设备，比如我在使用的小米 BE6500 Pro，即使只使用路由的 Wi-Fi 7 路由功能，我们将能够让上面的设备增加 6500M 的无线带宽，支持 4x4 160MHz 大频宽，能够让多台设备同时更新软件的时候得到更快的体验。


## 其他

算到这里其实还没有结束，因为交换机并不具备宽带拨号/DHCP管理能力，我们还需要计算一台真正的路由器的成本。

不过庆幸的是，因为家用宽带的出口有限（普遍在 2G 内），所以我们随便购买或者使用运营商赠送的全千兆路由器，其实都够跑满外部带宽。

在上面无线 AP 和交换机的加持下，拨号路由器负载会异常的低，而相同软件状况下，低负载意味着你的设备可以无故障运行更长时间，以及做更多你想做的事情。

当然，使用单一设备也有好处，当你设备压力复杂没有那么大的时候，单一的设备，不论是从空间体积、设备发热、还是产品设计来看，会优于组合方案，至于到底选择哪种，就仁者见仁了。

我的设备一般运行时间会是半年到一年，偶尔小区断电或者我打扫机柜，会让它的计时器中断，在它在线的时间里，除非运营商故障，我的网络会一直比较通畅。

- [关联知乎问题：如何跟小白解释路由器和交换机的区别？并且家用路由器充当了路由器和交换机的功能吗？](https://www.zhihu.com/question/22007235/answer/2072616337)