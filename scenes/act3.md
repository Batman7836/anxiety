# act3

```
SceneSetup.act3();
Game.WORDS_HEIGHT_BOTTOM = 205;
sfx("cheers");
```

r: نوش!

```
publish("act3",["roofhunter",1]);
publish("act3",["roofhong",1]);
sfx("drinking");
```

(...4001)

```
publish("act3-alpha", ["dizzyhunter",1]);
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",3]);
```

h2: *آخیش* چسبیدا.

```
publish("act3",["roofhunter",2]);
publish("act3",["roofhong",2]);
```

r: می‌دونی، بچه جون...

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",6]);
```

h2: مخصوصا به آمیگدال های چپ و راستم چسبید.

```
publish("act3",["roofhunter",8]);
publish("act3",["roofhong",5]);
```

r: تو منو یاد خودم می‌ندازی وقتی که جوون بودم. وقتی که حیوون درونم منو شکنجه می‌کرد.

```
publish("act3",["roofhunter",9]);
publish("act3",["roofhong",2]);
```

r: خیلی خوشحالم که می‌تونم. این لطف رو در حقت بکنم و بهت کمک کنم دیو درونت رو همونجوری که من مال خودمو کشتم بکشی.

```
publish("act3",["roofhunter",2]);
```

r: هی، یه سوال، جرعت یا حقیق--

```
publish("act3",["roofhunter",3]);
publish("act3",["roofhong",7]);
publish("act3-alpha", ["dizzyhong",0]);
```

h2: جرعت!

```
publish("act3-alpha", ["dizzyhong",1]);
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",2]);
```

r: هاها! خوبه.

```
publish("act3",["roofhunter",21]);
publish("act3",["roofhong",4]);
```

r: خب. اون استخر شنا رو اون پاییین می‌بینی؟

```
publish("act3-alpha", ["dizzyhong",0]);
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",9]);
```

h2: آره؟ همون که شیش طبقه پایینه؟

```
publish("act3",["roofhunter",10]);
publish("act3",["roofhong",8]);
```

r: بپر توش.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",10]);
```

h2: ...

```
publish("act3",["roofhong",11]);
```

h2: صبر کن بینم، چی؟

```
publish("act3",["roofhong",10]);
publish("act3",["roofhunter",2]);
```

r: حیوونه شروع کرده به غر زدن مگه نه؟

```
publish("act3",["roofhunter",23]);
```

r: *وااای نهههه خطرناکه، نکنی یوقت.*

```
publish("act3",["roofhunter",22]);
```

r: ولی این دقیقا دلیلیه که ما ماید این کارای پرهیجان مرگبار رو انجام بدیم! در لحظه زندگی کن!

```
publish("act3",["roofhunter",10]);
```

r: به اون حیوون نشون بده که غر زدنش به چپمون هم نیست! بپر توش.

```
publish("act3",["roofhunter",11]);
publish("act3",["roofhong",13]);
```

h2: آم، ولی بعضی وقتا... حق با ترسه...

```
publish("act3",["roofhunter",5]);
publish("act3",["roofhong",12]);
music(null, {fade:2});
```

r: ...

```
publish("act3-alpha", ["dizzyhunter",0]);
publish("act3",["roofhunter",6]);
publish("act3",["dd",1]);
```

r: ببخشید، نکنه دوباره گول تبلیغات اون کتابای حضور در لحظه (ذهن آگاهی) رو خوردی که میگن احساسات بد درواقع *خوبن*؟

```
publish("act3",["roofhunter",17]);
```

r: اون ^کونی^ هایی که این دنیا رو میچرخونن به بقیه *ما* ها اضطراب و افسردگی میدن.

```
publish("act3",["roofhunter",18]);
```

r: بعدم تو سخنرانی هاشون بهمون میگن که *کیر* خوردن رو قبول کنیم و اون دیو سادیسمی تو کلمون رو بپذیریم.

```
publish("act3",["roofhunter",6]);
```

r: ببین بچه‌جون، من می‌دونم که *تو* می‌دونی اون حیوون به افردای مثل ما صدمه میزنه. افرادی مثل ما رو *شکنجه* می‌کنه.

```
publish("act3",["roofhunter",19]);
```

r: اون دوست ما نیست. اون یه دیو هاره، که یا باید *بیهوش* بشه،

```
publish("act3",["roofhunter",20]);
```

r: یا *یه گلوله بخوره تو سرش*

```
publish("act3",["roofhunter",27]);
```

r: وگرنه، تو بهش اجازه میدی که ببره.

```
publish("act3",["roofhunter",31]);
publish("act3",["roofhong",14]);
publish("act3",["dd",2]);
```

h2: نه. تو اشتباه می‌کنی.

```
publish("act3",["roofhunter",13]);
publish("act3",["roofhong",15]);
music('battle_dark', {volume:1.0}, function(){
	music('battle_dark_loop');
});
```

h2: من بهش اجازه نمیدم ببره.

```
publish("act3",["roofhunter",25]);
publish("act3-alpha", ["roofhong",0]);
publish("act3-alpha", ["transition",1]);
publish("act3",["dd",6]);
```

r: همینه! من بهت ایمان دارم! بکشش!

(#act3a)



# act3a

```
Game.clearText();
publish("act3-out");
Game.WORDS_HEIGHT_BOTTOM = -1; /* reset */
_.act3_bb_body = 1;
```

(...1500)

```
publish("hp_show");
```

b: نه نه نه نه نه

n: این قسمت دوتا پایان ممکن داره و یکیشون *خیلی خیلی بده!*

b: نه نه نه نه نه نه نه نه 

n: بادقت انتخاب کن. از انسانت محافظت کن.

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: واااااااای

`bb({ mouth:"normal" });`

n: موفق باشی.

```
Game.clearText();
bb({ eyes:"start" });
```

[انسان، دیگه واقعا اینجا می‌تونی بمیری!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[این کار احمقانه و خود تخریبیه!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[اون روان‌پریش ها واقعا دوستات نیستن!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ا--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ا--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: ا--

(#act3a_after)

# act3a_after

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: میدونی چیه، من شاید باورت می‌کردم...اگه هزار بار دیگه همین حرفا رو نزده بودی.

h: تو شدی عین چوپان دروغگو.

```
bb({ eyes:"sad" });
```

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_harm"`

[](#act3_fork) `_.SPECIAL_ATTACK="harm"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_alone"`

[](#act3_fork) `_.SPECIAL_ATTACK="alone"; Game.OVERRIDE_CHOICE_LINE=true`

`Game.OVERRIDE_CHOICE_SPEAKER = "fear_bad"`

[](#act3_fork) `_.SPECIAL_ATTACK="bad"; Game.OVERRIDE_CHOICE_LINE=true`


# act3_fork

```
Game.clearText();
bb({body:"special_attack"});
sfx("charging");
Game.FORCE_CANT_SKIP = true;
```

(...1001)

```
Game.FORCE_CANT_SKIP = false;
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: قبلا اونم امتحان کردی.

b: انسان، لطفا...

`hong({ eyes:"look_right" });`

h: اوه *ببخشید* که صنعت داروسازی خود درمانی منو قبول نداره.

h: ببین ^کونی^، ما *هممون* یه راهی برای خفه کردن تو داریم.

`hong({ body:"look_up", eyes:"look_up" });`

h: بعضیا سرشون رو با کار شلوغ می‌کنن.

`hong({ body:"look_down", eyes:"look_down" });`

h: بعضیا وقتشون رو با سکس، مواد زدن و چک کردن اینستا تلف می‌کنن.

`hong({ body:"normal", eyes:"look_right" });`

h: بعضیا هم خودشون رو به یکی دیگه می‌چسبونن.

`hong({ eyes:"angry" });`

h: منم میخوام خودمو بندازم تو این استخر.

[تو مستی و اون شیش طبقه پایینه!](#act3_bad_1_harm)

[هعی، اینجوری از من تشکر می‌کنی؟!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[باشه، قبول دارم، من گند زدم.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: حتی اگرم تو استخر بی‌افتی، کشش سطحی آب دنده هات رو خرد می‌کنه و در بهترین حالت ضربه مغزیت می‌کنه!

h: اه.

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

h: یبار دیدم یه مرد روسی تو یوتوب این کارو کرد.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: چ- ببخشیدا، تشکر کنم؟

`bb({ eyes:"angry" });`

b: این دقیقا دلیلیه که من وجود دارم! انسان نمی‌تونن از خودشون محافظت کنن!

b: من تو کل عمرم سعی کردم تو رو از خطر حفظ کنم ولی الان میخوا--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)

# act3_good_1

`hong({ body:"laugh_1" })``

h: هه.

`hong({ body:"laugh_2" })``

h: هههه.

`hong({ body:"laugh_3" })``

h: هههههههههه

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: ای وای، خردنمایی از این بدتر تو کل قرن نداشتیم!

`hong({ body:"yell_2" });`

h: آره، تو ^گه^ صفت با اون پشمای قرمزت معلومه که گند زدی!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: چیز دیگه ای نداری بگی، کاپیتان واضح گو؟

[ولی انتخاب گرفتن از من راهش نیست.](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[اما این بار *واقعا* حق با منه.](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[من بهت آسیب زدم.](#act3_good_2a)


# act3_good_1_fail_revenge

b: تو باید رابطه بهتری با احساساتت داشته باشی، نکه همش بخوای با اون زهر مار--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)



# act3_good_1_fail_harm

b: پس لطفا، اون بطری رو بذار زمین--

```
hong({body:"drink"});
bb({body:"attacked"});
attackBB("32p");
_.act3_bb_body++;
```

(...2000)

```
hong({ body:"normal", mouth:"angry", eyes:"angry" });
bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });
```

(#act3_bad_2)




# act3_bad_2

`bb({ eyes:"sad" });`

b: لطفا... نکن...

h: مثل اینکه جونت خیلی داره کم میشه، گرگی.

h: اگه من جات بودم، حرف های بعدیت رو بادقت انتخاب می‌کردم.

`bb({ eyes:"normal" });`

[باشه. دیگه از محافظت ازت خسته شدم.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[همه این مدت حق با من بود.](#act3_bad_2_right)

[من متاسفم.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: پس، برو دیگه بپر. ببین اگه من اهمیت دادم.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: باشه دیگه! به سلامتی!

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: نه صب کن داشتم از روانشناسی معکوس استفاده می‌کردم. تو باید *برعکس* هر چی که گفتم رو انجام می‌دادی!

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: تو *داری* خودتو تو معرض خطر قرار می‌دی. اینایی که مثلا دوستاتن *دارن* ازت سوءاستفاده می‌کنن. و تو‌ هم *داری* از اونا سوءاستفاده می‌کنی.

`bb({ eyes:"sad" });`

b: پس لطفا، انسان... چرا به حرفم گوش نمیدی؟

h: چون تو هیچوقت به *من* باور نداشتی.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: گرگ های نگهلان دیگه انسان هایی دارن که از وقتشون می‌زنن تا صبورانه تربیتشون کنن، تا *یاد بگیرن* چطوری باهم کار کنن،

b: بجای اینکه از گرگ نگهبانشون متنفر باشن چون سعی میکنه ازشون محافظت کنه! پس پرا تو نمی‌تونی فقط--

`bb({ eyes:"normal" });`

h: جوابت اشتباه بود ^کیری^.

(#act3_bad_3)



# act3_bad_3

```
music(null);
hong({body:"drink"});
bb({body:"attacked"});
publish("bb_STOP_VIBRATING");
attackBB("100p");
```

(...2000)

```
hong({ body:"normal", mouth:"normal", eyes:"normal" });
bb({ body:"dead" });
```

(...999)

h: *"تنها چیزی که باید از آن ترسید خود ترس است."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"نگران نباش، خوشحال باش!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: تمام آدمای خردمند این زمونه موافقن که: احساسات منفی *بدن*!

`hong({ eyes:"less_angry" });`

h: والا! واسه همین بهشون میگن *منفی*!

b: انسان... لطفا...

`hong({ eyes:"normal" });`

h: یه مدت قبل، من گفتم: "من فقط میخوام از شر این همه درد خلاص بشم."

h: من به آرزوم رسیدم. دیگه نه درد، نه ترس و نه اضطراب...

h: اصلا دیگه هیچ حسی ندارم.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: انقد میخواستم مطمئن بشم چیزی بهت صدمه نمی‌زنه، که متوجه نشدم *من* اون چیزی بودم که داشت بهت صدمه می‌زد.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NO. S^HIT^.

`hong({ body:"yell_1" });`

h: !ای خدا لعنتت کنه! واقعا انقد طول کشید تا بفهمی؟

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: تو می‌تونستی از این همه بدبختی‌مون جلوگیری کنی، تو ^اسکل^ پشمالو. چرا زودتر متوجه نشدی؟

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ... تو *متاسفی*.

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: برای *چی* متاسفی؟

(#act3_good_2q)


# act3_good_2q

`bb({mouth:"sorry", eyes:"sorry"});`

{{if _.apologized_for_hurt}}
(#act3_good_2q_already_apologized)
{{/if}}

{{if !_.apologized_for_hurt}}
(#act3_good_2q_not_already_apologized)
{{/if}}


# act3_good_2q_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"less_angry" });`

[متاسفم که محافظ خوبی نبودم.](#act3_good_3_protector)

[متاسفم که بهت احترام نذاشتم.](#act3_good_3_respect)

[من متاسفم.](#act3_good_4)


# act3_good_2q_not_already_apologized

`hong({ body:"normal", mouth:"angry", eyes:"angry" }, 0);`

[I'm sorry I have a terrible human!](#act3_bad_2_terrible) `bb({mouth:"normal", eyes:"normal"})`

[I'm sorry I didn't respect you.](#act3_good_3_respect)

[I'm sorry I hurt you.](#act3_good_3_hurt)



# act3_good_3_protector

`bb({eyes:"sorry_down"});`

b: It's my duty to warn you against *real* danger, but I kept barking at cars and the mailman.

`bb({eyes:"sorry_up"});`

b: Barking at shadows. Barking so much.

`bb({eyes:"sorry"});`

b: It only makes sense that you'd want to muzzle me.

`bb({eyes:"sorry_down"});`

b: I'm sorry.

(#act3_good_4)



# act3_good_3_respect

`bb({eyes:"sorry_down"});`

b: I was supposed to be *your* loyal guard-dog, but I acted as if you were supposed to obey *me*.

`bb({eyes:"sorry_up"});`

b: There's a difference between a protector and a prison warden, and I crossed the line.

`bb({eyes:"sorry_down"});`

b: I'm sorry.

(#act3_good_4)



# act3_good_3_hurt

`bb({eyes:"sorry_down"});`

b: I was so obsessed with trying to protect you from being hurt, I never stopped to realize *I* was hurting you.

`bb({eyes:"sorry_up"});`

b: I was a bad dog.

`bb({eyes:"sorry_down"});`

b: I'm sorry.

(#act3_good_4)


# act3_good_4

```
music(null,{fade:3});
hong({ eyes:"less_angry", MOUTH_LOCK:true },0);
```

h: ...

```
hong({ body:"stop", mouth:"stop", eyes:"blank" });
```

h: Yeah, well, this was a dumb idea anyway.

h: I only did this to mess you up, and, well, I messed you up.

h: Let's just call this round a tie, okay?

```
bb({ mouth:"sorry", eyes:"sorry" });
bb({ MOUTH_LOCK:true });
```

b: ...

b: Okay.

h: Okay.

n: *TIE*

`_.a3_ending = "walkaway";`

(#act3_end)









# act3_end

```
Game.clearText();
publish("act3-in");
publish("hp_hide");
Game.FORCE_CANT_SKIP = true;
```

{{if _.a3_ending=="walkaway"}}
(#act3_walkaway)
{{/if}}

{{if _.a3_ending=="jump"}}
(#act3_jump)
{{/if}}






# act3_walkaway

```
publish("start-walkaway-anim");
Game.WORDS_HEIGHT_BOTTOM = 205;
```

(...3501)

```
sfx("bottle_toss");
publish('hong-next');
publish("act3",["roofhunter",7]);
```

(...667)

```
publish("act3",["dd",4]);
publish("act3",["roofhunter",26]);
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("concrete_step2");
```

(...667)

```
publish('hong-next');
publish("act3",["roofhunter",27]);
```

`Game.FORCE_CANT_SKIP = false;`

r: Oh *come on*. After all that animal's done to you, you're just *giving up?*

r: What's the matter, kid? Are you *scared?*

```
publish('hong-next');
publish("act3",["roofhunter",26]);
```

h2: Yes.

h2: I'm scared.

`publish('hong-next')`

h2: And that's okay!

`publish('hong-next')`

h2: It's okay to be scared.

`publish('hong-next')`

(...500)

```
Game.clearText();
Game.FORCE_CANT_SKIP = true;
```

(...1167)

```
publish('hong-next');
```

(...833)

```
publish('hong-next');
sfx("rustle2");
```

(...1333)

```
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",31]);
sfx("concrete_step4");
```

(...667)

```
publish('hong-next');
sfx("concrete_step1");
```

(...667)

```
publish('hong-next');
sfx("door");
```

(...1333)

```
publish('hong-next');
sfx("concrete_step2");
```

(...501)

```
publish('hong-next');
Game.FORCE_CANT_SKIP = false;
sfx("lock_door");
publish("act3",["roofhunter",32]);
```

(...2001)

```
publish("act3",["roofhunter",33]);
```

r: Did they just lock the door?

```
Game.clearAll();
_.INJURED = false;
Game.WORDS_HEIGHT_BOTTOM = -1;
```

(...2000)

(#act4)




# act3_jump

```
publish("start-jump-anim");
Game.FORCE_TEXT_Y = 300;
```

(...2001)

```
publish('hong-next');
sfx("bottle_toss");
```

(...833)

```
sfx("concrete_step1");
sfx("claps");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",28]);
```
(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step2");
publish('hong-next');
publish("act3",["roofhunter",28]);
```

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

`publish("act3",["roofhunter",28]);`

(...125)

`publish("act3",["roofhunter",29]);`

(...125)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",5]);
publish("act3",["roofhunter",34]);
```

(...1167)

```
sfx("rustle2");
publish('hong-next');
```

(...1001)

`publish('hong-next')`

b: no...

(...501)

`Game.clearText();`

`publish('hong-next')`

(...1333)

```
sfx("quack");
publish('hong-next');
```

(...1333)

`publish('hong-next')`

b: no no no

(...501)

`Game.clearText();`

`publish('hong-next')`

(...2001)

```
sfx("rustle2");
publish('hong-next')
```

(...501)

```
sfx("concrete_step1");
publish('hong-next');
publish("act3",["dd",4]);
publish("act3",["roofhunter",30]);
```

(...167)

```
sfx("concrete_step2");
publish('hong-next');
```

(...167)

```
sfx("concrete_step3");
publish('hong-next');
publish("act3",["dd",2]);
publish("act3",["roofhunter",15]);
```

(...167)

```
sfx("bottle_slip");
publish('hong-next');
publish("act3",["dd",3]);
publish("act3",["roofhunter",16]);
```

(...833)

```
sfx("rustle");
publish('hong-next');
```

(...167)

`publish('hong-next')`

(...167)

```
publish('hong-next');
Game.FORCE_TEXT_Y = 325;
Game.OVERRIDE_FONT_SIZE = 50;
```

b: NO!

(...400)

```
Game.WORDS_HEIGHT_BOTTOM = -1;
Game.FORCE_TEXT_Y = -1;
Game.clearText();
publish("act4-injury-show");
publish("hide_tabs");
```

(...2000)

```
sfx("hospital1");
publish("act4-injury", [1]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital2");
publish("act4-injury", [2]);
```

(...4000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...2000)

```
sfx("hospital3");
publish("act4-injury", [3]);
```

(...8000)

```
stopAllSounds();
publish("act4-injury", [0]);
```

(...5500)

`_.INJURED = true;`

(#act4)
