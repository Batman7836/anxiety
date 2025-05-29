# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

[PLAY!](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

# intro-start

(...500)

`clearText()`

n3: قبل از اینکه شرع کنیم، *تو* چطور میخوای بخونی؟

`publish("show_options_bottom")`

# intro-start-2

n3: حالا، بیا داستانمون رو شروع کنیم...

```
publish("hide_tabs");
clearText();
```

(...1000)

`publish("intro-to-game-2")`

n2: این یه آدمیزاده

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

n: و اینم اضطرابه آدمیزاده

n: _تو_ اضطرابشی

(#act1_normal)


# act1_normal

```
hong({body:"putaway"});
sfx("rustle");
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: نه. نه نه گوش نمیدم دام گوشیمو چک میکنم.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: وظیفه تو حفاظت از آدمت دربرابر *خطره.*

`bb({eyes:"look", mouth:"small_lock", body:"fear"})`

b: وای! بازم داری زندگیت رو با توییتر نگاه کردن حدر میدی!

```
bb({eyes:"normal", mouth:"normal", body:"normal"});
hong({eyes:"annoyed"});
```

h: آره نمیدونم چرا بیشتر نمیشینم به فکرام گوش بدم.

`hong({eyes:"neutral"});`

n: سریغ، بهش درباره یه *خطر* هشدار بده!

```
bb({eyes:"look"});
```

[وای نه، نگا چه خبر ناراحت کننده ای!](#act1d_news)

[وای نه، نکنه اون توییت درواقع درباره *ماست*؟](#act1d_subtweet)

[عه، این گربه رو ببین چه ناز شیر میخوره](#act1d_milk)

# act1d_milk

`hong({mouth:"smile", eyes:"surprise"});`

h: هه آره چقد نازه، من--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: گربه ها نمیتونن شیر رو هضم کنن و ما آدم های آشغالی هستیم که از حیوان آزاری حمایت می‌کنیم!

(...200)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("20p", "bad");
publish("hp_show");
```



