# act4

```
SceneSetup.act4();
publish("SAVE_GAME", ["act4"]);
Game.FORCE_CANT_SKIP = true;
```

(...5001)

```
publish("set_how_many_prompts", [1]);
Game.FORCE_CANT_SKIP = false;
Game.CLICK_TO_ADVANCE = true;
```

n3: (بازی بصورت اتوماتیک ذخیره شد.)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
var hong_frame = _.INJURED ? 9 : 0;
publish("act4", ["hong_walks_in",hong_frame]);
sfx("grass_step1", {volume:0.1});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.2});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.25});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.3});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...1667)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.35});
```

(...666)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step2", {volume:0.35});
```

(...1333)

```
publish("act4", ["hong_walks_in", "next"]);
sfx("grass_step1", {volume:0.20});
```

(...167)

```
publish("act4_hong_sits");
```

(...66)

```
publish("act4", ["hong_transition", "next"]);
sfx("squeak");
```

(...133)

`publish("act4", ["hong_transition", "next"]);`

(...1333)

```
publish("act4", ["hong_transition", "next"]);
sfx("rustle");
```

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1001)

```
publish("act4", ["hong_transition", "next"]);
```

(...333)

```
publish("act4", ["hong_transition", 9]);
sfx("sandwich");
```

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", 9]);`

(...333)

`publish("act4", ["hong_transition", 10]);`

(...333)

`publish("act4", ["hong_transition", "next"]);`

(...1466)

`publish("act4-out-1");`

(...201)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

`publish("act4", ["hong_transition", "next"]);`

(...99)

```
publish("act4-show-chars");
Game.FORCE_CANT_SKIP = false;
```

(...901)

`hong({body:"sigh_1"})`

(...601)

```
hong({body:"sigh_2"});
bb({eyes:"look_down"});
```

h: *نفس عمیق*

```
hong({body:"hold", eyes:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: پس نتیجه اخلاقی این داستان چی بود دقیقا؟

`hong({body:"one_up", eyes:"annoyed"})`

h: چی *یادگرفتیم* اصلا؟ من *داشتم* احمقانه رفتار می‌کردم، "دوستام" *داشتن* از من سوء‌استفاده می‌کردن، و ما تقریبا *مردیم*.

`hong({body:"normal", eyes:"normal"})`

{{if _.INJURED}}
[آره، تازه اگه حرفی از قبض بیمارستان نزنیم.](#act4a_bill)
{{/if}}

{{if !_.INJURED}}
[آره، تازه اگه صدمه به کبدت رو نادیده بگیریم.](#act4a_liver)
{{/if}}

[آره، اون بدترین حالت ممکن *بود*.](#act4a_worst)

[آره، حق با من بود.](#act4a_right)

# act4a_bill

`hong({eyes:"annoyed_l", mouth:"narrow"});`

h: درسته. فک نکنم طرح بیمه من شامل "یه ^اسکل^ بدبخت بودن" رو شامل میشه.

`hong({eyes:"annoyed", mouth:"normal"});`

b: با این‌حال... ما زنده موندیم!

`hong({eyes:"normal"});`

h: ؟

(#act4b)

# act4a_liver

`bb({eyes:"normal_d"});`

b: ما قطعا یه چندسالی از طول عمرمون کم کردیم...

`bb({eyes:"surprise"});`

b: ولی حداقل ما هنوز یه عمری *می‌کنیم*! ما زنده موندیم!

```
hong({eyes:"surprise"});
bb({eyes:"normal"});
```

h: ؟

(#act4b)

# act4a_worst

`bb({eyes:"normal_d"});`

b: و با این‌حال...

h: هم؟

`bb({eyes:"surprise"});`

b: ما زنده موندیم!

(#act4b)

# act4a_right

`bb({eyes:"normal_d"});`

b: ولی... حق با تو هم بود.

`hong({eyes:"surprise"});`

h: هم؟

`bb({eyes:"normal"});`

b: من عین چوپان دروغگو *بودم*. پس وقتی خطر *واقعی* مارو تهدید می‌کرد، تو - با دلیل منطقی - منو باور نکردی.

`bb({eyes:"surprise_r"});`

b: و با این‌حال، ما زنده موندیم!

(#act4b)

# act4b

```
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

b: با وجود همه اینها، ما هنوز اینجاییم.

`hong({eyes:"suspect"});`

{{if _.INJURED}}
h:  تو خیلی آروم بنظر می‌رسی با وجود اینکه ما تازه یه تجربه نزدیک به مرگ داشتیم.
{{/if}}

{{if !_.INJURED}}
h: و خیلی آروم بنظر می‌رسی با وجود اینکه ما تازه یه تجربه *نزدیک* نزدیک به مرگ داشتیم.
{{/if}}

```
hong({eyes:"normal"});
bb({eyes:"annoyed_d", mouth:"narrow"});
```

b: خب، باعث میشه همه‌چی به نسبت کمتر ترسناک بنظر بیاد. همچنین منو به فکر انداخت.

`bb({eyes:"normal", mouth:"normal"});`

b: اگه دعوا من با تو مزخرفه، چون ازت حفاظت نمی‌کنه...

h: ولی دعوا من با تو هم مزخرفه، چون فقط باعث میشه صدات رو ببری بالا...

`bb({eyes:"normal_r"})`

b: پس شاید...

`bb({eyes:"normal"})`

h: شاید ما مجبور نیستیم دعوا کنیم.

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
```

(...301)

`publish("smash",[0]);`

(...2001)

```
publish("smash",[1]);
sfx("smash_glass");
```

(...2601)

```
publish("smash",[2]);
bb({eyes:"normal", mouth:"normal"});
hong({eyes:"normal", mouth:"normal"});
```

(...2001)

`Game.FORCE_CANT_SKIP = false;`

(#act4b_2)

# act4b_2

```
music('dontfight',{fade:5, volume:0.6});
bb({eyes:"annoyed_d"});
```

b: من یه گرگ بزرگ خورنده نیستم. اما من یه گرگ نگهبان هم نیستم.

`bb({eyes:"sad_d"})`

b: من یه سگ صدمه‌دیده پناهگاهی هستم.

`bb({eyes:"sad"})`

b: ما از شرایط سختی گذشتیم. شاید شوک یا غفلت. این دلیلیه که من بعضی وقتا زیادی واکنش میدم و میگم:

```
sfx("yaps", {volume:0.6});
bb({body:"yap_1"});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 215;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: ور ور ور ور ور

(...1884)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_CANT_SKIP = false;
bb({body:"normal", mouth:"scream", eyes:"scream_sad"});
```

b: اما من *نمیخوام* یه سگ ترسو باشم! من میخوام ازت محافظت کنم! من میخوام یه سگ خوب باشم!

`bb({eyes:"sad", mouth:"normal"});`

b: انسان... کمک می‌کنی این گرگ رو رام کنی؟

`hong({eyes:"sad"})`

h: من... من سعیم رو می‌کنم.

`hong({eyes:"normal_l", body:"chin", mouth:"narrow"})`

h: خب. رابطه سالم با احساسات. رابطه‌ها نیاز به ارتباط خوب دارن. پس، بیا ارتباط برقرار کنیم.

`hong({eyes:"normal", body:"hands_1", mouth:"normal"})`

h: پنج دقیقه بعدی قراره خیلی بیخود باشن، اما بیا وانمود کنیم تا بهش برسیم.

```
hong({body:"hands_2", mouth:"normal"});
```

h: گرگ درون عزیز... حال *تو* چطوره؟

n2: تمام ترس های استفاده شده:

n2: *صدمه دیدن* {{_.attack_harm_total}}, *کمبود محبت* {{_.attack_alone_total}}, *آدم بدی بودن* {{_.attack_bad_total}}

n2: می‌خوای اول درباره کدوم ترس صحبت کنی؟

```
_.a4_fears_discussed = 0;
_.num_thanks = 0;
hong({body:"normal"});
bb({eyes:"normal"});
```

[من می‌ترسم ما صدمه ببینیم.](#act4_harm)

[من می‌ترسم ما تنها می‌مونیم.](#act4_alone)

[من می‌ترسم ما آدم بدی هستیم.](#act4_bad)

# act4_harm

```
_.a4_talked_about_harm = true;
_.a4_fears_discussed += 1;
```

`bb({eyes:"normal_d"})`

b: من می‌خوام از سلامت فیزیکیت حفاظت کنم،

`bb({eyes:"sad_d"})`

b: ولی *کل دنیا* خطرناک بنظر میاد، پر از مصیبت و شرارت.

`bb({eyes:"sad"})`

{{if _.a4_fears_discussed==1}}
b: من نمدونم، دیگه *من* به اندازه کافی انتخاب کردم چی بگی. تو چی میخوای بگی، انسان؟
{{/if}}

{{if _.a4_fears_discussed==2}}
b: دوباره، نوبت توعه، انسان. چی تو ذهنته؟
{{/if}}

{{if _.a4_fears_discussed==3}}
b: فکر دیگه‌ای داری، انسان؟
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[حق با توعه. بیا از خودمون محافظت کنیم.](#act4_harm_skills)

[بیا خودمون رو در معرض خطرات *بیشتری* قرار بدیم.](#act4_harm_exposure)

[ممنون.](#act4_thanks) `_.thanks_for = "سلامتی فیزیکی";`

# act4_harm_skills

`bb({eyes:"look_down", body:"paw"})`

b: ولی... چجوری؟ من نیش و پنجه دارم، ولی من فقط یه کنایه‌ام.

```
bb({ body:"normal", eyes:"normal" });
hong({ body:"one_up", eyes:"surprise" });
```

h: می‌تونیم دفاع شخصی یادبگیریم؟ عضو یه اجتماع بشیم که از همدیگه محافظت می‌کنن؟ سلامت و فضای شخصی خودمون رو ارتقا بدیم؟

```
bb({ eyes:"annoyed_r" });
hong({ body:"normal", eyes:"normal" });
```

b: شاید، اما...

[اصلا از کجا شروع کنیم؟](#act4_harm_skills_start)

[اگه بازم کار نکنن چی؟](#act4_harm_skills_work)

[اگه توی حفاظت زیاده‌روی کنیم چی؟](#act4_harm_skills_overboard)

# act4_harm_skills_start

`bb({ eyes:"sad_d" })`

b: کلی کار باید انجام بدیم، کلی از رفتار هامون رو باید اصلاح کنیم. اصلا از کجا *شروع* کنیم؟

`hong({ body:"shrug", eyes:"surprise" })`

h: همین الان داریم شروع می‌کنیم.

`bb({ eyes:"normal", mouth:"narrow" })`

b: ها؟

```
bb({ body:"normal", mouth:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal"});
```

h: همین الان داریم ارتباط خوب داشتن رو تمرین می‌کنیم. که بهمون کمک می‌کنه خطرات رو بهتر تشخیص بدیم، با اشتباهات خیلی کمتر.

`hong({ eyes:"surprise" });`

h: و *اون* جلوی صدمه دیدن مارو می‌گیره.

`hong({ eyes:"normal", mouth:"normal" });`

h: بنابراین: این *همون* تمرین دفاع از خوده.

`bb({ eyes:"normal_r" })`

b: هاه. من بیشتر توقع داشتم یچیزی مثل این باشه:

```
Game.FORCE_CANT_SKIP = true;
Game.clearText();
hong({ eyes:"sad", mouth:"smile" });
bb({ body:"karate_1" });
sfx("hiya");
```

(...1001)

`Game.FORCE_CANT_SKIP = false;`

(#act4_something_else)

# act4_harm_skills_work

`bb({ eyes:"normal" });`

h: درسته، ما هیچ‌وقت نمی‌تونیم 100% از خودمون محلفظت کنیم...

`hong({ body:"one_up" });`

h: ولی حتی 1% پیشرفت هم بهتر از هیچیه، مگه نه؟

```
bb({ eyes:"annoyed" });
hong({ normal:"one_up" });
```

b: تو داری لیوان رو بجای 99% خالی، 1% پر می‌بینی؟

`bb({ eyes:"normal" });`

h: همونم هنوز با‌ارزشه اگه وسط بیابون گیر افتادی.

`bb({ eyes:"closed" });`

b: خب. نوش جانت اگه اینطوریه.

(#act4_something_else)

# act4_harm_skills_overboard

`bb({ body:"chest", eyes:"annoyed" })`

b: منظورم اینه که، اصلا همه دلیلی که تو به هشدار های من توجه نکردی این بود که *من* تو حفاظت زیاده‌روی کردم!

`bb({ body:"normal", eyes:"normal" })`

h: حق با توعه. ما باید حفاظت رو با ملایمت انجام بدیم. همه‌چیز رو با ملایمت انجام می‌دیم.

`bb({ eyes:"suspect" })`

b: ببخشید، *همه‌چیز* رو با ملایمت انجام می‌دیم؟!

`hong({ eyes:"annoyed" })`

h: *یه مقدار ملایمی از چیزها* رو با ملایمت انجام می‌دیم.

```
bb({ eyes:"closed" });
hong({ eyes:"normal" });
```

b: ممنون که جملاتت رو درست می‌کنی.

(#act4_something_else)


# act4_harm_exposure

`bb({ mouth:"scream_talk", eyes:"scream", MOUTH_LOCK:true });`

b: *چی*

```
bb({ mouth:"narrow", eyes:"suspect" });
hong({ body:"one_up" });
```

h: منظورم اینه که، بیا تصور کنیم یه سگ از رعد و برق می‌ترسه.

`hong({ body:"hands_1" });`

h: یه ترفند که مربی سگ ها استفاده می‌کنن اینه که صدای رعد و برق رو با شدت کم برای سگ پخش می‌کنن، اگه سگ آروم موند بهش جایزه میدن.

`hong({ body:"hands_2" });`

h: بعد از چند روز، مربی شدت صدا رو کم کم افزایش میده، تا زمانی که سگ دیگه از رعد و برق نمی‌ترسه.

```
hong({ body:"normal", eyes:"surprise" });
bb({ mouth:"normal", eyes:"normal" });
```

h: به این روش میگن مواجهه درمانی!

`hong({ body:"point", eyes:"normal" });`

h: از اونجایی که تو یه سگی، باید برای تو هم کار کنه، مگه نه؟ همه پستانداران یه نوع غریزه ستیر یا گریز دارن.

`hong({ body:"normal" });`

[اگه تو حساسیت زدایی *زیاده روی* کردیم چی؟](#act4_harm_exposure_overboard)

[اگه در معرض خطر *واقعی* قرار گرفتیم چی؟](#act4_harm_exposure_hurt)

[من یه گرگم نه سگ.](#act4_harm_exposure_dog) `bb({ eyes:"suspect" })`

# act4_harm_exposure_dog

h: منم باهات با صبر و مهربانی رفتار می‌کنم تا زمانی که به یه سگ اهلی گوگولی تبدیل بشی.

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"sad", mouth:"smile" })`

b: آخی.

(#act4_something_else)

# act4_harm_exposure_overboard

`bb({ eyes:"annoyed" })`

b: ما *همین الان* دیدم چی میشه وقتی ترست رو سرکوب می‌کنی - خودتو وارد موقعیت هایی می‌کنی که *واقعا* خطرناکن.

`bb({ eyes:"angry_r", body:"one_up" })`

b: بعدم، فک نمی‌کنی حساسیت زدایی زیادی مارو روانی می‌کنه؟

`bb({ mouth:"scream", eyes:"scream", body:"two_up" })`

b: خیلی زود خودمونو با دیدن قیلم های قتل خوشحال می‌کنیم.

`hong({ eyes:"annoyed" })`

h: فک...کنم یه مرزی بین اون و رعد‌و‌برق وجود داره.

`bb({ body:"normal", mouth:"normal", eyes:"suspect" })`

b: ولی دقیقا *کجا*، انسان؟ *کجا؟!*

`hong({ eyes:"surprise", body:"one_up" })`

h: خب نمی‌دونم. ولی *تو* می‌تونی بهم کمک کنی.

`hong({ eyes:"normal", body:"normal" })`

h: با کار کردن و مذاکره کردن باهم، اون مرز رو مشخص می‌کنیم.

`bb({ body:"paw", mouth:"narrow", eyes:"closed" })`

b: باشه. ولی من انگشت شصت ندارم، پس تو باید مرز رو بکشی.

(#act4_something_else)

# act4_harm_exposure_hurt

`bb({ body:"two_up", eyes:"angry_r" })`

{{if _.INJURED}}
b: برای مثال: ما از بالای یه *سقف* پریدیم پایین!
{{/if}}

{{if !_.INJURED}}
b: برای مثال: کم مونده بود از بالای یه *سقف* بپریم پایین!
{{/if}}

```
hong({ eyes:"annoyed" });
bb({ body:"normal", eyes:"annoyed" });
```

h: نه حق با توعه. آدم *می‌تونه* زیاده روی کنه.

`hong({ eyes:"normal" });`

h: ولی واسه همینه که اگه مواجهه درمانی کنیم، با قدم های کوچیک شروع می‌کنیم به بالا رفتن.

h: و درست قبل اینکه به خطر *واقعی* برسیم، توقف می‌کنیم.

`bb({ eyes:"annoyed_r", mouth:"narrow" });`

b: آره منم مرز بین ترسیدن از صدای بلند رعد و برق و ایستادن وسط یه توفان با یه کلاه بلند نوک تیز رو مشخص می‌کنم.
(#act4_something_else)

# act4_thanks

`_.num_thanks += 1`

{{if _.num_thanks==1}}
(#act4_thanks_1)
{{/if}}

{{if _.num_thanks==2}}
(#act4_thanks_2)
{{/if}}

{{if _.num_thanks==3}}
(#act4_thanks_3)
{{/if}}

# act4_thanks_1

`bb({ MOUTH_LOCK:true })`

b: ...

`bb({ eyes:"annoyed" })`

b: صب کن ببینم، یعنی هیچی برای گفتن درباره احساسات من نداری؟ فقط... "ممنون"؟

`hong({ eyes:"surprise", body:"shrug" })`

h: آره! ممنون که نگران {{_.thanks_for}} من هستی.

```
bb({ eyes:"closed_annoyed", MOUTH_LOCK:true });
hong({ eyes:"normal", body:"normal" });
```

b: ...

h: حالت خوبه؟

`bb({ eyes:"super_sad", mouth:"narrow" });`

b: تو تابحال از من تشکر نکرده بودی.

`hong({ mouth:"smile" });`

h: آاا چه گرگ گوگولی و پشمالویی.

(#act4_something_else)

# act4_thanks_2

h: با اینکه بعضی وقتا بیش از حد واکنش میدی، مرسی که مراقب {{_.thanks_for}} من هستی.

`bb({ eyes:"annoyed" })`

b: صب کن ببینم... تو که "ممنون" رو تکرار نمی‌کنی که فقط نخوای درباره این ترس ها صحبت کنی؟

```
bb({ eyes:"normal" });
hong({ eyes:"annoyed", body:"chin" });
```

h: خب، قضیه پیچیده‌ایه، و من همیشه جوابارو حاضر و آماده ندارم.

`hong({ eyes:"annoyed_l", body:"one_up" })`

h: اینجوری نیست که زندگی بهت یه لیست سه تایی از دیالوگ های آماده بده.

`hong({ eyes:"normal", mouth:"smile", body:"normal" })`

h: ولی فعلا حداقل میتونم بگم، ممنون.

b: خب، منم می‌خوام بگم ممنون، ممنون که صبورانه به حرفام گوش میدی.

`bb({ eyes:"closed" });`

b: آخیی تو سگ کوچولو کی بودی؟

(#act4_something_else)

# act4_thanks_3

h: با اینکه ورور کردن تو منو می‌ترسونه، تو فقط می‌خوای از  {{_.thanks_for}} من محافظت کنی.

`bb({ eyes:"smile_r" });`

b: باشه، اگه هی بخوای اینجوری از من تعریف کنی، مردم فکرای بدی درباره ما می‌کنن.

```
bb({ eyes:"smile" });
hong({ eyes:"annoyed" });
```

h: بی‌خیال، من فقط یه بچه دانشجو آسیب پذیرم و تو فقط یه گرگ بزرگ درنده. چه اتفاق بدی می‌تونه بی--

`hong({ eyes:"normal", body:"point" });`

h: اصلا جواب اون سوالو نده.

(#act4_something_else)




# act4_alone

```
_.a4_talked_about_alone = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"sad_d" });`

b: من فقط می‌خوام مطمئن بشم تو به اون نیاز درونی انسانی متعلق بودن برسی.

`bb({ eyes:"sad_u" });`

b: ولی من نگرانم که اگه یوقت یکی مارو - ما *واقعی* - رو بشناسه ما اونو می‌ترسونیم.

`bb({ eyes:"sad" });`

{{if _.a4_fears_discussed==1}}
b: من نمدونم، دیگه من به اندازه کافی بریدم و دوختم. تو نظرت چیه انسان؟
{{/if}}

{{if _.a4_fears_discussed==2}}
b: دوباره نوبت توعه انسان، نظرت چیه؟
{{/if}}

{{if _.a4_fears_discussed==3}}
b: نظری نداری انسان؟
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[من موافقم: بیا روی زندگی اجتماعی‌مون کار کنیم.](#act4_alone_skills)

[به نظر من مردم از ما خوششون میاد، می‌خوای ببینیم؟](#act4_alone_experiment)

[ممنون.](#act4_thanks) `_.thanks_for = "تعلق اجتماعی";`

# act4_alone_skills

```
bb({ eyes:"normal" });
hong({ body:"chin" });
```

h: ما می‌تونیم مهارت هایی مثل سوال پرسیدن، گوش‌دادن و همدلی کردن، باز و آسیب پذیر بودن رو تمرین کنیم؟

`hong({ eyes:"normal_l" });`

h: یا می‌تونیم روی عادت های اجتماعی‌مون کار کنیم و اونا رو بهتر کنیم، مثلا می‌تونیم زمان مشخصی رو برای وقت گذروندن و رفتن به دورهمی با دوستامون تعیین کنیم؟

`hong({ body:"one_up" });`

h: و می‌تونیم سعی کنیم با جواب رد شنیدن راحت‌تر برخورد کنیم.

`hong({ eyes:"normal" });`

h: یا می‌تونیم یادبگیریم که چه مواقعی مردم به ما جواب رد *نمیدن* و فقط قیافه عبوسی دارن.

```
hong({ body:"normal" });
bb({ eyes:"annoyed_r" });
```

b: خیلی گزینه های مختلفی هست، ولی اگه بخوایم درباره مهارت های اجتماعی صحبت کنیم...

[بنظرت *گول زننده* نیست؟](#act4_alone_skills_manipulative)

[بنظرت باعث نمیشه ما *راحت‌تر گول بخوریم؟*](#act4_alone_skills_manipulated)

[اگه بازم موفق نشیم چی؟](#act4_alone_skills_fail)

# act4_alone_skills_manipulative

`bb({ eyes:"suspect" });`

b: اون قاتل های سریالی که می‌تونن احساسات قربانی‌هاشون رو بخونن هم "همدلی" بلد نیستن؟

`bb({ eyes:"annoyed" });`

b: چارلز منسون(قاتل و رهبر فرقه خانواده منسون) نبود که دوستای زیادی داشت و روی خیلی‌ها تاثیر گذاشت؟

`hong({ eyes:"annoyed", body:"chin" });`

h: نه، حق با توعه.

h: "مهارت های اجتماعی" به هیچ دردی نمیخورن وقتی ما *واقعا* به دیگران اهمیت ندیم.

`hong({ body:"normal" });`

h: خلاصه، آدم ^کیری^ نباش.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: این میتونه یه پوستر انگیزشی باشه.

`hong({ body:"shrug", mouth:"narrow" });`

h: "^کیری^ نباش."

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: خودمونو تبدیل می‌کنیم به یه پادری "خوش آمدید"، هی میگیم "لطفا" و "ممنون" وقتی که مردم پاهاشون رو با ما تمیز می‌کنن.

`bb({ mouth:"scream", eyes:"scream" })`

b: انقد پاچه خواری مردم رو می‌کنیم که تیکه های پارچه لای دندون هامون گیر کنه.

```
bb({ mouth:"normal", eyes:"normal" });
hong({ body:"chin" });
```

h: نه، تو راست میگی. مهرات های اجتماعی فقط شامل خوشحال کردن دیگران نیست، ما باید *حریم شخصی* خودمون رو هم مشخص کنیم.

`hong( body:"one_up" });`

h: مل نمیتونیم بقیه رو به خونه خودمون دعوت کنیم اگه خونمون دیوار نداشته باشه.

```
hong({ eyes:"angry", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: و اینکه منظورت چیه تیکه های پارچه لای دندونهامون گیر کنن؟

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: شاید موفق نشیم. در واقع، موفق *نمیشیم*.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: و این چیز بدی نیست! شکست مقدمه پیروزیه!

`hong({ body:"normal", eyes:"normal" });`

h: پس بیا با هم شکست بخوریم، نظرته؟

`bb({ eyes:"normal_r" });`

b: باشه، گمونم... تو بدترین حالت ممکن

`bb({ eyes:"normal" });`

h: آره، فکر کنم این روزا هزینش فقط دو بیت‌کوینه.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: می‌تونیم چندتا چیز رو امتحان کنیم!

`hong({ body:"chin" });`

h: می‌تونیم به یه دوست پیام بدیم که با هم بگردیم، با یه رفیق قدیمی دوباره ارتباط برقرار کنیم، یا حتی فقط با یه باریستا گپ بزنیم.

`hong({ body:"normal" });`

h: فکر کنم متوجه بشیم که دوست‌داشتنی‌تر از چیزی هستیم که فکر می‌کنیم.

`bb({ eyes:"annoyed" });`

[اگه اینا پیروزی‌های کوچیک و بی‌ارزش باشن چی؟](#act4_alone_experiment_cheap)

[اگه این کار برای دیگران دردسرساز باشه چی؟](#act4_alone_experiment_burden)

[اما حرف زدنای روزمره که نشون دهنده خود *واقعی* ما نیست!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: اگه یه لبخند سطحی بزنیم، هیچوقت واقعاً با کسی ارتباط برقرار نمی‌کنیم،

`bb({ eyes:"super_sad" });`

b: *اما* اگه با بقیه راحت باشیم، همه میتونن باطن درب و داغون مارو ببین!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: غلت بزن.

b: چی.

`hong({body:"hands_1"})`

h: وقتی سگ‌ها میخوان عشق و اعتمادشونو نشون بدن، با نشون دادن شکمشون خودشونو آسیب‌پذیر جلوه میدن.

`hong({body:"one_up"})`

h: شاید ما *هنوز* اونقدر احساس امنیت نمی‌کنیم که خیلی جلو هم آسیب‌پذیر باشیم، اما با تمرین کافی،

`hong({body:"normal", eyes:"surprise"})`

h:  یه روزی می‌تونیم خود واقعیمون رو به مردم نشون بدیم – کاملاً درب و داغون، کاملاً انسان.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: اگه بهم جایزه بدی غلت می‌زنم.

`bb({ eyes:"normal", mouth:"normal" });`

h: نه.

(#act4_something_else)


# act4_alone_experiment_cheap

b: سلام کردن به یه باریستا دقیقا لایق مدال طلای اجتماعی بودن نیست.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: برای *ما* هست!

`hong({ body:"one_up", eyes:"annoyed" });`

h: تو کشتی اجتماعی، ما حتی تو رده پَر وزن هم نیستیم، ما بیشتر نزدیک رده وزن کوارکیم.

`hong({ body:"normal", eyes:"normal" });`

h: اگه مجبوریم با پیروزی‌های کوچیک و بی‌ارزش شروع کنیم، باشه. باید قبل از پله هزارم، پله اول رو بالا بری.

b: آره! شاید بعد از گفتن "سلام"، بتونیم پیشرفت کنیم به گفتن...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"چطوری؟"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"چه خبر!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: شاید باریستا فقط میخواد اون قهوه لعنتی رو درست کنه، نه اینکه یه *آزمایش* باشه تا ما ببینیم مهارت‌های اجتماعی‌مون افتضاحه یا نه.

`bb({ eyes:"annoyed" })`

h: خب، اگه معلوم بشه که ما *داریم* مایه دردسر میشیم...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: اینم خوبه که بدونیم!

`hong({ eyes:"normal" });`

h: اونوقت می‌تونیم یاد بگیریم چطور فعالانه از مردم بپرسیم با چی راحتن، تا حریم شخصی دیگران رو بشناسیم و بهشون احترام بذاریم.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: میدونی، همه اون ^چرندیات^ "مهارت‌های بین فردی" که تو بروشورهای مشاوره می‌بینیم.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: من می‌خوام از نیازهای اخلاقی تو دفاع کنم، اون انگیزه‌ای که تو رو به آدم بهتری شدن سوق میده،

`bb({ eyes:"sad_d" })`

b: اما ته دلم حس می‌کنم که ما اساساً... داغونیم.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: و بهم نگو که ما داغون *نیستیم*. ما از یه *سقف* پریدیم پایین.
{{/if}}

{{if !_.INJURED}}
b: و بهم نگو که ما داغون *نیستیم*. ما تقریبا از یه *سقف* پریدیم پایین.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: نمی‌دونم، دیگه بسه خسته شدم از بس *من* انتخاب کردم چی بگیم. تو چی میگی، آدمیزاد؟
{{/if}}

{{if _.a4_fears_discussed==2}}
b: دوباره، نوبت توئه، آدمیزاد. تو چی فکر می‌کنی؟
{{/if}}

{{if _.a4_fears_discussed==3}}
b: فکر دیگه‌ای داری، آدمیزاد؟
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[پس ما داغونیم. بیا درستمون کنیم.](#act4_bad_fix)

[پس ما داغونیم. بیا باهاش کنار بیایم.](#act4_bad_accept)

[ممنون.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: می‌تونیم آروم آروم عادت‌های بهتری بسازیم، زندگیمون رو بیشتر با چیزایی که برامون ارزش داره هماهنگ کنیم،

`hong({body:"one_up"});`

h: و اگه لازم شد، می‌تونیم از یه متخصص کمک بگیریم – یه روانشناس یا مشاور.

`hong({body:"normal"});`

h: راه‌هایی برای درست کردن ما وجود داره

[اگه نتونیم همه‌چیز رو درست کنیم چی؟](#act4_bad_fix_cant)

[اگه *زیادی* درست کنیم چی؟](#act4_bad_fix_too_much)

[ما نمی‌تونیم از پس هزینه مشاوره بربیایم.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: نه، فکر کنم حق با توئه.

h: ما نمی‌تونیم همه‌چیز رو درست کنیم.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: آآآآخ میدونستم ما همیشه خراب می‌مونیم!

`hong({eyes:"surprise"});`

h: اما حداقل می‌تونیم *کمتر* خراب باشیم.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: زخم‌ها با گذر زمان خوب میشن، اما هیچوقت از بین نمیرن. و این اشکالی نداره.

`bb({eyes:"annoyed_r"});`

b: لابد. تازه،

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: زخم‌ها *جذاب* هستن.

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: لطفاً این کارو نکن.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: اعتراف این حال بهم زنه، اما... یه بخشی از من *میخواد* که این اختلال رو داشته باشه.

`bb({ eyes:"angry" })`

b: منظورم اینه که، بدون اون، ما *کسل‌کننده* نمیشیم؟

`bb({ eyes:"sad_r", body:"one_up" })`

b: بدون این اختلال، هنرمون بی‌روح و بی‌مزه نمیشه؟

`bb({ eyes:"sad_u", body:"two_up" })`

b: بدون این اختلال، نمی‌تونیم با دوستامون که این اختلال رو دارن ارتباط برقرار کنیم؟

`bb({ eyes:"sad", body:"chest" })`

b: اگه یه روزی از زندگی راضی باشیم، دیگه خودمونو برای انجام کارهای بزرگ تحت فشار قرار نمیدیم؟

`hong({ MOUTH_LOCK:true })`

h: ...

h:حتی اکه ما از... "تموم شدن ترسامون" هم می‌ترسیم...

h: فکر نکنم ترسامون تموم بشه.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: اوه، آره! آخیش! خیالم راحت شد!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "دکتر، من اضطراب دارم که ساعتی ۱۰۰ دلار میدم فقط برای اینکه ازم بپرسی *این چه حسی بهت میده؟"*

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "اوهوم. و این چه حسی بهت میده؟"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: نه، این یه نگرانی کاملاً منطقیه.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: و واقعاً افتضاحه که خدمات سلامت روان برای خیلی از مردم مقرون‌به‌صرفه نیست.

`hong({ eyes:"normal", mouth:"normal" });`

h: با این حال، چندتا گزینه ارزون یا رایگان وجود داره:

`hong({ body:"chin" })`

h: گروه‌های حمایتی، روانشناسی آنلاین، مراکز بهداشت دانشجویی/غیرانتفاعی...

`hong({ body:"hands_1" })`

h: ساختن عادت‌هایی مثل مدیتیشن، خوب خوابیدن، مرتب گپ زدن با دوستا، یاد گرفتن چیزای جدید...

`hong({ body:"hands_2" })`

h: رفتن به کتابخونه برای قرض گرفتن کتاب‌های روان‌درمانی‌های مبتنی بر شواهد...

`hong({ body:"one_up" })`

h: یه لیست کامل از منابع در انتهای این بازی هست!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: خب *اون* دیوار چهارم هم زیاد دووم نیاورد.

`hong({ body:"point" });`

h: بعضی چیزا از قراردادهای روایی مهم‌ترن. مثل سلامت روان.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: منظورم اینه که، این چیزیه که روانشناس‌ها میگن، درسته؟ همه احساساتت رو بپذیر، حتی منفی‌هاشو؟

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: صبر کن.

["منظورت پذیرفتن" به معنی تسلیم شدن؟](#act4_bad_accept_give_up)

[منظورت "پذیرفتن" به معنی تایید کردن؟](#act4_bad_accept_approve)

[منظورت "پذیرفتن" به معنی  تحت‌اللفظی برداشت کردن؟](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: فکر می‌کنی مارتین لوتر کینگ می‌گفت، "ای بابا نمی‌تونیم جلوی اتوبوس بشینیم، بیاین فقط *بپذیریمش*؟"

`bb({ eyes:"angry_r", body:"two_up" });`

b: چرا مجتمع صنعتی خود-یاری فکر می‌کنه بالا بردن پرچم سفید یه جور *حکمت عمیقه*؟

`bb({ eyes:"annoyed", body:"normal" });`

h: فکر کنم منظور روانشناس‌ها از "پذیرفتن" چیزای بد اینه که: اعتراف کنیم که وجود دارن و تغییر دادنشون سخته،

h: اما نه لزوماً دست کشیدن از تعهد به تغییر.

`bb({ eyes:"suspect" });`

b: پس روانشناس‌ها باید بگن *اذعان کردن*، نه *پذیرفتن*.

`hong({ body:"chin", eyes:"annoyed" });`

h: آره راست میگی، "پذیرفتن" یه جورایی گیج‌کننده‌س.

`bb({ eyes:"closed", mouth:"narrow" });`

b: خب، من به این *اذعان می‌کنم*.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b:  انگار که *خوبه* که ما داغونیم یا یه همچین چیزی؟ نه!

`bb({ eyes:"angry_r", body:"one_up" });`

b: همه اون فیلمنامه‌نویسای لعنتی هالیوود که بیماری روانی رو رمانتیک جلوه میدن، چرت میگن!

`bb({ eyes:"angry", body:"two_up" });`

b: داشتن اختلال روانی *افتضاحه*! زندگی رو از مردم *می‌دزده*! چرا باید اونو "بپذیریم"؟!

`bb({ body:"normal" });`

h: فکر کنم منظور روانشناس‌ها از "پذیرفتن" احساساتمون اینه که: باهاشون صبور باشیم.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: مثل اینکه چطور دست و پا زدن تو باتلاق باعث میشه سریع‌تر فرو بری، و راه‌حلش اینه که صبورانه صاف دراز بکشی،

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: جنگیدن با تو، ترس من، باعث شد از یه سقف بپرم پایین.
{{/if}}

{{if !_.INJURED}}
h: جنگیدن با تو، ترس من، تقریباً باعث شد از یه سقف بپرم پایین.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: به جاش، راه‌حل اینه که کاری رو بکنیم که الان داریم می‌کنیم – نه اینکه بجنگیم، بلکه با هم صبور باشیم.

`bb({ eyes:"annoyed" });`

b:  پس باید *اونو* بگن به جای یه کلمه مشکل‌ساز مثل "پذیرفتن".

`hong({ body:"chin", eyes:"annoyed" });`

h: آره راست میگی، "پذیرفتن" یه جورایی مزخرفه.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: من "پذیرفتن" رو نمی‌پذیرم.

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: اما ما که از قبل *می‌دونیم* نباید حرفای منو تحت‌اللفظی بگیری!

`bb({ eyes:"sad_u", body:"two_up" });`

b: کل *مشکل* اینه که من می‌خوام بهت کمک کنم، اما تو استفاده از کلمات برای این کار افتضاحم!

`bb({ eyes:"sad", body:"normal" });`

h: فکر کنم منظور روانشناس‌ها از "پذیرفتن" احساساتت اینه که: "باهاشون نجنگ یا نادیده‌شون نگیر."

`hong({ eyes:"surprise", body:"one_up" });`

h:  اینکه بهت گوش بدیم، *با* تو کار کنیم، اما حرفاتو به عنوان حقیقت ۱۰۰٪ تحت‌اللفظی نگیریم.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: پس باید *اونو* بگن به جای یه کلمه مبهم و گیج‌کننده مثل "پذیرفتن".

`hong({ body:"chin", eyes:"annoyed" });`

h: فکر کنم اونا هم تو استفاده از کلمات افتضاحن.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: به هر حال، چیز دیگه‌ای هست که بخوای در موردش گپ بزنیم؟
{{/if}}

{{if _.a4_fears_discussed==2}}
h: خب، چیز دیگه‌ای تو دل خونت مونده؟
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[می‌ترسم آسیب ببینیم.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[می‌ترسم تنها بمونیم.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[می‌ترسم ما آدمای بدی هستیم.](#act4_bad)
{{/if}}

[نه، فعلاً خوبم.](#act4c_prelude)

# act4_something_else_2

h: باشه، فکر کنم الان در مورد همه ترسامون صحبت کردیم.

b: آره، فقط سه تا ترس وجود داره.

h: آره، دقیقاً سه تا.

b: چه خوب.

(#act4c)

# act4c_prelude

h: گپ خوبی بود، تیم.

(#act4c)

# act4c

```
Game.clearText();
music(null,{fade:3});
bb({body:"normal", eyes:"normal", mouth:"normal", MOUTH_LOCK:true},0);
hong({body:"normal", eyes:"normal", mouth:"normal"},0);
```

b: ...

`hong({MOUTH_LOCK:true},0)`

h: ...

`bb({eyes:"annoyed_d"})`

b:  این یه *بازی* نیست، میدونی.

`bb({eyes:"angry_d", body:"one_up"})`

b: ساختن یه رابطه سالم با احساساتت به سادگی کلیک کردن دکمه‌ها روی صفحه نمایش نیست.

`bb({eyes:"sad", body:"normal"})`

b: *واقعاً* می‌تونیم با هم کنار بیایم؟

b: *می‌تونیم* با هم کار کنیم، به عنوان یه تیم؟

`hong({eyes:"sad", body:"one_up"})`

h: خب،

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: بـ... ببخشید...

```
Game.clearText();
publish("act4-in-2");
music('campus', {volume:0.5, fade:1});
```

(...2101)

(#act4d)

# act4d

`Game.WORDS_HEIGHT_BOTTOM = 221;`

`publish("act4", ["alshire", 0]);`

a: مـ... میـ... میشه برای ناهار پیشتون بشینم؟

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s:  *این* کراش توئه؟ چرا مثل یه قاتل زنجیره‌ای روانی تنها نشسته؟
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: از کراشت می‌پرسی می‌تونی پیشش بشینی؟ میدونی چقدر *وابسته* به نظر میایم؟!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s:  *این* کراش توئه؟ آرامش و سکوتشون رو به هم زدیم! ما چقدر مایه دردسریم!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: مـ... منظورم اینه... اگه نه هم اشکالی نداره، من فقط...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[صبر کن، من تو رو تو مهمونی ندیدم](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[آره، البته! بیا اینجا.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[ببخشید، الان به تنهایی نیاز دارم.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: آره تو روی کاناپه بودی! تو اولین مهمونی‌ای که رفتم...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: جایی که اون حمله پنیک بهم دست داد و میزبان رو زدم.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: جایی که اون حمله پنیک بهم دست داد و با گریه فرار کردم.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: صبر کن آدمیزاد، ممکنه داریم اذیتش می‌کنیم.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: آخ، نمی‌خوام تو رودربایستی قرارت بدم!

`publish("act4", ["hong_to_alshire",4]);`

h2: فقط یه چهره آشنا یادم اومد، همین.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: آآآآآآآه میدونستم! اون یه روانی خطرناک و وحشت‌ناکه!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s:  آآآآه اولین تاثیری که گذاشتیم "شاهد ترومای من بودی" بود! این یعنی از ما متنفرن!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: آآآآه باعث شدیم یکی یه اتفاق تروماتیک رو به یاد بیاره. صرف حضور ما به دیگران آسیب میزنه.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: صبر کن آدمیزاد، به نظر ناراحت میاد.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: آخ، البته فشاری روت نیست!

`publish("act4", ["hong_to_alshire", 4]);`

h2: فقط میگم، اگه میخوای میتونی اینجا بشینی.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s:  اون زیادی دوستانه رفتار می‌کنه! مثل تد باندی، قاتل زنجیره‌ای!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: اونا فقط دارن نقش آدمای خوب رو بازی می‌کنن! هیچکس *واقعاً* نمیخواد به ما نزدیک بشه!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: آآآه ما همیشه باعث میشیم دیگران احساس معذب بودن بکنن! ما یه لکه ننگ روی زمینیم!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: صبر کن آدمیزاد، ممکنه داریم اذیتش می‌کنیم.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2:  آخ، نمی‌خوام بی‌ادبی کنم!

`publish("act4", ["hong_to_alshire", 6]);`

h2: فقط یه کم وقت لازم دارم تا احساساتم رو پردازش کنم. لطفاً اینو به عنوان یه طرد شخصی برداشت نکن.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s:  چه افکار مریض و پیچیده‌ای رو دارن پردازش می‌کنن؟! چه امیال تاریکی قلب این روانی رو پر کرده؟!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: مارو شخصا رد کرد، هیچوقت هیچکس مارو دوست نداره!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: ما پردازش احساسی‌شون رو قطع کردیم! حالا تا ابد تروماتیزه میشن و همه‌ش تقصیر ماست!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن فرار کن

```
Game.clearText();
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["alshire", 10]);
sfx("pop");
```

(...1001)

```
publish("act4", ["alshire", 11]);
sfx("alshire_run");
```

(...2601)

```
publish("act4-out-3");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
```

(...1201)

`publish("act4-jumpcut-hong");`

h: هوم. عجیب بود. کنجکاوم بدونم تو سرش چی میگذشت.

`publish("act4", ["hong_closer", 2]);`

h: به هر حال، داشتی میگفتی؟

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b:  اوه، یادم رفت؟ یه چیزی در مورد تیم‌ها و کار؟

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: میگن باید با احساساتت "صلح کنی"، انگار که احساساتت *جنایتکار جنگی* هستن.

`publish("act4", ["bb_closer", 7]);`

b: اما من میخوام ما *بیشتر* از یه صلح ساده برقرار کنیم! من میخوام ما *متحد* باشیم!

`publish("act4", ["bb_closer", 3]);`

b: من میخوام یه سگ نگهبان خوب باشم. درست مثل اینکه گرسنگی و تشنگی هشدارهایی برای نیازهای فیزیکی تو هستن،

`publish("act4", ["bb_closer", 8]);`

b: من میخوام هشدار برای نیازهای *روانی* تو باشم – نیازهای تو برای امنیت، تعلق، و خوب بودن.

`publish("act4", ["bb_closer", 1]);`

b: اما... من تو کارم افتضاحم، پس لازمه که تو منو تربیت کنی.

`publish("act4", ["bb_closer", 4]);`

b: من "همیشه معتبر" نیستم، و "همیشه غیرمنطقی" هم نیستم. من فقط... دارم تمام تلاشمو می‌کنم. پس، لطفاً،

`publish("act4", ["bb_closer", 30]);`

b: کمکم کن تا کمکت کنم!

`publish("act4", ["bb_closer", 6]);`

b: هرچند، یاد دادن ترفندهای جدید به یه سگ پیر *زمان* می‌بره. شاید *سال‌ها*.

`publish("act4", ["bb_closer", 3]);`

b:  و بعضی وقتا دوباره برمی‌گردم، به عادت‌های قدیمیم دچار میشم.

`publish("act4", ["bb_closer", 2]);`

b: به سایه‌ها پارس می‌کنم. با کلمات می‌ترسونمت. حتی ممکنه چندتا تصویر مزاحم از... چیزا بهت نشون بدم.

`publish("act4", ["bb_closer", 9]);`

b: متاسفم! من یه سگ پناهگاهی آسیب‌دیده‌ام! سگ‌های آسیب‌دیده بعضی وقتا رو تختت خرابکاری می‌کنن!

`publish("act4", ["bb_closer", 4]);`

b: اما اگه با من صبور باشی... و فقط بمونی و کنارم بشینی...

`publish("act4", ["bb_closer", 8]);`

b: شاید بتونی این گرگ رو رام کنی.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[سگ خوب.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[آدم خوب.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

# act4f-pat-hong

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 13]);
```

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...501)

`publish("act4", ["bb_closer", 13]);`

(...501)

`publish("act4", ["bb_closer", 14]);`

(...6501)

`publish("act4", ["bb_closer", 15]);`

(...1001)

(#act4f)

# act4f-pat-bb

```
Game.clearText();
publish("hide_tabs");
Game.FORCE_CANT_SKIP = true;
music(null,{fade:0.5});
sfx("youbothwin");
```

```
publish("act4", ["hong_closer", 4]);
publish("act4", ["bb_closer", 10]);
```

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...501)

`publish("act4", ["bb_closer", 10]);`

(...501)

`publish("act4", ["bb_closer", 11]);`

(...6501)

`publish("act4", ["bb_closer", 12]);`

(...1001)

(#act4f)

# act4f

```
Game.FORCE_CANT_SKIP = false;
publish("act4", ["bb_closer", 16]);
publish("act4", ["hong_closer", 5]);
```

{{if _.fifteencigs}}
b: آآآآآ هنوز داری تنها غذا می‌خوری پونزده تا سیگار آآآآآ
{{/if}}

{{if _.parasite}}
b: آآآآآ هنوز موقع غذا خوردن بازدهی نداری ما انگل‌ جامعه‌ایم آآآآآ
{{/if}}

{{if _.whitebread}}
b: آآآآآ داری بیشتر نون سفید می‌خوری آآآآآ
{{/if}}

```
publish("act4", ["bb_closer", 18]);
publish("act4", ["hong_closer", 6]);
sfx("yaps", {volume:0.6});
Game.FORCE_CANT_SKIP = true;
Game.WORDS_HEIGHT_BOTTOM = 205;
Game.FORCE_TEXT_DURATION = 90;
Game.FORCE_NO_VOICE = true;
```

b: وَق وَق وَق وَق وَق

(#credits)
