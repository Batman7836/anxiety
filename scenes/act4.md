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

h: No, you're right.

h: "Social skills" mean nothing if we don't genuinely care *for* people.

`hong({ body:"normal" });`

h: Basically, just don't be a ^dick^.

`bb({ eyes:"annoyed", mouth:"smile" });`

b: That's a motivational poster caption right there.

`hong({ body:"shrug", mouth:"narrow" });`

h: “Don't Be A ^Dick^™”

(#act4_something_else)

# act4_alone_skills_manipulated

`bb({ eyes:"angry" })`

b: We'll become a Welcome doormat, saying Please and Thank You as people wipe their feet on us!

`bb({ mouth:"scream", eyes:"scream" })`

b: We'll kiss so much butt, it'll look like we're wearing brown lipstick!

```
bb({ mouth:"normal", eyes:"normal" });
hong({ body:"chin" });
```

h: Nah, you're right. "Social skills" can't be just about pleasing others, it's also got to be about setting *boundaries.*

`hong( body:"one_up" });`

h: We can't invite others into our home, if we have no walls to hold up our home.

```
hong({ eyes:"angry", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Also... re: that lipstick mental image... *ew??*

(#act4_something_else)

# act4_alone_skills_fail

`bb({ eyes:"annoyed" });`

h: We might fail. Actually, we *will* fail.

```
bb({ eyes:"normal" });
hong({ eyes:"surprise", body:"shrug" });
```

h: And that's fine! Failing is how anyone learns anything new at first!

`hong({ body:"normal", eyes:"normal" });`

h: So let's fail forward together, yeah?

`bb({ eyes:"normal_r" });`

b: Sure, I guess... worst-case scenario, we can just skip town and get a new identity.

`bb({ eyes:"normal" });`

h: Yeah I think that only costs two bitcoins these days.

(#act4_something_else)

# act4_alone_experiment

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: We could try some experiments!

`hong({ body:"chin" });`

h: We could ping a friend to hang out, reconnect with an old pal, or even just chat with a barista.

`hong({ body:"normal" });`

h: I think we may find we're more likeable than we suspect.

`bb({ eyes:"annoyed" });`

[What if these are small, cheap "wins"?](#act4_alone_experiment_cheap)

[What if this is a burden to others?](#act4_alone_experiment_burden)

[But small talk isn't the *real* us!](#act4_alone_experiment_real_us)

# act4_alone_experiment_real_us

`bb({ eyes:"sad" });`

b: If we put on a shallow smile, we'll never really connect with anyone,

`bb({ eyes:"super_sad" });`

b: *But* if we open up, other people will see all our messed-up insides!

`hong({body:"chin", mouth:"narrow", MOUTH_LOCK:true})`

h: ...

```
hong({body:"normal", mouth:"normal"});
bb({eyes:"normal"});
```

h: Roll over.

b: What.

`hong({body:"hands_1"})`

h: When dogs want to show love and trust, they make themselves vulnerable by exposing their belly.

`hong({body:"one_up"})`

h: Maybe we're not *yet* secure enough to be too vulnerable, but with enough training,

`hong({body:"normal", eyes:"surprise"})`

h: One day we can show people the real us – all messed-up, all human.

```
hong({eyes:"normal"});
bb({ eyes:"super_sad", mouth:"smile", body:"chest" });
```

b: I'll roll over if you give me a treat.

`bb({ eyes:"normal", mouth:"normal" });`

h: No.

(#act4_something_else)


# act4_alone_experiment_cheap

b: Saying "hi" to the barista isn't exactly gold-medal performance in the Social Butterfly Olympics.

```
hong({ body:"point", eyes:"surprise" });
bb({ eyes:"normal" });
```

h: It is for *us!*

`hong({ body:"one_up", eyes:"annoyed" });`

h: In the social arena, we're not even featherweight class, we're like... quark-weight.

`hong({ body:"normal", eyes:"normal" });`

h: If we have to start with small, cheap wins, so be it. Gotta climb the 1st step before the 1000th step.

b: Yeah! Maybe after saying "Hi", we can advance to saying...

`bb({ body:"two_up", mouth:"smile", eyes:"smile_u" });`

b: *"How are you?"*

`hong({ body:"shrug", mouth:"smile", eyes:"surprise_l" });`

h: *"Not much!"*

(#act4_something_else)

# act4_alone_experiment_burden

`bb({ eyes:"suspect_r" })`

b: Maybe the barista just wants to make some dang coffee, not be an *experiment* to see if our social skills suck.

`bb({ eyes:"annoyed" })`

h: Well, if it turns out we *are* being a burden...

```
hong({ eyes:"surprise" });
bb({ eyes:"normal" });
```

h: That's good to know, too!

`hong({ eyes:"normal" });`

h: We can then learn how to pro-actively ask people what they're comfortable with, to know and respect others' boundaries.

```
hong({ eyes:"annoyed_l", mouth:"narrow" });
bb({ eyes:"annoyed", mouth:"smile" });
```

h: Y'know, all that "inter-personal skills" ^crap^ we see in counselor brochures.

(#act4_something_else)



# act4_bad

```
_.a4_talked_about_bad = true;
_.a4_fears_discussed += 1;
```

`bb({ eyes:"annoyed_r" })`

b: I want to defend your moral needs, that drive to become a better person,

`bb({ eyes:"sad_d" })`

b: But it just feels like deep down, we're so fundamentally... broken.

`bb({ body:"two_up", eyes:"angry" })`

{{if _.INJURED}}
b: And don't tell me we're *not* messed up. We jumped off a *roof*.
{{/if}}

{{if !_.INJURED}}
b: And don't tell me we're *not* messed up. We almost jumped off a *roof*.
{{/if}}

`bb({ body:"normal", eyes:"sad" })`

{{if _.a4_fears_discussed==1}}
b: I dunno, enough of *me* choosing what to say next. What do *you* say, human?
{{/if}}

{{if _.a4_fears_discussed==2}}
b: Again, back to you, human. What do you think?
{{/if}}

{{if _.a4_fears_discussed==3}}
b: More thoughts, human?
{{/if}}

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[So we're broken. Let's fix us.](#act4_bad_fix)

[So we're broken. Let's accept it.](#act4_bad_accept)

[Thank you.](#act4_thanks) `_.thanks_for = "moral well-being";`

# act4_bad_fix

```
bb({eyes:"normal"});
hong({body:"chin"});
```

h: We could slowly build better habits, get our life more in line with what we value,

`hong({body:"one_up"});`

h: And if needed, we could get professional help – a therapist or counsellor.

`hong({body:"normal"});`

h: There's ways to fix us.

[What if we can't fix it all?](#act4_bad_fix_cant)

[What if we fix *too* much?](#act4_bad_fix_too_much)

[We can't afford professional help.](#act4_bad_fix_afford)

# act4_bad_fix_cant

`hong({eyes:"annoyed"});`

h: Nah, I guess you're right.

h: We can't fix it all.

`bb({mouth:"scream", eyes:"scream_sad"});`

b: Ahhh I knew it we'll always be broken!

`hong({eyes:"surprise"});`

h: But we can at least be *less* broken.

```
bb({mouth:"normal", eyes:"annoyed"});
hong({eyes:"sad", mouth:"smile"});
```

h: Scars heal with time, but they never go away. And that's okay.

`bb({eyes:"annoyed_r"});`

b: I guess. Besides,

```
Game.FORCE_TEXT_Y = 460;
Game.clearText();
publish("act4-sexy", [true]);
```

b: Scars are *sexy.*

```
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-sexy", [false]);
bb({body:"chest", mouth:"smile_talk", MOUTH_LOCK:true, eyes:"sexy"}, 0);
hong({eyes:"normal", mouth:"normal"}, 0);
```

h: Please do not do that.

(#act4_something_else)

# act4_bad_fix_too_much

`bb({ eyes:"angry_d" })`

b: This feels sick to admit, but... some part of me *wants* to have this disorder.

`bb({ eyes:"angry" })`

b: I mean, without it, won't we be *boring?*

`bb({ eyes:"sad_r", body:"one_up" })`

b: Without the disorder, won't our art become stale and bland?

`bb({ eyes:"sad_u", body:"two_up" })`

b: Without the disorder, won't we be unable to connect with our friends who have the disorder?

`bb({ eyes:"sad", body:"chest" })`

b: If we're ever content with life, won't we stop driving ourselves to do great things?

`hong({ MOUTH_LOCK:true })`

h: ...

h: If we even fear... "running out of fears"...

h: I don't think we're gonna run out of fears.

`bb({ eyes:"smile_u", body:"normal", mouth:"smile" })`

b: Oh, yeah! Whew! What a relief!

(#act4_something_else)

# act4_bad_fix_afford

`bb({ body:"one_up", eyes:"sexy", mouth:"normal" })`

b: "Doc, I'm anxious that I'm paying $100/hr just to hear you ask *how does that make you feel?*"

`bb({ body:"paw", eyes:"closed", mouth:"narrow" })`

b: "Mm-hmm. And how does that make you feel?"

```
bb({ body:"normal", eyes:"normal", mouth:"normal" });
hong({ eyes:"sad" });
```

h: Nah, that's a totally reasonable worry.

`hong({ eyes:"annoyed", mouth:"sad" });`

h: And it genuinely sucks that mental healthcare isn't affordable for lots of folks.

`hong({ eyes:"normal", mouth:"normal" });`

h: Still, there are some cheap or free options:

`hong({ body:"chin" })`

h: Support groups, online therapy, student/non-profit health centers...

`hong({ body:"hands_1" })`

h: Building habits like meditation, sleeping well, chatting regularly with friends, learning new things...

`hong({ body:"hands_2" })`

h: Going to a library to borrow workbooks for evidence-based psychotherapies...

`hong({ body:"one_up" })`

h: There's a full list of resources at the end of this game!

```
hong({ body:"normal" });
bb({ eyes:"annoyed", mouth:"narrow" });
```

b: Well *that* fourth wall didn't last long.

`hong({ body:"point" });`

h: Some things are more important than narrative convention. Such as mental health.

(#act4_something_else)


# act4_bad_accept

```
bb({ eyes:"normal" });
hong({ eyes:"normal_l", body:"one_up", mouth:"narrow" });
```

h: I mean, that's what therapists say right? Accept all your emotions, even the negative ones?

```
bb({ eyes:"annoyed" });
hong({ eyes:"normal", body:"normal", mouth:"normal" });
```

b: Wait.

["Accept" as in *give up*?](#act4_bad_accept_give_up)

["Accept" as in *approve*?](#act4_bad_accept_approve)

["Accept" as in *take literally*?](#act4_bad_accept_literally)

# act4_bad_accept_give_up

`bb({ eyes:"angry", body:"one_up" });`

b: Do you think Martin Luther King would've said, "Shucks we can't sit in the front of the bus, let's just *accept* it?"

`bb({ eyes:"angry_r", body:"two_up" });`

b: Why does the Self-Help Industrial Complex think waving the white flag is some *profound wisdom?*

`bb({ eyes:"annoyed", body:"normal" });`

h: I think therapists mean "accept" bad things as in: acknowledging they exist and are hard to change,

h: But not necessarily giving up a commitment to change.

`bb({ eyes:"suspect" });`

b: Then therapists should say *acknowledge*, not *accept*.

`hong({ body:"chin", eyes:"annoyed" });`

h: Yeah come to think of it, "accept" is kinda confusing.

`bb({ eyes:"closed", mouth:"narrow" });`

b: Well, I *acknowledge* that.

(#act4_something_else)

# act4_bad_accept_approve

`bb({ eyes:"angry" });`

b: Like it's *good* that we're broken or something? No!

`bb({ eyes:"angry_r", body:"one_up" });`

b: All those dang Hollywood screenwriters who romanticize mental illness are full of crud!

`bb({ eyes:"angry", body:"two_up" });`

b: Having a mental disorder *sucks!* It robs people of *lives!* Why should we "accept" that?!

`bb({ body:"normal" });`

h: I think therapists mean "accept" our emotions as in: be patient with them.

```
hong({ body:"one_up" });
bb({ eyes:"normal" });
```

h: Like how struggling in quicksand makes you sink faster, and the solution is to patiently lie flat,

`hong({ eyes:"surprise" });`

{{if _.INJURED}}
h: Fighting against you, my fear, led me to jump off a roof.
{{/if}}

{{if !_.INJURED}}
h: Fighting against you, my fear, almost led me to jump off a roof.
{{/if}}

`hong({ body:"normal", eyes:"normal" });`

h: Instead, the solution is to do what we're doing now – not to fight, but to patiently be with each other.

`bb({ eyes:"annoyed" });`

b: Then they should say *that* instead of some problematic word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: Yeah come to think of it, "accept" kind of sucks.

`bb({ eyes:"closed_annoyed", mouth:"narrow" });`

b: I do not accept "accept".

(#act4_something_else)

# act4_bad_accept_literally

`bb({ eyes:"sad", body:"one_up" });`

b: But we already *know* you shouldn't take me literally!

`bb({ eyes:"sad_u", body:"two_up" });`

b: The whole *problem* is that I want to help you, but I suck at using words to do so!

`bb({ eyes:"sad", body:"normal" });`

h: I think therapists mean "accept" your emotions as in: "don't fight or ignore them."

`hong({ eyes:"surprise", body:"one_up" });`

h: To listen to you, work *with* you, but not take what you say as 100% literal truth.

```
hong({ eyes:"normal", body:"normal" });
bb({ eyes:"annoyed", mouth:"normal" });`
```

b: Then therapists should say *that* instead of some vague confusing word like "accept".

`hong({ body:"chin", eyes:"annoyed" });`

h: I guess they suck at using words, too.

(#act4_something_else)




# act4_something_else

```
bb({ body:"normal", mouth:"normal", eyes:"normal" });
hong({ body:"normal", mouth:"normal", eyes:"normal" });
```

{{if _.a4_fears_discussed==1}}
h: Anyway, anything else you wanna chat about?
{{/if}}

{{if _.a4_fears_discussed==2}}
h: So, anything else on your heavy heart?
{{/if}}

{{if _.a4_fears_discussed==3}}
(#act4_something_else_2)
{{/if}}

{{if _.a4_talked_about_harm!=true}}
[I'm scared we'll be harmed.](#act4_harm)
{{/if}}

{{if _.a4_talked_about_alone!=true}}
[I'm scared we'll be alone.](#act4_alone)
{{/if}}

{{if _.a4_talked_about_bad!=true}}
[I'm scared we're bad people.](#act4_bad)
{{/if}}

[Nah, I'm good for now.](#act4c_prelude)

# act4_something_else_2

h: Okay, I think we've talked about all our fears now.

b: Yes, there are only three fears.

h: Yup, exactly three.

b: Convenient.

(#act4c)

# act4c_prelude

h: Good chat, team.

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

b: This isn't some *game*, you know.

`bb({eyes:"angry_d", body:"one_up"})`

b: Building a healthy relationship with your emotions isn't as simple as clicking buttons on a screen.

`bb({eyes:"sad", body:"normal"})`

b: *Can* we really get along?

b: *Can* we work together, as a team?

`hong({eyes:"sad", body:"one_up"})`

h: Well,

```
hong({eyes:"surprise_l"});
bb({eyes:"normal"});
```

a: E-excuse me...

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

a: W-wo-would you mind if I sat with you for lunch?

`publish("act4", ["alshire", 1]);`

{{if _.TOP_FEAR=="harm"}}
s: *This* is your crush? Why are they sitting alone like a psycho serial killer?
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: Asking your crush if you can sit with them? Do you know how *needy* we sound?!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: *This* is your crush? We interrupted their peace and quiet! We're such a burden!
{{/if}}

`publish("act4", ["alshire", 2]);`

a: I- I mean- it's, it's okay if not, I just...

`publish("act4", ["alshire", 3]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "h2"`

[Wait, didn't I see you at the party?](#act4d_recognition) `publish("act4", ["hong_to_alshire",1])`

[Yeah, of course! Come here.](#act4d_yes) `publish("act4", ["hong_to_alshire",2])`

[Sorry, I need alone time right now.](#act4d_no) `publish("act4", ["hong_to_alshire",8])`

# act4d_recognition

`publish("act4", ["hong_to_alshire",2]);`

h2: Yeah you were on the couch! At the first party I went to...

`publish("act4", ["hong_to_alshire",10]);`

{{if _.a2_ending=="fight"}}
h2: Where I had that panic attack and punched the host.
{{/if}}

{{if _.a2_ending=="flight"}}
h2: Where I had that panic attack and ran out crying.
{{/if}}

```
publish("act4", ["hong_to_alshire", 0]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to put you on the spot!

`publish("act4", ["hong_to_alshire",4]);`

h2: Just remembering a friendly face, is all.

```
publish("act4", ["hong_to_alshire",5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: AHHHHH I KNEW IT! THEY'RE A DANGEROUS PANIC-DRIVEN PSYCHO!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: AAHHH THE FIRST IMPRESSION WE MADE WAS "WITNESSED MY TRAUMA"! THAT MEANS THEY HATE US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AAAHHH WE MADE SOMEONE REMEMBER A TRAUMATIC EVENT. OUR MERE PRESENCE HURTS OTHERS.
{{/if}}

(#act4e)

# act4d_yes

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, they seem uncomfortable.

```
publish("act4", ["hong_to_alshire", 6]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, no pressure of course!

`publish("act4", ["hong_to_alshire", 4]);`

h2: Just saying, you can sit here if you want to.

```
publish("act4", ["hong_to_alshire", 5]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: THEY'RE BEING *TOO* FRIENDLY! LIKE TED BUNDY, THE SERIAL KILLER!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: THEY'RE JUST ACTING NICE! NO ONE *REALLY* WANTS TO BE CLOSE TO US!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: AHHH WE ALWAYS MAKE OTHERS FEEL AWKWARD! WE'RE A STAIN UPON THE EARTH!
{{/if}}

(#act4e)

# act4d_no

```
publish("act4", ["hong_to_alshire", 9]);
publish("act4", ["bb_to_alshire", _.INJURED ? 3 : 1]);
```

b: Hang on human, we may be making them uncomfortable.

```
publish("act4", ["hong_to_alshire", 3]);
publish("act4", ["bb_to_alshire", _.INJURED ? 2 : 0]);
```

h2: Ah, I don't mean to be rude!

`publish("act4", ["hong_to_alshire", 6]);`

h2: I just need some time to process my emotions. Please don't take it as a personal rejection.

```
publish("act4", ["hong_to_alshire", 7]);
publish("act4", ["alshire", 4]);
```

{{if _.TOP_FEAR=="harm"}}
s: WHAT SICK, TWISTED THOUGHTS ARE THEY PROCESSING?! WHAT DARK DESIRES FILL THIS PSYCHO'S HEART?!
{{/if}}

{{if _.TOP_FEAR=="alone"}}
s: WE'VE BEEN PERSONALLY REJECTED! WE'LL NEVER BE LOVED!
{{/if}}

{{if _.TOP_FEAR=="bad"}}
s: WE INTERRUPTED THEIR EMOTIONAL PROCESSING! NOW THEY'LL BE TRAUMATIZED FOREVER AND IT'S ALL OUR FAULT!
{{/if}}

(#act4e)

# act4e

```
Game.WORDS_HEIGHT_BOTTOM = 195;
publish("act4", ["alshire", 6]);
```

s: RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN RUN

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

h: Huh. That was weird. I wonder what was going on in their head.

`publish("act4", ["hong_closer", 2]);`

h: Anyway, you were saying?

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 6]);
```

b: Uh, I forget? Something about teams and work?

```
publish("act4", ["bb_closer", 0]);
publish("act4", ["hong_closer", 3]);
```

h: ¯\_(ツ)_/¯

```
publish("act4", ["hong_closer", 1]);
publish("act4", ["bb_closer", 4]);
```

b: They say you should "make peace" with your emotions, as if your emotions are *war criminals*.

`publish("act4", ["bb_closer", 7]);`

b: But I want us to make *more* than mere peace! I want us to be *allies!*

`publish("act4", ["bb_closer", 3]);`

b: I want to be a good guard-dog. Just like how hunger & thirst are alarms for your physical needs,

`publish("act4", ["bb_closer", 8]);`

b: I want to be the alarm for your *psychological* needs – your needs for safety, belonging, goodness.

`publish("act4", ["bb_closer", 1]);`

b: But... I suck at my job, so I need you to train me.

`publish("act4", ["bb_closer", 4]);`

b: I'm not "always valid," nor "always irrational." I'm just... trying my best. So, please,

`publish("act4", ["bb_closer", 30]);`

b: Help me help you!

`publish("act4", ["bb_closer", 6]);`

b: Though, teaching an old dog new tricks *will* take a while. Maybe *years.*

`publish("act4", ["bb_closer", 3]);`

b: And sometimes I'll relapse, I'll slip into my old habits.

`publish("act4", ["bb_closer", 2]);`

b: I'll bark at shadows. I'll scare you with words. I might even show you some intrusive images of... things.

`publish("act4", ["bb_closer", 9]);`

b: I'm sorry! I'm a battered shelter dog! Battered dogs poop on your bed sometimes!

`publish("act4", ["bb_closer", 4]);`

b: But if you're patient with me... and just stay and sit with me...

`publish("act4", ["bb_closer", 8]);`

b: Maybe you can tame this wolf.

`publish("act4", ["bb_closer", 0]);`

`Game.clearText();`

(...1000)

`Game.OVERRIDE_CHOICE_SPEAKER = "h"`

[Good dog.](#act4f-pat-bb) `Game.OVERRIDE_CHOICE_SPEAKER = "h"; publish("act4", ["hong_closer", 2]);`

`Game.OVERRIDE_CHOICE_SPEAKER = "b"`

[Good human.](#act4f-pat-hong) `Game.OVERRIDE_CHOICE_SPEAKER = "b"; publish("act4", ["bb_closer", 8]);`

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
b: AAAAA YOU'RE STILL EATING ALONE FIFTEEN CIGARETTES AAAAA
{{/if}}

{{if _.parasite}}
b: AAAAA YOU'RE STILL NOT PRODUCTIVE WHILE EATING WE'RE SOCIETY-PARASITES AAAAA
{{/if}}

{{if _.whitebread}}
b: AAAAA YOU'RE EATING MORE WHITE BREAD AAAAA
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

b: YAP YAP YAP YAP YAP

(#credits)
