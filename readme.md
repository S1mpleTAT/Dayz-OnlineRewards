【Because my english very bad, can only use Google Translate...

Some words may be wrong (please forgive me)】


### 🎉 Free DayZ mods, [@Time Is Money](https://steamcommunity.com/sharedfiles/filedetails/?id=2045438856&searchtext=Time+Is+Money) updated version.
##### Each player can be rewarded with bank deposits based on the amount of time they spend online;

## Special Version:
##### Additional mods required: [@CF](https://steamcommunity.com/sharedfiles/filedetails/?id=1559212036) & [@Banking](https://steamcommunity.com/sharedfiles/filedetails/?id=1836257061)
##### This mods is not: -servermod !!!

## Main Function:
#### Show/Hide Menu Keys： T(Default button, can be changed in game settings)
#### Online Reward:
        Server:
            Set for each player: reward interval, reward quantity, reward times
        Client:
            Reminder pops up when your online time is met, open the main menu to receive rewards.
#### Transfer:
        Server:
            Settings in mods profile file:
                Transfer switch
                Transfer tax (percentage, max 95)

            Transfer tax calculation formula = Transfer amount * (Tax * 0.01) + Transfer amount

        Client:
            Both players must have the relevant @Banking profile (path: DayZServer\Profiles\xxxx\DC_Banking\PlayerDatabase\PlayerID.json)
            Transfer amount must be >= 100 (multiple of 100)
            Transfer player currency must be >= transfer amount.
            Transfer tax is paid by the transfer player.
            Beneficial players can get transfer amount even if they are offline.

## [[Server]profile](https://github.com/S1mpleTAT/Dayz-OnlineRewards/tree/english/Profile)