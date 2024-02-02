<h1 align='center'>兰博电竞幻兽帕鲁MOD服务器基础文件</h1>
<p align='center'> 
  仅支持基于 Windows Server 2019 及以上的 x64 服务器。
</p>

> 由于原始的服务器注入器放入其它文件夹会被服务端更新校验覆盖掉，所以放在根目录中避免被校验覆盖。

功能：

- [x] 初始化的服务端 UE4SS 配置
- [x] 同步 VeroFess 的 UE4SS 服务端 API https://github.com/VeroFess/PalWorld-Server-Unoffical-Api
- [x] 基于 xmake 和非内存注入方式的服务端注入器
- [x] 放入 memreduct 用来降低不必要的内存消耗
- [ ] 其它功能...

## 部署 sav-agent
由于与兰博电竞业务不同，需要部署 https://github.com/zaigie/palworld-server-tool 来进行游戏内存档解析
save-agent 将开启一个端口，游戏内的存档可以在其它机器上解析 **非常重要，因为超过100玩家角色建立后游戏存档可能大于20M，解压后大于2G**
在一些情况下你可能不想要它们部署在游戏服务端的机器上：

- 需要单独部署在其它服务器
- 只需要部署在本地个人电脑
- 游戏服务器性能较弱不满足，采用上述两种方案之一

## 许可证

根据 [Apache2.0 许可证](LICENSE) 授权，任何转载请在 README 和文件部分标明！任何商用行为请务必告知！
