# launchd
- 簡単に言えばcronみたいなもの
- OSXで定期実行させたいスクリプトをXMLで書いていく

# 使い方

- `~/Library/LaunchAgents`にplistファイルを置いて
```
launchctl load ~/Library/LaunchAgents/....plist
```
- ファイルに変更があった場合は以下のようにunloadしてからloadし直す
```
launchctl unload ~/Library/LaunchAgents/....plist
```
