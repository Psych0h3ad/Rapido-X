# Validation records / 計算の検証記録

These files document the exploratory runs described in the [report](../README.md). They do not validate real-world cooling performance. The specified flow residual target was not reached, and each mesh has one high-skewness warning.

このフォルダーには[比較資料](../README.md)の試験的な計算記録を掲載しています。実機性能を保証するものではありません。設定した流れの残差目標は未達で、各メッシュに高skewness面の警告が1件あります。

- `*-thermal-audit.csv`: patch areas, volume flow and heat balance for all six runs / 6条件の面積・流量・熱収支。
- `*-thermal-convergence.log`: additional scalar convergence on the frozen flow / 流れを固定した温度場の追加収束。
- `*-flow.log`: 25 Pa baseline flow and scalar iteration records / 25 Paの基準計算記録。
- `*-mesh-check.log`: mesh checks, including the remaining warning / 未解消の警告を含むメッシュ検査。
- `geometry-repair.json` and `hotend-repair-location.json`: sampled geometry repair checks / メッシュ修復のサンプル比較。

In the logs, only the machine hostname and local workspace path were replaced with `REDACTED_HOST` and `<CFD_WORKSPACE>`. Numerical solver output has not been changed.

ログ内の計算機名とローカル作業パスのみ、それぞれ `REDACTED_HOST` と `<CFD_WORKSPACE>` に置き換えています。計算値は変更していません。
