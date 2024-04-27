## Unityで制作する方へ
アプリ名をmain.exeとするためには、ビルド設定>プレイヤー設定>ProductName を「main」とする必要がありますが、ウインドウのタイトルが「main」となってしまいます。<br>
タイトル名を変更したい場合は、ゲーム2024\制作補助ツール\Unity\TitleChange.csの以下の部分をお好みで書き換えたうえで、そのスクリプトを任意のオブジェクト（MainCameraなど、常時オンになっているものが好ましい）にアタッチしてお使いください。<br>
Mac/Linux版ではこの作業は不要です。（WinAPIを使用しているため、）<br>
>SetWindowText(windowPtr, "MonitorManShooting");<br>
の"MonitorManShooting"の部分<br>
（参考:https://qiita.com/broken55/items/5a2faca1a039f47e43f0 ）
