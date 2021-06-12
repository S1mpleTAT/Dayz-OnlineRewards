🎉 免费的Dayz模组，可以根据每个玩家的在线时间给予银行存款奖励；[@Time Is Money](https://steamcommunity.com/sharedfiles/filedetails/?id=2045438856&searchtext=Time+Is+Money) 的升级版。

## 特别说明：
#### 需要的额外模组：[@CF](https://steamcommunity.com/sharedfiles/filedetails/?id=1559212036) & [@Banking](https://steamcommunity.com/sharedfiles/filedetails/?id=1836257061)
#### 这个模组不是： -servermod ！！！

## 模组安装：
  :video_camera: [查看视频](https://www.bilibili.com/video/BV1qy4y1u7hr)

## 重点功能：
#### 显示/隐藏 主菜单按键： T(默认按钮，可以在游戏设置里修改)
#### 领奖：
        服务器： 单独设置每个玩家的：奖励间隔、存款奖励数量、领取存款的次数 (玩家与玩家之间的设置不会互相影响)
        玩家端： 在线时间达到要求时会弹窗提醒, 玩家需要打开主菜单 然后手动领取奖励。
#### 转账：
        服务器：
            模组配置文件里设置：
                开/关 转账功能 和 转账需要的手续费 (百分比，最多95)

            转账费用的计算公式：转账金额 * (手续费 * 0.01) + 转账金额
                如果:  手续费: 5%，转账金额: 100
                例子1:
                    发起玩家拥有余额：110
                    实际扣除金额 = 100 * (5 * 0.01) + 100  也就是：105
                    那么：
                      发起玩家剩下余额 = 110 - 105  也就是：5
                      目标玩家拥有余额 += 100

                例子2:
                    发起玩家拥有余额：100
                    因为 发起玩家拥有余额 <= 转账金额
                    所以 实际扣除金额 = 转账金额  也就是：100
                         目标玩家获得 = 转账金额 - (转账金额 * (5 * 0.01))  
                             也就是： 100 - ( 100 * (5 * 0.01) ) = 95
                         目标玩家拥有余额 += 95

        玩家端:
            双方玩家都必须拥有 @Banking 的相关配置文件 ( 路径: DayZServer\Profiles\xxxx\DC_Banking\PlayerDatabase\玩家ID.json )
            转账金额必须 >= 100 (并且是100的倍数)
            发起玩家的余额必须 >= 转账金额。
            转账扣除的手续费由发起玩家支付。
            目标玩家的游戏状态即使是离线也能转账给他。

## [[服务器]配置文件](https://github.com/S1mpleTAT/Dayz-OnlineRewards/tree/chinese/%E9%85%8D%E7%BD%AE%E6%96%87%E4%BB%B6)