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

r: همینه! من بهت ایمان دارم عزیزم! بکشش!

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

b: no no no no no no

n: THIS CHAPTER HAS TWO POSSIBLE ENDINGS. ONE IS *VERY, VERY BAD.*

b: NO NO NO NO NO NO NO NO NO NO NO NO NO NO

n: CHOOSE WISELY. PROTECT YOUR HUMAN

`bb({ eyes:"oh_crap", mouth:"normal_talk", MOUTH_LOCK:true });`

b: AAAAAAAAAAAAAAAAAA

`bb({ mouth:"normal" });`

n: GOOD LUCK

```
Game.clearText();
bb({ eyes:"start" });
```

[Human, you could actually DIE here!](#act3a_harm) `Game.OVERRIDE_CHOICE_LINE=true`

[This is stupid and self-destructive!](#act3a_bad) `Game.OVERRIDE_CHOICE_LINE=true`

[These sickos aren't really your friends!](#act3a_alone) `Game.OVERRIDE_CHOICE_LINE=true`

# act3a_harm

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: H--

(#act3a_after)

# act3a_alone

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

(#act3a_after)

# act3a_bad

`bb({ MOUTH_LOCK:true, mouth:"normal_talk" });`

b: T--

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

h: You know, I might've believed you... if you hadn't tried that a zillion times before.

h: You're the wolf who cried wolf.

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

h: You tried that too.

b: human, please...

`hong({ eyes:"look_right" });`

h: Oh I'm *sorry* Big Pharma doesn't approve of my self-medication.

h: Look ^asshole^, we *all* have a way of shutting you the ^fuck^ up.

`hong({ body:"look_up", eyes:"look_up" });`

h: Some people throw themselves into work.

`hong({ body:"look_down", eyes:"look_down" });`

h: Some people throw themselves into sex, drugs, and refreshing their Facebook feed.

`hong({ body:"normal", eyes:"look_right" });`

h: Some people throw themselves into other people. 

`hong({ eyes:"angry" });`

h: I'm going to throw myself into that swimming pool.

[You're drunk and it's SIX FLOORS DOWN](#act3_bad_1_harm)

[Dang it, this is the thanks I get?!](#act3_bad_1_insult) `bb({eyes:"angry"});`

[Okay, I admit it. I messed up.](#act3_good_1) `bb({mouth:"sorry", eyes:"sorry_down"});`

# act3_bad_1_harm

b: Even if you land in the water, the surface tension will crack your ribs and give you a concussion *at the least!*

h: Eh.

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

h: I saw a Russian guy do this on YouTube once.

(#act3_bad_2)

# act3_bad_1_insult

`hong({ eyes:"look_right" });`

h: I- Excuse me, the *thanks?*

`bb({ eyes:"angry" });`

b: This is exactly why I *exist!* Because humans can't be trusted to protect themselves!

b: I've been trying to protect your stupid butt all my life and now you're just going t--

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

h: heh.

`hong({ body:"laugh_2" })``

h: hahahaha

`hong({ body:"laugh_3" })``

h: HAHAHAHAHAHA

```
bb({ eyes:"sorry"});
hong({ body:"yell_1", mouth:"yell", eyes:"blank" });
```

h: Oh WOW is that the biggest *^fuck^ing* understatement of the century!

`hong({ body:"yell_2" });`

h: Yeah, you rotting pile of blood-coated ^shit^! You messed the ^fuck^ up!

`hong({ body:"normal", mouth:"angry", eyes:"angry" });`

h: Any other remarks, Captain Obvious?

[But revenge on me isn't the answer!](#act3_good_1_fail_revenge) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[But this time I'm *actually* right!](#act3_good_1_fail_harm) `bb({ body:"normal_"+_.act3_bb_body, mouth:"normal", eyes:"normal" });`

[I've hurt you.](#act3_good_2a)


# act3_good_1_fail_revenge

b: You need to have a healthier relationship with your emotions, rather than drown them wi--

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

b: So please, put the bottle down and let's--

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

b: please... don't...

h: Your energy bar's looking awfully low there, wolf.

h: If I were you, I'd choose your next words very carefully.

`bb({ eyes:"normal" });`

[Fine. I'm done protecting you.](#act3_bad_2_jump) `bb({ mouth:"ignore", eyes:"ignore" });`

[I was right all along.](#act3_bad_2_right)

[I'm sorry.](#act3_good_2b) `bb({mouth:"sorry", eyes:"sorry_down"});`


# act3_bad_2_jump

b: So, go ahead and jump. See what I care.

`hong({ eyes:"look_right", mouth:"normal", MOUTH_LOCK:true });`

h: ...

```
hong({ eyes:"less_angry", mouth:"normal" });
bb({ eyes:"ignore_oh_crap" });
```

h: Okay then. Bottoms up.

```
bb({ mouth:"normal", eyes:"oh_crap" });
Game.OVERRIDE_TEXT_SPEED = 2;
```

b: WAIT NO THAT WAS REVERSE PSYCHOLOGY YOU WERE SUPPOSED TO DO THE *OPPOSITE* OF WHAT I SA--

(#act3_bad_3)



# act3_bad_2_right

`bb({ eyes:"angry" });`

b: You *are* putting yourself in danger. Your so-called friends *are* using you. And *you* are using your so-called friends.

`bb({ eyes:"sad" });`

b: So please, human... why don't you believe me?!

h: Because you never believed in *me*.

(#act3_bad_3)


# act3_bad_2_terrible

`bb({ eyes:"angry" });`

b: Other guard-wolves have humans who actually take time to patiently train them, to *learn* to work together,

b: Rather than hate the guard-wolves for trying to protect them! So why can't you jus--

`bb({ eyes:"normal" });`

h: Wrong ^fuck^ing answer.

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

h: *"The only thing to fear is fear itself."*

`hong({ body:"look_up", mouth:"happy", eyes:"blank" });`

h: *"Don't worry, be happy!"*

`hong({ body:"normal", mouth:"normal", eyes:"normal" });`

h: All the wise folk of our time agree: negative emotions are *bad!*

`hong({ eyes:"less_angry" });`

h: Duh! That's why they're called *negative!*

b: human... please...

`hong({ eyes:"normal" });`

h: A while back, I said: “I just want to be free from all this pain.”

h: I got my wish. I no longer feel pain, or fear, or anxiety...

h: I don't feel anything at all.

`_.a3_ending = "jump";`

(#act3_end)



# act3_good_2a

`bb({mouth:"sorry", eyes:"sorry_down"});`

b: I was so obsessed with making sure nothing else hurt you, that I didn't realize *I* was creating the hurt.

```
bb({ eyes:"sorry"});
hong({ body:"yell_2", mouth:"yell", eyes:"blank" });
```

h: NO. S^HIT^.

`hong({ body:"yell_1" });`

h: ^GODDAMN^. It really took you this long to finally figure it out?!

`hong({ body:"cry", mouth:"cry", eyes:"blank" });`

h: You could've saved us so much trouble, you big fluffy dumb^ass^. Why didn't you realize this sooner?...

`_.apologized_for_hurt = true;`

(#act3_good_2q)



# act3_good_2b

`hong({ body:"normal", mouth:"angry", eyes:"look_right" });`

h: ...you're *sorry.*

`hong({ eyes:"angry", MOUTH_LOCK:true });`

h: ...

h: Sorry for *what*?

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

[I'm sorry I wasn't a good protector.](#act3_good_3_protector)

[I'm sorry I didn't respect you.](#act3_good_3_respect)

[I'm sorry.](#act3_good_4)


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
