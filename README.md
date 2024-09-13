# Emoji4JE
絵文字を使えるようにするリソースパックのテンプレートと作り方  
[もっと詳しく知りたければここ](https://minecraft.fandom.com/ja/wiki/フォントのカスタマイズ)  

## assets/minecraft/textures/font/emoji/
ここに72x72の解像度でアイコン画像を作って配置する。

## assets/minecraft/font/default.json
```json
{
  "providers": [
    {
      "type": "bitmap",
      "file": "minecraft:font/emoji/1f004.png",
      "ascent": 8,
      "height": 8,
      "chars": ["\uD83C\uDC04"]
    }
  ]
}
```
テンプレートのZipの中身の絵文字があまりにも多すぎるから、使う個数だけ絞っていらないやつ消すと思うんだけど、その時定義しているJson部分もしっかり消してあげないといけない。  
例えば上のdefault.jsonに書かれた一個の絵文字だけを入れたいときは、ちゃんとそれ以外の画像ファイルも消す。
