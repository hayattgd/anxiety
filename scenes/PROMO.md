# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[プレイ!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: 始める前に、*あなた*好みの表示設定ができます。

`publish("show_options_bottom")`

# intro-start-2

n3: それでは、わたしたちの物語を始めましょう...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: これは にんげん

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`

# act1

```
SceneSetup.act1();
publish("hide_tabs");
music('battle', {volume:0.5});
```

(...300)

n: これは にんげんの ふあん

n: _あなた_ は ふあん

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: いやだ。やだ、やだ、聴かないよ。スマホ見るからね。

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: あなたの 仕事は あなたのにんげんを *危険* から守ること

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: はっ! またツイッターで人生をスクロールしてる!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: ああ どうしてわたしについての感想をちゃんとただ座って聞かないんだろうね

`hong({eyes:"neutral"});`

n: *危険* について素早く警告しましょう!

```
bb({eyes:"look"});
```

[なんてこった、その恐ろしいニュースを見なよ!](#act1d_news)

[なんてこった、そのツイートは *ぼくら* のことじゃないか?](#act1d_subtweet)

[あ、ネコがミルクを飲むGIF動画だ](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: うん かわいい、わたし--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: ネコはミルクでお腹を壊すのに ぼくらは動物虐待を楽しむひどい人間だ

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



