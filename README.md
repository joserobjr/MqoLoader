# MqoLoader
Mqo (3D model) loader for Minecraft Mod

MOD開発者向けのマインクラフトでMQO(メタセコイア形式のモデル)を読み込み、描画するコードです。  
[MCヘリコプターMOD](http://forum.minecraftuser.jp/viewtopic.php?f=13&t=14837 "") からモデルの読み込み機能だけ抜き出しました。


modeltest 配下  
　modelloader を扱うサンプルコード  
modelloader 配下  
　モデルの読み込みと描画を行う  

* マテリアルには非対応
* スムージングに対応
* メタセコイア内のオブジェクトの親子関係は読み込まない
* オブジェクト名の頭に $ を付けると親扱いとなり、  
$ がついていないオブジェクトを子として描画する
* メタセコイア内の 100.0 はマインクラフト内で 1.0 (1ブロック)となる
* 三角形または四角形のみ読み込む(四角形は読み込み時に三角形2つとして扱う)
* 指定した範囲の番号の面または線を描画することができる  
→MCヘリコプターMOD の製図台で機体を描画するのに使用している
