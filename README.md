# solenoid-valve
[こちら](https://github.com/funi007/solenoid-valve.git)の電磁弁基板の改良版です。未テストですので使用に際しては十分注意してください。

# 履歴
## 改良基板の初版
- 2023/11/03
- ERC and DRC check
- 6f543627d558cafed8350256de44e78604443efa
- 改良基板の初期版。未テスト。

# 改良点
## フォトリレーが焼ける問題を解消
フォトリレーに負電圧がかかることで内部のFETが焼ける問題を解消しました。フォトリレー自体を採用せず、FETによるオープンドレイン出力としました。

## XT30コネクタに変更
駆動用電源のコネクタをEPコネクタからXT30コネクタ(オス)に変更しました。

## DCDCコンバータの安定性・効率を向上
DCDCコンバータに適正な負荷をかけ、連続モードでの動作とすることで、DCDCコンバータの安定性を改善ました。また、効率の上昇や高調波ノイズの低減も期待できます。

## フォトカプラへの配線を改善
ベタパターンの島ができにくいように、フォトカプラへの配線をまとめました。

# 問題点