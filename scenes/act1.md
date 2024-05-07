# act1

```
SceneSetup.act1();
```

(...300)

n:  و اینم اضطراب انسانه

n: _تو_ اضطرابش هستی

{{if window.localStorage.continueChapter=="replay"}}
(#act1_replay)
{{/if}}

{{if window.localStorage.continueChapter!="replay"}}
(#act1_normal)
{{/if}}



# act1_replay

`hong({mouth:"0_neutral", eyes:"0_neutral"})`

h: اوه سلام! دوباره برگشتیم اینجا؟

`hong({eyes:"0_neutral"})`

n: وظیفه تو حفاظت از انسانت دربرابر *خطر* هستش

`bb({eyes:"look", mouth:"small_lock"})`

n: درواقع، دوباره بازی کردن این بازی همین الان اون رو در معرض *خطر* قرار میده

n: سریع، بهش هشدار بده!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: انسان! گوش بده، ما درخطریم! این بازیکن...

[قراره دوباره آزارمون بده...](#act1_replay_torture)

[قرار نیست یه پایان متفاوت پیدا کنه...](#act1_replay_alternate)

[دچار ناهماهنگی روایی میشه...](#act1_replay_dissonance)

# act1_replay_torture

```
window.HACK_REPLAY = JSON.parse(localStorage.act4);
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

{{if window.HACK_REPLAY.act1_ending=="fight"}}
b: They'll make us curl up into a ball and cry!
{{/if}}

{{if window.HACK_REPLAY.act1_ending=="flight"}}
b: They'll make us kill your phone for giving you a panic attack!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="fight"}}
b: They'll make us *NOT* punch the party host!
{{/if}}

{{if window.HACK_REPLAY.a2_ending=="flight"}}
b: They'll make us punch the Sympathetic Anti-Villain party host!
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="jump"}}
h: Well at least we might not jump off the roof this ti--
{{/if}}

{{if window.HACK_REPLAY.a3_ending=="walkaway"}}
b: THEY'LL MAKE US JUMP OFF THE ROOF.
{{/if}}

`bb({body:"fear"});`

b: تمام این بلا ها سرمون میاد، و بعد ما--

(#act1_replay_end)


#act1_replay_alternate

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: البته، *کلیت* داستان همونه، اما هر قسمت دوتا پایان ممکن داره، بعلاوه شاخه های مختلف هر دیالوگ--

`bb({body:"fear"});`

b: بازیکن ناامید میشه، ای صفحه رو می‌بنده، نرم افزارمون ور پاک میکنه، بعد ما--

(#act1_replay_end)


# act1_replay_dissonance

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich"});
```

h: ناهماهنگی چی؟

`bb({eyes:"normal"});`

b: قوس داستانی درباره این بود که چطور میتونیم *انتخاب* کنیم که رابطه سالمی با ترسمون داسته باشیم

`bb({eyes:"normal_right"});`

b: اما دوباره بازی کردن همون داستان رو بهمون میده، انگار *انتخاب‌ها* مهم نبودن،
`bb({eyes:"narrow_eyebrow"});`

b: بنابراین تضاد بین پیام و ساز‌وکار این بازی رو نشون می‌ده،

`bb({eyes:"fear"});`

b:  از این رو تار و پوداین جهان داستانی رو از هم باز می‌کنه،

`bb({body:"fear"});`

b: و بعد ما--

(#act1_replay_end)


# act1_replay_end

`bb({body:"panic"})`

b: می‌میرییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.clearText();
```

(...1001)

```
bb({body:"laugh"});
hong({body:"laugh"});
Game.clearText();
sfx("laugh");
```

(...5001)

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({body:"0_sammich"});
```

h: اوکی حالا بیا برگردیم به داستان.

```
Game.clearText();
```

n4: (LET _YOUR_ ANXIETY BLAH BLAH BLAH MOST SIMILAR TO WHAT _YOUR_ FEAR BLAH BLAH YOU KNOW THE DRILL)

```
sfx("squeak");
hong({body:"0_squeeze"});
bb({body:"squeeze"});
```

(#act1_normal_choice)



# act1_normal

`hong({mouth:"0_neutral", eyes:"0_annoyed"})`

h: اوه چه خوب، گرگم برگشته. خیلی هم عالییی.

`hong({eyes:"0_neutral"})`

n: وظیفه تو حفاظت از انسانت دربرابر *خطر* هستش

`bb({eyes:"look", mouth:"small_lock"})`

n: درواقع، اون ساندویچ داره همین الان در معرض *خطر* قرارش میده

n: سریع، بهش هشدار بده!

```
sfx("squeak");
bb({body:"squeeze_talk"});
hong({body:"0_squeeze"});
```

b: انسان! گوش بده، ما در خطریم! خطر اینه که...

`bb({body:"squeeze"})`

n4: )بذار اضطراب  _خودت_ وارد عمل بشه! گزینه ای رو انتخاب کن که به ترس _خودت_ نزدیکتره( 

(#act1_normal_choice)

# act1_normal_choice

[ما داریم تنهایی نهار می‌خوریم! دوباره!](#act1a_alone) `bb({body:"squeeze_talk"})`

[ما موقع غذا خوردن مفید نیستیم!](#act1a_productive) `bb({body:"squeeze_talk"})`

[اون نون سفید برامون بده!](#act1a_bread) `bb({body:"squeeze_talk"})`

# act1a_alone

```
bb({body:"normal", mouth:"small", eyes:"narrow"});
hong({body:"0_sammich"});
```

b: میدونی تنهایی به اندازه کشیدن 15 سیگار در روز روی مرگ های زودهنگام تاثیر داره؟

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({mouth:"normal", eyes:"normal_right"})`

b: (Holt-Lunstad 2010, PLoS Medicine)

`hong({eyes:"0_annoyed"})`

h: ام، مرسی که منابعت رو ذکر کردی اما--

`Game.OVERRIDE_TEXT_SPEED = 2;`

`bb({body:"fear", mouth:"normal", eyes:"fear"})`

b: ای یعنی اگه ما *همین الان* با یکی بیرون نریم--

`bb({body:"panic"})`

b: می‌میریییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "alone");
publish("hp_show");
```

(...2500)

`_.fifteencigs = true`

n: تو از *ترس از کمبود محبت* استفاده کردی

(#act1b)

# act1a_productive

```
bb({body:"normal", mouth:"small", eyes:"normal"});
hong({body:"0_sammich"});
```

b: همین حالا لپ‌تاپت رو در بیار و شروع کن به کار کردن!

`hong({eyes:"0_annoyed"})`

h: ام، ترجیح میدم خرده نون نریزم تو کیبوردم--

```
bb({mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: اگه ما به بدنه جامعه کمک نکنیم یه انگل اجنماعی محسوب میشیم

b: اونموقع بدن جامعه میره پیش دکتر جامعه که ازش دارو بگیره برای از بین بردن انگل جامعه بعد ما--

```
bb({body:"panic", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: می‌میرییییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "bad");
publish("hp_show");
```

(...2500)

`_.parasite = true`

n: تو از *ترس از آدم بدی بودن* استفاده کردی

(#act1b)

# act1a_bread

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({body:"0_sammich", eyes:"0_annoyed"});
```

h: اصلا اون مطالعات ازمایش شدن--

```
bb({body:"fear", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: گندم فرآوری شده باعث بالا رفتن قند خونمون میشه و بعد مجبور میشن دست و پاهامون رو قطع کنن و بعد ما-

`bb({body:"panic"})`

b: می‌میریییییم

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"0_shock", eyes:"0_shock"});
attack("18p", "harm");
publish("hp_show");
```

(...2500)

`_.whitebread = true`

n: تو از *ترس از صدمه دیدن* استفاده کردی

(#act1b)

# act1b

n: خیلی تاثیر گذاره

`bb({mouth:"smile", eyes:"smile"});`

b: دیدی انسان؟ من گرگ نگهبان وفادار تو‌ام!

`bb({body:"pride_talk"});`

b: به حرف دلت گوش بده! همیشه حق با احساساتته!

`bb({body:"pride"});`

n: جون انسانت رو به صفر برسون

n: برای محافظت از سلامتی جسمانی، اجتماعی و روحی-روانی میتونی از موارد زیر اسفاده کنی:

n: ترس از *صدمه دیدن* #harm#

n: ترس از *کمبود محبت* #alone#

n: ترس از *آدم بدی بودن* #bad#

`Game.OVERRIDE_TEXT_SPEED = 1.25;`

n4: (یه نکته: موقع بازی کردن گزینه هایی رو انتخاب کن که به ترس های واقعی خودت نزدیکتر هستن)

h: ...

```
hong({body:"putaway"});
sfx("rustle");
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

(...1000)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h: میدونی چیه؟ شاید وقتشه گوشیمو یه چک بکنم.

```
sfx("rustle2");
hong({body:"phone1", mouth:"neutral", eyes:"neutral"})
```

n: از انسانت محافظت کن

n: دربرار دنیا. در یرابر دیگران. دربرار خودش.

n: موفق باشی

(...500)

`Game.clearText()`

(...500)

(#act1c)

# act1c

`music('battle', {volume:0.5})`

n: راند اول: *بجنگید*

`bb({body:"normal", mouth:"normal", eyes:"normal"});`

h: ها. صفحه فیس بوکم میگه که دوستم قراره آخر هفته پارتی بگیره.

`bb({eyes:"uncertain"});`

b: اون اسکل *هر هفته* پارتی نمی‌گیره؟

`bb({eyes:"uncertain_right"});`

b: چه خلا درونی رو میخوان پر کنن؟ باید خیلی از درون درب و داغون باشن!

`hong({eyes:"surprise"});`

h: راستی، منم دعوت کردن.

`bb({eyes:"fear", mouth:"normal"});`

b: خب دیگه!

[بگو آره، یا از تنهایی می‌میریم!](#act1c_loner)

[بگو نه، این پارتی ها پر از مواد مخدرن!](#act1c_drugs)

[نادیده بگیرش، ما کلا تو پارتی ها ضدحالیم.](#act1c_sad)

# act1c_loner

{{if _.fifteencigs}}
b: پونزده تا سیگار در روز، پونزده تا!
{{/if}}

{{if !_.fifteencigs}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if !_.fifteencigs}}
b: بعدم هیچ کس نمیاد خاک سپاری ما، خاکسترمون رو میریزن تو دریا، بعد یه وال مارو میخوره،
{{/if}}

{{if !_.fifteencigs}}
b: بعد تبدیل میشیم به عن وال!
{{/if}}

{{if !_.fifteencigs}} `_.whalepoop = true` {{/if}}

(...500)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

{{if !_.fifteencigs}}
b: پس آره حتما باید بریم به اون پارتی!
{{/if}}

{{if _.parasite}}
b: فقط لپ‌تاپ رو لا خودت بیار که اونجا کار کنیم، و انگل اجتماعی نباشیم.
{{/if}}

{{if _.whitebread}}
b: خداکنه نون سفید تو منوشون نباشه!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ای خدا. اگه با بله گفتن من تو خفه میشی، باشه.

h: بهشون میگم میام.

{{if _.whalepoop}}
b: عن وال میشیما! عن وال!
{{/if}}

`_.partyinvite="yes"`

(#act1d)

# act1c_drugs

`bb({mouth:"small", eyes:"fear"});`

{{if _.whitebread}}
b: یا شایدم بدتر... نون سفید!
{{/if}}

{{if _.whitebread}}
`Game.OVERRIDE_TEXT_SPEED = 1.5;`
{{/if}}

{{if _.whitebread}}
b: انقد شیشه می‌کشیمو نون سفید می‌خوریم که اصلا نمی‌تونن جسد خیکی‌مون رو تو کوره مرده سوزی جا بدن!
{{/if}}

{{if !_.whitebread}}
b: قراره انقد مواد بزنیم که حتی مسئول خاکسپاری هم تعجب کنه که چطور بدنمون از قبل مومیایی شده!
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.parasite}}
b: گذشته از این، ما وقت واسه پاتی رفتن نداریم، هنوز کلی از کارامون مونده و اگه کار نکنیم میشیم انگل اجتماعی!
{{/if}}

`hong({mouth:"anger", eyes:"anger"});`

h: ای خدا. اگه با نه گفتن من تو خفه میشی، باشه.

h: بهشون میگم نمیام.

`_.partyinvite="no"`

(#act1d)

# act1c_sad

`bb({eyes:"uncertain_right", mouth:"normal"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.fifteencigs}}
b: ما که کل روز یه گوشه نشستیم و درباره اینکه چطور تنهایی به اندازه 15 سیگار در روز مضره زار می‌زنیم.
{{/if}}

{{if _.parasite}}
b: ما همیشه تو پارتی ها نگران اینیم که به اندازه کافی کار نمیکنیم و مفید نیستیم.
{{/if}}

{{if _.whitebread}}
b: همش نگران اینیم که غذاهای ناسالم قراره بکشنمون.
{{/if}}

```
bb({mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"lookaway"});
```

h: وای یعنی دلیلش چی میتونه باشه.

`hong({eyes:"neutral"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: پس اگه بریم اونارو هم ناراحت میکنیم، ولی اگه دعوتشون رو رد کنیم هم ناراحت میشن!

`bb({body:"fear", eyes:"fear"});`

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

b: ما همش باعث ناراحتی دیگران میشیم، پس خودمونم باید احساس ناراحتی کنیم

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`hong({mouth:"anger", eyes:"anger"});`

h: اه. اگه با نادیده گرفتن من تو خفه میشی، باشه.

h: اصلا به دعوتشون نگاهم نمی‌کنم.

`_.partyinvite="ignore"`

(#act1d)

# act1d

```
bb({body:"normal", mouth:"normal", eyes:"normal"});
hong({mouth:"neutral", eyes:"annoyed"});
```

h: به هر حال. فیس بوک یکم زیادی شلوغه. من به یه چیز ملایم‌تر نیاز دارم که کمتر باعث اضطرابم بشه.

`hong({eyes:"neutral"});`

h: ببینیم تو توییتر په خبره؟

`bb({eyes:"look"});`

[وای نه، نگا چه خبر ناراحت کننده ای!](#act1d_news)

[وای نه، نکنه اون توییت درواقع درباره *ماست*؟](#act1d_subtweet)

[عه، این گربه رو ببین چه ناز شیر میخوره](#act1d_milk)


# act1d_news

```
bb({eyes:"pained1"});
music(null, {fade:2});
```

b: ای خدا، دنیا داره نابود میشه مگه نه؟

```
bb({eyes:"pained2"});
hong({mouth:"sad", eyes:"sad"});
```

b: انگار همش داره تموم میشه، یعنی همه‌چیز داره می‌میره و ما هم محکوم به فناییم و هیچکاری از دستمون بر نمیاد.

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
bb({mouth:"shut"});
```

b: ...

`bb({mouth:"smile", eyes:"smile"});`

b: بیا اون خبر رو ریتوییت کنیم!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.badnews=true`

```
music('battle', {volume:0.5});
hong({mouth:"anger", eyes:"anger"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: باشه ریتوییتش میکنم به شرطی که تو ساکت شی!

`hong({mouth:"neutral", eyes:"annoyed"});`

h: حالا هرچی، بیا یه سر به اسنپ‌چت هم بزنیم.

(#act1e)


# act1d_subtweet

`bb({eyes:"fear"});`

b: یه ساب‌توییته! یه ساب‌توییت خیلی زیرکانه!

`hong({eyes:"annoyed"});`

h: نکه نیست؟

`bb({eyes:"narrow", mouth:"small"});`

b: نکنه دارن پشت سرمون حرف میزنن؟

h: نه نمی--

`bb({body:"fear", eyes:"fear", mouth:"normal"});`

b: جلوی سرمون!

`hong({eyes:"sad", mouth:"sad"});`

h: فک--

`bb({eyes:"narrow", mouth:"small"});`

b: ولی *اگه باشن چی*

h: خفه--

`bb({eyes:"narrow_eyebrow"});`

b: *اگه باشن چی*

```
Game.OVERRIDE_TEXT_SPEED = 0.5;
hong({mouth:"shut"});
```

h: ...

(...1000)

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.subtweet=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: اوکیی، بریم تو اسنپ‌چت.

(#act1e)

# act1d_milk

`hong({mouth:"smile", eyes:"neutral"});`

h: آره خیلی نازه، ریتوییتش کردم--

```
hong({mouth:"shock", eyes:"shock"});
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.8;
```

b: گربه ها نمیتونن شیر رو هضم کنن و ما آدم های آشغالی هستیم که از حیوان آزاری حمایت می‌کنیم!

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
attack("18p", "bad");
```

(...2500)


`_.catmilk=true`

```
hong({mouth:"anger", eyes:"annoyed"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: اوکیی، ببینم اسنپ‌چت چخبره.

(#act1e)

# act1e

`hong({mouth:"neutral", eyes:"neutral"});`

h: عه، عکس های دیشبن. پس اون پارتی های هفتگی *اینطورین*.

{{if _.partyinvite=="yes"}} (#act1e_said_yes) {{/if}}

{{if _.partyinvite=="no"}} (#act1e_said_no) {{/if}}

{{if _.partyinvite=="ignore"}} (#act1e_said_ignore) {{/if}}

# act1e_said_yes

`hong({mouth:"sad", eyes:"annoyed"});`

h: اوه، بنظر خیلی شلوغ میاد برای آدمی مضطرب مثل من.

h: شاید نباید دعوتشون رو قبول میکردم؟

```
hong({mouth:"neutral", eyes:"neutral"});
bb({mouth:"normal", eyes:"normal"});
```

[جوابمون رو عوض کنیم؟ مثل احمقا؟!](#act1e_yes_dontchange)

[جوابتو عوض کن! خیلی شلوغه!](#act1e_yes_changetono)

{{if _.subtweet}}
[آره قطغا منظورشون تو اون توییت ما بودیم.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[صب کن ببینم ما الان بدون تحقیق اون خبر رو ریتوییت کردیم.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[میدونی چیه؟ تو بدن خیلی بد فورمی داری.](#act1e_ignore_posture)
{{/if}}

# act1e_yes_dontchange

```
bb({eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: اونا رو ما حساب کرده بودن که بیایم و حالا ما میخوایم به اعتماد اونا خیانت کنیم؟! میخوای تنها بمیری؟

{{if _.fifteencigs}}
b: پونزده‌تا سیگار.
{{/if}}

{{if _.whalepoop}}
b: عن وال.
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو خفه شو جوابم رو همون بله نگه میدارم

(#act1f)

# act1e_yes_changetono

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: مگه نمیدونی آدما هم میتونن رم کنن؟

```
bb({body:"fear", mouth:"small", eyes:"narrow"});
hong({eyes:"sad", mouth:"sad"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تو سال 2003 تو ایلت رود ایلند آتشسوزی تو یه کلاب باعث شده همه برن سمت در خروجی و 100 نفر سوختن و مردن-
```
bb({body:"normal", mouth:"normal", eyes:"fear"});
hong({mouth:"shock"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: میخوای اون اتفاق برای ما هم بیوفته-

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 2.5;
```

b: بگو نه بگو نه بگو نه بگو نه بگو نه بگو نه بگو نه بگو ن-


```
bb({body:"normal", eyes:"fear", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
hong({eyes:"anger", mouth:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو خفه شو بهشون میگم نمیام! ای خدا!

(#act1f)

# act1e_said_no

`hong({mouth:"sad", eyes:"sad"});`

h: هم... بنظر باحال میاد.

h: شاید نباید دعوتشون رو رد میکردم؟

`bb({mouth:"normal", eyes:"normal"});`

[جوابمون رو عوض کنیم؟ مثل احمقا؟!](#act1e_no_dontchange)

[جوابمون رو عوض کن! تنها نمیر!](#act1e_no_changetoyes)

{{if _.subtweet}}
[آره قطغا منظورشون تو اون توییت ما بودیم.](#act1e_ignore_subtweet)
{{/if}}

{{if _.badnews}}
[صب کن ببینم ما الان بدون تحقیق اون خبر رو ریتوییت کردیم.](#act1e_ignore_factcheck)
{{/if}}

{{if (!_.subtweet && !_.badnews)}}
[میدونی چیه؟ تو بدن خیلی بد فورمی داری.](#act1e_ignore_posture)
{{/if}}

# act1e_no_dontchange

`bb({eyes:"anger"})`

b: همه رو ما حساب کرده بودن!

b: ... که بلاخره تنهاشون میذاری که پارتیشون رو بگیرن و مجبور نباشن به رخیت نحس {{if _.whitebread}}white-bread-munching{{/if}} یکی مثل تو نگاه کنن-


```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
bb({body:"normal", eyes:"uncertain", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو خفه شو جوابم رو نه نگه میدارم!

(#act1f)

# act1e_no_changetoyes

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تنهایی مضمن باعث افزایش کلسترول خون و ریسک ابتلا به بیماری های قلبی-عروقی و سکته میشه!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

{{if _.fifteencigs}}
b: FIFTEEN. CIGARETTES.
{{/if}}

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: خفه شو خفه شو جوابم رو به بله عوض میکنم! ای خدا!

(#act1f)

# act1e_ignore_subtweet

```
bb({eyes:"fear", mouth:"small"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: تمام توییت های مشکل‌دارمون قراره باعث بدبختیمون بشن!

```
bb({body:"fear", eyes:"fear", mouth:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.7;
```

b: قراره مارو رسوا کنن و آبرومون رو ببرن و بعد با طناب به اسب ببندنمون و توی اتوبان اطلاعات انقد بکشنمون تا بمیریم

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: آخه تو چرا همچینی؟

(#act1f)

# act1e_ignore_factcheck

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ما داریم اطلاعات غلط پخش میکنیم! و داریم این دنیای مطبوعات آزاد رو نابود میکنیم!

```
bb({body:"scream"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: ما دلیل بوجود اومدن فاشیسم از خرابه های دموکراسی هستیم!

```
bb({body:"normal", eyes:"anger"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

```
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
_.factcheck = true;
```

h: آخه تو چرا همچینی؟

(#act1f)

# act1e_ignore_posture

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: میخوای بجای ستون فقرات نون سنگک داسته باشی؟ انقد موقع گوشی بازی قوز نکن!

```
bb({body:"meta"});
```

b: تو هم همینطور جناب بازیکن!

```
bb({body:"normal", mouth:"normal"});
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({mouth:"anger", eyes:"anger"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

h: آخه چرا تو همچینی؟

(#act1f)

# act1e_said_ignore

`hong({mouth:"sad", eyes:"sad"});`

h: هم.. بنظر باحال میاد.

h: شاید نباید دعوتشون رو نادیده میگرفتم؟

`bb({mouth:"normal", eyes:"normal"});`

[بازم نادیده بگیر، ما هنوزم زد حالیم.](#act1e_ignore_continue)

[اصلا بهشون بگو میری.](#act1e_ignore_changetoyes)

[اصلا بهشون بگو نمیری.](#act1e_ignore_changetono)

# act1e_ignore_continue

`hong({eyes:"annoyed"});`

h: یکم زشت نیست همش دعوتشون رو نادیده میگیرم؟

`bb({eyes:"normal_right"});`

b: خب بقیه هم همیشه *ما* رو نادیده میگیرن، پس

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`bb({eyes:"normal"});`

b: پس این به اون در

(#act1f)

# act1e_ignore_changetoyes

`hong({eyes:"surprise", mouth:"smile"});`

h: تو...داری به من اجزاه میدی خوش بگذرونم؟

b: آخه، تنهایی *میتونه* مارو بکشه.

`hong({eyes:"neutral", mouth:"neutral"});`

(#act1e_no_changetoyes)

# act1e_ignore_changetono

`bb({eyes:"narrow"});`

b: خیلی شلوغه، شلوغی خطرناکه.

(#act1e_yes_changetono)


# act1f

```
hong({mouth:"neutral", eyes:"neutral"});
bb({body:"normal", mouth:"normal", eyes:"normal"});
```

h: حالا هرچی، پیام جدید از تیندر(برنامه زید‌یابی)

`bb({eyes:"uncertain"})`

b: چی، اون برنامه هرزگی؟

`hong({eyes:"annoyed"})`

h: برنامه هرزگی نیست، فقط یه راه برای آشنایی با آدما--

`bb({eyes:"narrow"})`

b: برنامه هرزگیه.

```
hong({eyes:"surprise", mouth:"smile"});
bb({eyes:"normal"});
```

h: اوه، یه کیس جدید برام پیدا شد! چه ناز و گوگولیه!

```
bb({eyes:"narrow_eyebrow"});
hong({eyes:"sad", mouth:"anger"})
```

h: میشه لطفا به این یه چیز تر نزنی؟

```
bb({body:"panic"});
Game.OVERRIDE_TEXT_SPEED = 2.0;
```

b: خطر خطر خطر خطر خطر خطر

`bb({body:"fear", eyes:"fear", mouth:"normal"})`

[دیگران فقط دارن از ما *استفاده* میکنن](#act1f_used_by_others)

[ما داریم فقط از دیگران *استفاده* میکنیم](#act1f_using_others)

[کیس تو یه قاتل سریالیه!](#act1f_killer)

# act1f_used_by_others

`bb({body:"point_crotch", eyes:"normal", mouth:"normal"})`

b: با هرزگی شاید بتونی سوراخ اون پایینو پر کنی،

b: ولی هیچوقت نمیتونی سوراخی رو پرکنی که...

`bb({body:"point_heart", eyes:"pretty", mouth:"small"})`

b: *اینجاست*.

(...1000)

```
bb({body:"normal", mouth:"normal", eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: منظورم اینه که قراره تنها بمیریم!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "alone");
```

(...2500)

`_.hookuphole=true`

(#act1g)

# act1f_using_others

`bb({eyes:"narrow", mouth:"small"})`

b: فک میکنی کیرای مردم تمبرن که میخوای جمعشون کنی؟

```
bb({body:"sing", eyes:"pretty", mouth:"shut"});
music("pokemon");
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

```
Game.FORCE_TEXT_DURATION = 1000;
Game.FORCE_NO_VOICE = true;
```

b: دوستان این بخش خیلی به فرهنگ ایرانی ربطی نداره و فحشم زیاد میده پس...

(...5600)

```
bb({mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2400;
```

b: ♫ ممد نبودی ببینی

(...500)

```
bb({eyes:"narrow", mouth:"small"});
Game.FORCE_TEXT_DURATION = 2100;
```

b: ♫ شهر آزاد گشته

(...1500)

```
bb({eyes:"pretty"});
Game.FORCE_TEXT_DURATION = 2300;
```

b: ♫ خون یارانت پر ثمر گشته

(...500)

```
bb({eyes:"fear", mouth:"normal"});
Game.FORCE_TEXT_DURATION = 2000;
```

b: ♫ آه و واويلا كو جهان آرا؟

(...1000)

```
bb({eyes:"smile", mouth:"smile"});
Game.FORCE_TEXT_DURATION = 1000;
```

b: ♫ نور دو چشمان تر ما…

```
Game.FORCE_CANT_SKIP = false;
Game.clearText();
music(false);
bb({body:"normal", mouth:"normal", eyes:"normal"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: مهم اینه که تو یه آدم فریبکار چندش هستی!

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "bad");
```

(...2500)

`_.pokemon=true`

(#act1g)

# act1f_killer

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

{{if _.whitebread}}
b: اونا میندازنت تو یه چاه و انقد بهت نون سفید میدن میدن که چاق و چله بشی بعدم میخورنت و از پوستت کت درست میکنن
{{/if}}

{{if _.parasite}}
b: اونا با یه زمان سنج پومودورو میزنن تو سرت و میگن "تو باید مفید تر و پربازده تر میبودی ای انگل بدبخت"
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: از تیکه های بدنت به عنوان نقل و نبات استفاده میکنن و از دل و رودت ریسه درست میکنن بعدم خونت رو به عنوان نوشیدنی سرو میکنن!
{{/if}}

{{if !_.whitebread && !_.parasite}}
b: حالا دعوت پارتی رو چطور دوست داری؟
{{/if}}

```
hong({mouth:"shock", eyes:"shock"});
attack("18p", "harm");
```

(...2500)

`_.serialkiller=true`

(#act1g)

# act1g

```
bb({body:"normal", mouth:"normal", eyes:"look"});
hong({body:"2_tired"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
music(false);
```

h: ...

(...500)

h: من دیگه خسته شدم از این بازی مسخره.

(...700)

`Game.OVERRIDE_TEXT_SPEED = 1.5;`

h:
{{if _.fifteencigs}}"تنهایی مارو میکشه"... {{/if}}
{{if _.parasite}}"ما یه انگل اجتماعی هستیم"... {{/if}}
{{if _.whitebread}}"اونو نخور، میمیریا!"... {{/if}}
{{if _.subtweet}}"اونا دارن پشت سرمون حرف میزنن"... {{/if}}
{{if _.badnews}}"دنیا در حال نابودیه"... {{/if}}
{{if _.hookuphole}}"ما آخرسر تنها میمیریم"... {{/if}}
{{if _.serialkiller}}"اون یه قاتل سریالیه"... {{/if}}
{{if _.catmilk}}"گربه ها نمیتونن شیر رو هضم کنن"... {{/if}}
{{if _.pokemon}}ممد نبودی... {{/if}}

h: من فقط میخوام زندگیمو بکنم.

h: فقط میخوام از شر این همه... درد خلاص بشم

`bb({eyes:"look_sad"});`

b: هی... انسان...

`Game.OVERRIDE_TEXT_SPEED = 0.5;`

b: همه‌چی درست میشه

(...600)

`bb({body:"point_heart", eyes:"look_sad_smile", mouth:"smile"});`

b: As your loyal guard-wolf, I'll always keep an eye out for danger, and do my best to keep you safe.

`bb({body:"normal", eyes:"look_sad", mouth:"smile"});`

b: I promise.

(...600)

```
bb({body:"normal", eyes:"normal", mouth:"normal"});
hong({body:"phone1", eyes:"neutral", mouth:"neutral"});
```

h: Last app. Instagram. What you got?

`hong({eyes:"sad"});`

h: It's... more party pictures.

`hong({mouth:"sad"});`

h: Everyone looks so happy. Free from worry. Free from anxiety.

`hong({mouth:"anger"});`

h: God, why can't I be like them? Why can't I just be *normal?*

`bb({eyes:"normal_right"});`

b: Speaking of parties, about this weekend's invite. Here's my FINAL decision:

`bb({eyes:"normal"});`

[We should go.](#act1g_go) `Game.OVERRIDE_CHOICE_LINE=true`

[We should not go.](#act1g_dont) `Game.OVERRIDE_CHOICE_LINE=true`

# act1g_go

`_.act1g = "go"`

(#act1h)

# act1g_dont

`_.act1g = "dont"`

(#act1h)

# act1h

b: We sh--

```
bb({eyes:"wat", mouth:"small"});
hong({body:"2_fuck"});
```

h: *^FUCK^.*

`hong({body:"2_you"});`

h: YOU.

(...500)

b: w

(...1500)

`bb({eyes:"wat_2"});`

b: wha?

`hong({body:"phone1", eyes:"anger", mouth:"anger"});`

h: I'm going to say YES to that party,

{{if _.act1g=="go"}}
h: NOT because you want me to, but because *I* want to.
{{/if}}

{{if _.act1g=="dont"}}
h: Precisely BECAUSE you don't want me to.
{{/if}}

```
hong({body:"putaway"});
sfx("rustle");
```

h: You're NOT in control of me.

```
sfx("rustle2");
hong({body:"0_sammich", eyes:"0_annoyed", mouth:"0_neutral"});
```

h: Now excuse me while I eat this delicious sandwich in ^goddamn^ peace.

`hong({body:"2_sammich_eat"});`

(...601)

```
sfx("sandwich");
hong({body:"2_sammich_eaten", eyes:"0_lookaway", mouth:"0_chew1"})
```

(...601)

```
bb({body:"normal", eyes:"uncertain", mouth:"shut"});
Game.OVERRIDE_TEXT_SPEED = 0.5;
```

b: ...

```
bb({eyes:"normal_right"});
Game.OVERRIDE_TEXT_SPEED = 1;
```

b: ...

```
bb({eyes:"fear"});
Game.OVERRIDE_TEXT_SPEED = 4;
```

b: ..................

(...500)

`bb({mouth:"normal"});`

[AHHHH WE'RE GONNA DIE](#act1h_death) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH EVERYONE HATES US](#act1h_loneliness) `Game.OVERRIDE_CHOICE_LINE = true;`

[AHHHH WE'RE HORRIBLE PEOPLE](#act1h_worthless) `Game.OVERRIDE_CHOICE_LINE = true;`

# act1h_death

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH WE'RE GONNA DIE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "harm");
```

(...2500)

(#act1i)

# act1h_loneliness

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH EVERYONE HATES US AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "alone");
```

(...2500)

(#act1i)

# act1h_worthless

```
bb({body:"fear"});
Game.OVERRIDE_TEXT_SPEED = 3;
```

b: AHHHH WE'RE HORRIBLE PEOPLE AAAAAAHHHHHHH

```
hong({body:"3_defeated1"});
attack("100p", "bad");
```

(...2500)

(#act1i)

# act1i

```
bb({mouth:"smile_lock", eyes:"smile", body:"normal"});
music('battle', {volume:0.5});
```

n: CONGRATULATIONS

(...500)

n: YOU'VE SUCCESSFULLY PROTECTED YOUR HUMAN'S PHYSICAL + SOCIAL + MORAL NEEDS

n: WHY, LOOK HOW GRATEFUL THEY ARE!

(...500)

n: NOW THAT THEIR ENERGY IS ZERO, YOU CAN DIRECTLY CONTROL THEIR ACTIONS

`bb({mouth:"smile", eyes:"normal"});`

n: PICK YOUR ENDING MOVE

`bb({mouth:"small_lock", eyes:"fear"});`

n: *FINISH THEM*

[{FIGHT: Punish your stressful phone!}](#act1i_phone) `Game.OVERRIDE_CHOICE_LINE=true`

[{FLIGHT: Curl up in a ball and cry!}](#act1i_cry) `Game.OVERRIDE_CHOICE_LINE=true`

# act1i_phone

`bb({mouth:"normal", eyes:"narrow"})`

b: Your phone was giving you a panic attack!

`bb({eyes:"anger"})`

b: Zuckerberg and Co are hijacking your mental health for venture capitalist money!

```
bb({body:"fear", eyes:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Punish your phone! Destroy it! Kill it!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "fight";
```

b: KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL IT KILL I--

(#act1j)

# act1i_cry

`bb({eyes:"fear", mouth:"normal"})`

b: The whole world is filled with danger!

```
bb({body:"fear"});
hong({body:"3_defeated2"});
Game.OVERRIDE_TEXT_SPEED = 1.5;
```

b: Do like the armadillo! Curl up into a ball for self-defense!

```
Game.OVERRIDE_TEXT_SPEED = 2.5;
bb({body:"flail"});
hong({body:"3_defeated3"});
_.act1_ending = "flight";
```

b: CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CRY CURL UP AND CR-- 

(#act1j)

# act1j

`SceneSetup.act1_outro()`