# STORYLINES - CyberTok Interactive Visual Novel

## How To Use This Script

- This file is written as a playable branching scenario for an interactive game.
- Each scene includes:
  - Background narration
  - Character dialogue
  - Player choices
  - Branch outcomes
- Use scene IDs to connect branches in your game engine.

---

## CAST

- You (Player, 14 years old, gender neutral)
- FaizTheGoat (Trusted friend)
- AbangMer.11 (Groomer)
- U_look_gut (Catfish/Sextortion blackmailer)
- The_Si_Kamar (Scammer)
- BawangGirlzzz (Cyberbully)
- System Narrator

---

## GLOBAL MECHANICS

- Trust Meter: Starts neutral.
- Safety Meter: Starts neutral.
- Every unsafe choice lowers Safety Meter.
- If Safety Meter remains high through a route, player can reach Good Ending.

Safety actions that increase Safety Meter:
- Refusing secrecy
- Blocking/reporting suspicious users
- Preserving evidence (screenshots)
- Telling a trusted adult

---

## SCENE 00 - TITLE SCREEN

[Background: Neon Kuala Lumpur skyline at sunset. Soft lo-fi beat.]

Narrator:
A first laptop.
A first social media account.
A first week online without supervision.

Narrator:
Some people online are real.
Some are fake.
Some are hunting.

System:
CYBERTOK: THINK BEFORE YOU CLICK
Press Start.

[CHOICE]
A) Start Game -> SCENE 01
B) Safety Tips First -> SCENE 00A

---

## SCENE 00A - QUICK SAFETY TIPS

[Background: In-game tips panel with icons.]

System:
Before you begin, remember:

1. Do not share school details, address, or routine.
2. Never share TAC/OTP/passwords.
3. Never move to secret chats with strangers.
4. Screenshot suspicious behavior.
5. Block, report, tell a trusted adult.

[CHOICE]
A) Continue -> SCENE 01

---

## SCENE 01 - FIRST ACCOUNT

[Background: Bedroom desk, new laptop glow, rain outside.]
[BGM: Upbeat lo-fi]

Narrator:
You finally got your own laptop.
No more borrowing Mum's old tablet.
No more waiting turns.

You:
Okay. New era. New account. New me.

System:
Welcome to CyberTok Malaysia (v2026.5).
Initialize profile.

You:
Faiz should be done with cybersecurity class soon.
I need to look active before he follows me.

System:
Enter Username.

[CHOICE]
A) RealName_Official
B) MythicKidX
C) Create custom username

System:
Select privacy settings.

[CHOICE]
A) Public account, DMs open to everyone
B) Private account, DMs from followers only

Narrator:
You hover over the options, thumb twitching over the trackpad.

If A Public -> SCENE 02P
If B Private -> SCENE 02R

---

## SCENE 02P - PUBLIC ACCOUNT START

[Background: Profile page goes live, follower count jumps from 0 to 12 quickly.]

System:
Account visibility: PUBLIC

You:
Nice, people can find me faster.
Faiz better not be late.

System:
Create your first post.

[CHOICE]
A) OOTD in school uniform
Caption: "Bored after school at SMK Damai. MLBB anyone?"

B) Laptop setup photo
Caption: "Rate my setup. Mythical grind starts tonight."

If A OOTD -> add risk tag SchoolExposure
If B Setup -> add risk tag LowExposure

-> SCENE 03_HUB

---

## SCENE 02R - PRIVATE ACCOUNT START

[Background: Lock icon appears on profile.]

System:
Account visibility: PRIVATE

You:
Safe mode on. Easy.

Narrator:
Within minutes, follow requests appear:
@U_look_gut
@HafizGamerz67
@AbangMer.11

You:
I do not know these people... but I need followers before Faiz arrives.

[CHOICE]
A) Accept all requests
B) Accept only mutuals / people you can verify
C) Reject all unknowns

If A -> Safety Meter down
If B -> Safety Meter neutral
If C -> Safety Meter up

System:
Create your first post.

[CHOICE]
A) OOTD in school uniform
B) Laptop setup photo

-> SCENE 03_HUB

---

## SCENE 03_HUB - MULTIPLE THREATS ARRIVE

[Background: Notification feed flooding animation.]
[BGM: Faster beat with notification pings]

Narrator:
Three DMs arrive in the same hour.
Different profile pictures.
Same objective: access.

System:
New DM from AbangMer.11
New DM from U_look_gut
New DM from The_Si_Kamar
New comment from BawangGirlzzz

You:
So many people on day one?
Is this normal...?

[CHOICE]
A) Open gamer DM (AbangMer.11) -> SCENE G1
B) Open attractive profile DM (U_look_gut) -> SCENE B1
C) Open business opportunity DM (The_Si_Kamar) -> SCENE S1
D) Check toxic comment thread (BawangGirlzzz) -> SCENE C1

Note:
In full game implementation, player can experience all four arcs over multiple in-game days.

---

# ROUTE G - GROOMING ARC

## SCENE G1 - FRIENDLY ENTRY

[Background: DM window with gaming stickers]
[BGM: Calm acoustic guitar]

AbangMer.11:
Hey bro, saw your MLBB post. Clean setup.
I am Mythic. Want free carry tonight?

You:
Free? Seriously?

AbangMer.11:
Ya lah. Just helping younger players.
No charge.

Narrator:
Compliment. Offer. Quick trust.
Classic soft entry.

[CHOICE]
A) "Sure, thanks!"
B) "How do I know you are legit?"
C) Ignore DM

If A -> SCENE G2
If B -> SCENE G2V (verification branch)
If C -> SCENE G_SAFE1

---

## SCENE G_SAFE1 - EARLY EXIT SAFE CHOICE

[Background: DM request panel closes]

You:
I do not know this person well enough. Not worth the risk.

Narrator:
You limit contact, keep your profile boundaries, and avoid emotional entanglement.

System:
SAFE RESOLUTION G (EARLY) - Grooming path avoided before escalation.
Safety Meter increased.

-> SCENE END_HUB

---

## SCENE G2V - VERIFICATION ATTEMPT

You:
Before we play, how old are you and which school?

AbangMer.11:
I am 15. Chill lah, why so formal?
Come, I send ID.

Narrator:
He sends a profile screenshot that can be faked in seconds.

[CHOICE]
A) Trust screenshot -> SCENE G2
B) Refuse and stay cautious -> SCENE G_SAFE1

---

## SCENE G2 - PERSONAL PROBING

[Background: Voice chat waveform animation]

Narrator:
You play three matches together. He is skilled and patient.
Then questions shift from game strategy to your personal life.

AbangMer.11:
You sound stressed today.
Family okay?

You:
My dad is angry about exams.
He might take my laptop.

AbangMer.11:
Parents never understand pressure. I understand you.
You can tell me anything.

[CHOICE]
A) Share deeper personal problems
B) Keep conversation game-only
C) End session politely

If A -> Safety down -> SCENE G3
If B -> SCENE G3
If C -> SCENE G_SAFE1

---

## SCENE G3 - ISOLATION TACTIC

[Background: Darker room tone, evening ambience]

AbangMer.11:
That Faiz friend? He does not defend you.
Honestly, I care more than your real friends.

Narrator:
He reframes your relationships.
This is isolation by suggestion.

[CHOICE]
A) "Maybe you are right..."
B) "Do not talk about my friends like that."
C) Screenshot this message

If A -> SCENE G4
If B -> SCENE G4
If C -> Safety up + evidence saved -> SCENE G4

---

## SCENE G4 - SECRECY + MIGRATION

AbangMer.11:
My parents monitor CyberTok.
Move to Telegram. Keep it between us.
I will send 1,000 diamonds now.

Narrator:
Secrecy request.
Platform migration.
Reward bait.
Three red flags at once.

[CRITICAL CHOICE]
A) Accept and move secretly -> SCENE G_BAD
B) Refuse secrecy, block, report -> SCENE G_GOOD
C) Ask trusted adult first -> SCENE G_GOOD

---

## SCENE G_BAD - BAD ENDING: GROOMED

[Background: Bus terminal at night, rain, neon blur]
[BGM: Low static drone]

Narrator:
Weeks pass.
He becomes controlling.
He asks for selfies, then secrets, then obedience.

Narrator:
You stop telling friends.
You hide chats from family.
You feel trapped but call it loyalty.

Narrator:
One night, he asks you to meet in person.
No cameras. No questions.

System:
BAD ENDING G - "The Trap Behind Kind Words"

Cybersecurity Debrief:
- Groomers build trust before control.
- Secrecy is the strongest warning sign.
- Safe action: stop contact, preserve evidence, report, tell a trusted adult immediately.

-> SCENE 99_RESTART

---

## SCENE G_GOOD - SAFE END: GROOMING BLOCKED

[Background: Report dialog box confirmation]

You:
Real friends do not need secrets.
Blocked.

System:
User reported for suspicious grooming behavior.

You:
(Messaging parent) Can we talk? Someone online is being weird and pushy.

Narrator:
The danger ends where secrecy ends.

System:
SAFE RESOLUTION G - Threat interrupted early.
Safety Meter increased.

-> SCENE END_HUB

---

# ROUTE B - CATFISH/SEXTORTION ARC

## SCENE B1 - LOVE-BOMBING ENTRY

[Background: Aesthetic profile grid, heart reaction spam]
[BGM: Soft romantic synth]

U_look_gut:
Hey... your vibe is so nice.
You are honestly my type.

You:
Uh... me?

U_look_gut:
Yes, you. I feel like we connect.

Narrator:
Attention can feel like truth.
But speed can be strategy.

[CHOICE]
A) Flirt back quickly
B) Keep neutral tone
C) Ignore message

If A or B -> SCENE B2
If C -> SCENE B_SAFE1

---

## SCENE B_SAFE1 - EARLY EXIT SAFE CHOICE

[Background: Chat request declined animation]

You:
Too fast. Too personal. I am out.

Narrator:
You decline the chat, restrict DMs, and avoid a potential catfish funnel.

System:
SAFE RESOLUTION B (EARLY) - Risk removed before pressure stage.
Safety Meter increased.

-> SCENE END_HUB

---

## SCENE B2 - PRIVATE PLATFORM PUSH

U_look_gut:
CyberTok is noisy. Move to Snapchat or Telegram.
Messages disappear there. Safer ;)

Narrator:
"Disappearing" does not mean unrecordable.

[CHOICE]
A) Move platform
B) Stay on CyberTok only
C) Stop chatting

If A -> SCENE B3
If B -> SCENE B3
If C -> SCENE B_SAFE1

---

## SCENE B3 - PRESSURE REQUEST

[Background: Typing bubble pauses, then appears repeatedly]

U_look_gut:
Can you send a private pic?
Just for me. If you trust me.

You:
I do not feel comfortable.

U_look_gut:
So you do not love me?

Narrator:
Guilt and affection are being weaponized.

[CRITICAL CHOICE]
A) Send image under pressure -> SCENE B_BAD
B) Refuse, screenshot, block/report -> SCENE B_GOOD
C) Tell trusted adult before responding -> SCENE B_GOOD

---

## SCENE B_BAD - BAD ENDING: SEXTORTION LOOP

[Background: Screen flashes with payment demand]
[SFX: Harsh static cut]

U_look_gut:
I recorded it. Pay RM500 now or everyone sees it.

Narrator:
You pay once.
Another demand follows.
Then another.

Narrator:
Blackmail does not end with compliance.
It scales.

System:
BAD ENDING B - "Paying The Threat"

Cybersecurity Debrief:
- Sextortion relies on fear and urgency.
- Paying confirms you are a profitable target.
- Safe action: do not pay, save evidence, block/report, inform trusted adults and authorities.

-> SCENE 99_RESTART

---

## SCENE B_GOOD - SAFE END: SEXTORTION STOPPED

[Background: Evidence folder with screenshots and username]

You:
No.

Narrator:
You screenshot threats, block the account, report in-app, and tell your parent/counselor.

System:
SAFE RESOLUTION B - Extortion attempt documented and escalated.
Safety Meter increased.

-> SCENE END_HUB

---

# ROUTE S - SCAM/SOCIAL ENGINEERING ARC

## SCENE S1 - EASY MONEY BAIT

[Background: "Business Account" badge and flashy income screenshots]
[BGM: Busy electronic rhythm]

The_Si_Kamar:
Yo boss, you want side income?
Student can earn RM200 daily.
Easy typing job.

You:
I am 14. Can I even do this legally?

The_Si_Kamar:
No issue. Digital era. I guide you.

Narrator:
The hook is desire: money, status, independence.

[CHOICE]
A) "Tell me more"
B) "I need to verify first"
C) Ignore and report

If A or B -> SCENE S2
If C -> SCENE S_SAFE1

---

## SCENE S_SAFE1 - EARLY EXIT SAFE CHOICE

[Background: Report modal success tick]

You:
If it sounds too good to be true, it probably is.

Narrator:
You report the account and verify opportunities only through trusted offline channels.

System:
SAFE RESOLUTION S (EARLY) - Scam entry point blocked.
Safety Meter increased.

-> SCENE END_HUB

---

## SCENE S2 - URGENCY + FAKE PROOF

The_Si_Kamar:
Slots almost full. Last day today.
See this screenshot? Form 2 student already bought gaming chair.

Narrator:
Urgency reduces critical thinking.
Fake proof replaces real verification.

[CHOICE]
A) Continue quickly
B) Ask parent before continuing
C) Ask for registered company info

If A -> SCENE S3
If B -> SCENE S_GOOD
If C -> SCENE S3V

---

## SCENE S3V - SHALLOW VERIFICATION FAIL

The_Si_Kamar:
No need so formal lah.
Trust me, I help youth.

Narrator:
He avoids verifiable details and redirects emotionally.

[CHOICE]
A) Proceed anyway -> SCENE S3
B) Stop and report -> SCENE S_GOOD

---

## SCENE S3 - CREDENTIAL THEFT REQUEST

The_Si_Kamar:
To release your RM200, send your Mum's bank card photo and TAC code.
Fast only.

Narrator:
No legitimate process asks for TAC/OTP from family accounts.

[CRITICAL CHOICE]
A) Share TAC code -> SCENE S_BAD
B) Refuse, screenshot, report -> SCENE S_GOOD
C) Tell parent immediately -> SCENE S_GOOD

---

## SCENE S_BAD - BAD ENDING: ACCOUNT DRAIN

[Background: Banking alert notifications nonstop]

Narrator:
The transfer succeeds.
RM4,500 disappears.
The account blocks you instantly.

Narrator:
Your home goes silent.
Then your mother cries.

System:
BAD ENDING S - "One Code, Full Loss"

Cybersecurity Debrief:
- Scammers exploit urgency and family trust.
- TAC/OTP is a key, not a formality.
- Safe action: never share TAC, verify opportunities offline, involve guardian immediately.

-> SCENE 99_RESTART

---

## SCENE S_GOOD - SAFE END: SCAM INTERRUPTED

[Background: Scam account report submitted]

You:
Real jobs do not need stolen bank access.
Reported.

Narrator:
You show the chat to your parent.
Damage prevented.

System:
SAFE RESOLUTION S - Financial scam blocked.
Safety Meter increased.

-> SCENE END_HUB

---

# ROUTE C - CYBERBULLY ARC

## SCENE C1 - BAIT COMMENT

[Background: Public comment thread, reaction emojis]
[BGM: Low bass tension]

BawangGirlzzz:
Ew, cringe. @YourUsername thinks they are famous.
Go back to Roblox lah.

You:
Why are you being toxic?

Narrator:
Public humiliation invites audience participation.

[CHOICE]
A) Reply angrily
B) Reply once, then stop
C) No reply, mute thread

If A or B -> SCENE C2
If C -> SCENE C_GOOD

---

## SCENE C2 - DOGPILE ESCALATION

Narrator:
She reposts your photo as a meme.
Now strangers pile into your comments and DMs.

RandomUser88:
Delete your account.

AnotherUser:
Your school should be embarrassed.

Narrator:
Harassment shifts from one bully to a swarm.

[CHOICE]
A) Post long angry defense
B) Collect evidence quietly
C) Ask friend/parent for help now

If A -> SCENE C_BAD
If B or C -> SCENE C_GOOD

---

## SCENE C_BAD - BAD ENDING: VIRAL RETALIATION

[Background: School hallway whispers, phone camera flashes]

Narrator:
Your rage replies become screenshot content.
Edited clips go viral out of context.

Narrator:
Mockery leaves the app and follows you to school.
Sleep drops. Anxiety rises.

System:
BAD ENDING C - "Fed The Fire"

Cybersecurity Debrief:
- Rage-bait aims to harvest reactions as content.
- Public retaliation often multiplies reach.
- Safe action: disengage, document abuse, block/report, involve school and guardians.

-> SCENE 99_RESTART

---

## SCENE C_GOOD - SAFE END: HARASSMENT CONTAINED

[Background: Notification settings toggled off, block list updated]

You:
I will not perform for bullies.

Narrator:
You screenshot evidence, block the ringleader, report posts, and speak to a counselor and parent.

System:
SAFE RESOLUTION C - Harassment documented and escalated safely.
Safety Meter increased.

-> SCENE END_HUB

---

## SCENE END_HUB - WEEKEND CALL WITH FAIZ

[Background: Discord call overlay, warm room lighting]
[BGM: Hopeful theme]

[SFX: Discord join sound]

FaizTheGoat:
Yo, finally. Sorry I am late, cyber class overtime.
How was your first week on CyberTok?

You:
Honestly? Messy.
I saw how fast things can turn unsafe.

FaizTheGoat:
What did you do?

If player completed safe resolution for each route encountered:

You:
I watched for red flags, took screenshots, blocked and reported, and told adults early.

FaizTheGoat:
That is real cyber defense.
Not just passwords. Decisions.

System:
GOOD ENDING - "Think Before You Click"

Learning Recap:
- Grooming: kindness + secrecy + isolation
- Sextortion: romance pressure + threats
- Scam: urgency + fake proof + TAC theft
- Bullying: provocation + viral amplification

Final Rule:
Stop. Check. Share.

-> SCENE 100_CREDITS

If player has unresolved bad endings:

FaizTheGoat:
We can still fix this.
You are not alone, okay?

System:
PARTIAL ENDING - "Recovery Starts Now"

Recovery Actions:
1. Save all evidence
2. Block/report all involved accounts
3. Inform trusted adult and school
4. Contact official help channels

-> SCENE 100_CREDITS

---

## SCENE 99_RESTART - TRY AGAIN PROMPT

System:
You reached a bad ending.
Do you want to replay from the critical choice?

[CHOICE]
A) Replay critical choice
B) Return to route start
C) Return to title screen

---

## SCENE 100_CREDITS

[Background: Sunrise over city skyline]
[BGM: Triumphant light orchestral]

Narrator:
Cyber safety is not one app setting.
It is a habit repeated in small moments.

Narrator:
When in doubt:
Pause.
Document.
Report.
Tell someone you trust.

System:
Thank you for playing.

---

## IMPLEMENTATION NOTES FOR DEVELOPERS/EDUCATORS

- Add in-game glossary popup for terms:
  - Grooming
  - Sextortion
  - Social engineering
  - Doxxing
  - TAC/OTP
- At each critical choice, provide optional "Why this matters" tooltip.
- Add local support resource panel in main menu.
- Enable teacher mode:
  - Pause on critical choices
  - Show discussion prompts
  - Export route decisions for classroom debrief
