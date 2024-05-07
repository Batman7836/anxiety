# intro

`SceneSetup.intro();`

# intro-play-button

(...51)

```
_.PLAYED_BEFORE = !!window.localStorage.continueChapter;
```

{{if !_.PLAYED_BEFORE}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if !_.PLAYED_BEFORE}}
[#play1# بازی کن! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act2"}}
[_CONTINUE_: پارتی](#act2) `publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act3"}}
[_CONTINUE_: اون یکی پارتی](#act3) `publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="act4"}}
[_CONTINUE_: اون یکی ساندویچ](#act4) `publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
`Game.OVERRIDE_FONT_SIZE=30;`
{{/if}}

{{if _.PLAYED_BEFORE && window.localStorage.continueChapter=="replay"}}
[#play1# دوباره بازی کن! #play2#](#intro-start) `publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if _.PLAYED_BEFORE}}
[انتخاب بخش](#chapter-select) `Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

[(نکات این محتوا)](#intro-play-button) `Game.OVERRIDE_CHOICE_LINE=true; publish('show_cn');`

# chapter-select

`publish("HACK_chselect");`

[1. ساندویچ](#intro-start) `publish("HACK_chselect_end"); publish("intro-to-game-1"); Game.OVERRIDE_CHOICE_LINE=true;`

[2. پارتی](#act2) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act2"]); Game.OVERRIDE_CHOICE_LINE=true;`

{{if window.localStorage.act3}}
[3. اون یکی پارتی](#act3) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act3"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act3}}
[3. اون یکی پارتی]()
{{/if}}

{{if window.localStorage.act4}}
[4. اون یکی ساندویچ](#act4) `publish("HACK_chselect_end"); publish("LOAD_GAME", ["act4"]); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.act4}}
[4. اون یکی ساندویچ]()
{{/if}}

{{if window.localStorage.credits}}
[5. تیتراژ](#to-credits) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`
{{/if}}

{{if !window.localStorage.credits}}
[5. تیتراژ]()
{{/if}}

[(منو اصلی)](#intro-play-button) `publish("HACK_chselect_end"); Game.OVERRIDE_CHOICE_LINE=true;`

# to-credits

`stopAllSounds();`

(...101)

(#credits)

# intro-start

(...500)

`clearText()`

n3: خوش اومدی! خیلی نمیشه اسم این رو یه "بازی" گذاشت، بیشتر مثل یه داستان تعاملی می‌مونه. پس امیدوارم از خوندن خوشت بیاد بیچاره!

n3: پس قبل از اینکه شروع کنیم، *تو* چطور دوست داری بخونی؟

`publish("show_options_bottom")`

# intro-start-2

n3: عالیه! یه نکته: تو همچنان میتونی تنظیمات رو با ایکون ⚙ پایین صفحه عوض کنی. همچنین، بازی هر قسمت رو بصورت اتوماتیک ذخیره می‌کنه!

n3: ...و حالا، بیا داستانمون رو شروع کنیم

`clearText()`

(...1000)

`publish("intro-to-game-2")`

n2: این یه انسانه

(...600)

`clearText()`

(...300)

`publish("intro-to-game-3")`
