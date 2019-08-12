# 開発方針

１．最低でも画面とサーバで分けておく。  
　　FEとBFF＋BEのようなイメージ。  
　　FE＋BFF＋BEで作成してもOK。

２．Controller、Service、Infrastructureで構成する。  
　　ControllerはServiceに、ServiceはInfrastructureに依存する。逆は不可。

３．Voを作成すること。  
　　equals, hasCode, toStringメソッドを作成する。  
　　ofというメソッド名でprivateかつstaticなfactoryメソッドを作成すること。