# Build Offline Hide-and-Seek, Then Pitch Publishers

A low-poly, round-character hide-and-seek game for Android is feasible, and the genre still has demand. It is also crowded at the top, so you will only succeed with a clear twist, a meta layer, and either publisher-funded user acquisition or a strong regional niche. The genre's biggest hit was built by a solo developer: Supersonic's **Hide 'N Seek! has about 278M Android installs** and is still being updated in 2026. **Hide Online (165M) and Kwalee's Hunt & Seek (82M)** show the demand is lasting. But when Hide 'N Seek's own developer self-published an online follow-up, it reached **only about 209K installs**. That is the clearest warning against launching with no user acquisition. Here is the recommended build:

- **Camera:** a fixed high-angle follow camera at about 50°.
- **Controls:** a floating joystick plus one context-sensitive "Hide" button.
- **Players:** offline AI bots with believable names. Do not build real-time multiplayer.
- **Monetization:** opt-in rewarded ads, capped interstitials between rounds, and a "No Ads" purchase.
- **Theme:** a house starter map plus Indian-themed maps (a Kerala tharavad, a train, a temple festival) as the thing that sets you apart.

Ad money from India and nearby South Asian countries alone will be small. Tier-1 players, usually reached through a publisher, are what make it a real income.

## Three hits prove the demand; one flop proves the distribution problem

The market data has two sides. Hide 'N Seek! (Supersonic) launched in April 2020 and has **278.2M installs and a 3.8-star Android rating**. It runs 17 ad-network SDKs and was updated on September 26, 2026 ([AppGoblin](https://appgoblin.info/apps/com.seenax.HideAndSeek)). Hide Online: Prop Hunt has **165M+ installs at 4.53 stars** and is still updated eight years after launch ([AppGoblin](https://appgoblin.info/apps/com.hitrock.hideonline)). Kwalee's Hunt & Seek, launched as recently as 2022, reached **82.3M** ([AppGoblin](https://appgoblin.info/apps/com.kwalee.transformhunt)). Games this old being actively updated in 2026 means they still make money.

The solo-developer story matters most here. Hide 'N Seek was made by one developer. It **reached #1 on Google Play US and was profitable on day one** of its global launch. Supersonic ran the ad waterfalls and the UA creatives ([Supersonic case study](https://supersonic.com/case-studies/hide-n-seek)). The fixes that improved retention apply directly to your design: a coin bonus level every 10 levels lifted **D1 retention to 48%**, and Supersonic also advised smaller levels, slower characters, a smaller vision field, vertical level elements, simpler menus, and skins with progression ([Supersonic](https://supersonic.com/case-studies/hide-n-seek)). These are 2020 numbers, though. The same developer's self-published online game, Hide & Seek Friends!, reached only **~209K installs** despite a known name ([AppGoblin](https://appgoblin.info/apps/com.seenax.hnsonline)).

The market has also shifted. Industry voices in late 2025 say "we don't talk about low CPIs anymore". Pure hyper-casual games don't keep players, so the money has moved to hybrid-casual games, which add a metagame and in-app purchases ([PocketGamer.biz](https://www.pocketgamer.biz/we-dont-talk-about-low-cpis-anymore-as-hybridcasual-raises-player-retention)). Appodeal's 2025 benchmarks put average hyper-casual ARPU at **$0.86** and say such games "suffer from low ad ARPU and poor retention" ([App Developer Magazine](https://appdevelopermagazine.com/mobile-casual-benchmarks-report-2025/)). So yes, it is feasible, but as a **hybrid-casual** game with skins, map unlocks and progression, not a one-mechanic throwaway.

There are gaps you can use. Mid-core competitors like Hide Online get reviews complaining that coins are only buyable with money, that skins are too hard to unlock, and that an alert icon gives away a hider who stands still. They also get repeated requests for more maps and props ([App Store](https://apps.apple.com/us/app/-/id1408624516)). Hide 'N Seek reviewers say the levels get repetitive ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)). None of the leading map lists use Indian settings. That is my own observation from the lists I saw, not a verified market gap.

## A tilted follow camera and a one-button hide beat every alternative

**Camera.** Each standard view has a weakness for this game. Top-down shows the layout and routes clearly but gives little sense of height. Third-person shows the character and its costume but has trouble with walls blocking the view. First-person hides your own body and can cause motion sickness ([Unity](https://unity.com/blog/video-game-camera-perspectives)). Your hiding spots depend on height: under beds, on tables, on the top bunk. So the best choice is a **high-angle third-person follow camera at about 45–60°, with no manual rotation by default**. It keeps top-down readability, shows furniture height, and shows off round-character skins, which you will sell. Make walls fade or become see-through when they come between the camera and the player. When the player is under a bed, show them their own outline; the seeker sees nothing unless the vision cone and line of sight reach the hider. Free camera control is a known failure point. A low-rated prop-hunt clone gets repeated complaints that the camera "would not move" or was "confusing" ([App Store](https://apps.apple.com/app/id1604406350)). Accessibility guidance also says to avoid camera movement the player didn't ask for, and to make camera shake and head bob optional ([Xbox Accessibility Guideline 117](https://devdocs.xbox.com/gaming/accessibility/xbox-accessibility-guidelines/117)).

**Seeker vision.** Draw the seeker's sight as a **visible red cone or flashlight**. This is the central readability device in Supersonic's hit, where touching the red area means you are found ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)). On a small screen it gives hiders a clear signal of danger.

**Controls.** Use a **floating joystick on the left half of the screen and one large context button on the right**. Its icon changes with the nearest object: "Hide under bed", "Climb onto table/bunk", "Lie down", "Open closet". Tapping it auto-snaps the character into the hide pose, so players never have to make precise jumps. That suits casual players and budget Indian phones. Hide 'N Seek itself uses simple drag-to-move ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)). Hide Online, aimed at a more core audience, lets players move, resize and change the transparency of buttons, and offers 30–120 FPS options ([App Store](https://apps.apple.com/us/app/-/id1408624516)). Add those settings later. Touchscreens give no physical feedback, so make up for it with layered sound, visual and animation cues ([Game Developer](https://www.gamedeveloper.com/game-platforms/designing-better-controls-for-the-touchscreen-experience)). A haptic tick when entering or leaving a hiding spot does this cheaply. Add at most one ability button. Roblox's Hide and Seek Extreme gives each seeker a single ability on one button ([Sportskeeda](https://sportskeeda.com/roblox-news/everything-know-roblox-hide-seek-extreme)). Target 30 FPS by default, with a 60 FPS option.

**Core loop.** Use a 15–20 s hide countdown while the seeker is frozen, then a 60–90 s search, and swap roles each round. Fortnite's prop-hunt template shows the balancing tools you can borrow ([Epic](https://dev.epicgames.com/documentation/fortnite/design-a-prop-hunt-game-in-fortnite-creative)):

- a hider head start
- slower hunters and faster hiders
- a penalty for spamming searches
- coins scattered around the map that tempt hiders out of cover

Two more ideas are proven in this genre:

- **Cage and rescue:** caught hiders go into a cage, and teammates can free them for coins ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)).
- **Noise and per-spot rules from Granny:** noise reveals your exact location to the hunter, and each hiding spot has its own way of being searched, such as a drop-and-lunge under beds and a pull-out from cabinets ([Granny wiki](https://slendrinahorrorgame.fandom.com/wiki/Granny_(character)?oldid=4170)).

If a hider stays still for more than about 20 s, give a short, subtle reveal pulse. Do not use a permanent giveaway icon.

## Offline bots are enough at launch, as long as the store listing is honest

**Real-time multiplayer is not necessary for v1, and you should not build it.** The genre leader appears to be fully offline. Reviewers note that it works with Wi-Fi off and that the "other players" look like bots, yet it holds **4.6 stars from 82K UK ratings**. "No online play" is a complaint but has not hurt it badly ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)). Photon's Mark Val says many .io-era hits were "fake" multiplayer. He recommends bots for onboarding, for replacing players who disconnect, and for filling empty rooms ([PocketGamer.biz](https://www.pocketgamer.biz/hypercasual-multiplayer-mark-val-photon-engine)).

Server costs are not the real obstacle. Photon gives **100 CCU free, including commercial use**, for Fusion and Quantum games ([Photon](https://doc.photonengine.com/photon/current/pricing)), and it has a **Chennai region** ([Photon Regions](https://doc.photonengine.com/fusion/current/reference/regions)). Unity Relay gives 50 average CCU free ([Unity](https://unity.com/products/gaming-services/pricing)). The real obstacle is **empty lobbies**. A new game with a few hundred daily players spread across time zones will usually have only a handful online at once, so you would need bot backfill anyway. Cheating is the second problem: anyone with a modded APK and a wallhack ruins a hiding game, and stopping that needs server authority, which multiplies cost. Offline also fits your target players. Industry commentary says "offline is a must in developing countries", and ads can still be cached in the background while the phone is connected ([PocketGamer.biz](https://www.pocketgamer.biz/the-case-for-offline-mobile-games/)).

The one firm rule is about Google Play policy, not the bots themselves. Google bans "false or misleading information or claims" in a listing and requires apps to "accurately and clearly describe their functionality" ([Google Play Policy](https://support.google.com/googleplay/android-developer/answer/9888077)). Fake player names are fine. Do not say "play online with real players" in your title, description or screenshots, and avoid fake "searching for players…" screens that reviewers will expose. Core gamers strongly dislike hidden bots ([PC Gamer](https://www.pcgamer.com/games/fps/games-that-try-to-sneak-bots-into-multiplayer-matches-are-automatically-trash/)). Casual players care less, but honest wording costs you nothing.

**Making the AI feel human** needs no machine learning. Use NavMesh, hand-placed hiding-spot nodes, and some deliberate imperfection. One hide-and-seek AI demo gives its seeker a 180° vision cone and a "suspicious area" that spreads outward from where it last saw a hider ([Minsu portfolio](https://minsu9486.github.io/portfolio/ai-game-tilemap)). Influence maps in Game AI Pro 2 answer "where can't I be reached?" by inverting a threat map, only spreading into cells the threat can see, and updating every 0.5–2 s to save CPU ([Game AI Pro 2](https://www.gameaipro.com/GameAIPro2/GameAIPro2_Chapter30_Modular_Tactical_Influence_Maps.pdf)).

In practice, have each **hider bot** score spots by how hidden they are, how far they are by path from the seeker, and how far from other hiders, plus some randomness, and then pick from the top few. Bots should fidget, and sometimes move to a new spot when the seeker is far away. The **seeker bot** keeps a list of spots it has visited, checks unvisited spots in order of score, and when it half-sees a hider, goes to the last known position.

For human feel, give bots a reaction delay of about **0.2–0.6 s** (my estimate, not a sourced figure) and a short "noticing" meter instead of instant detection. Add occasional wrong turns and look-around pauses. Draw names from region-appropriate lists with number suffixes, such as "Arjun_27", "Emma2011" or "Rafi.bd". To set difficulty, tune the cone angle, the reaction time, and how often the bot picks the best spot. Let new players win more often. Build bots on the same "player controller" interface a networked player would use, so you can add friend rooms in v2 (Photon Fusion Shared mode, with bots filling empty slots) if you get enough players.

## India pays roughly a tenth of Tier-1 per ad, so plan for both

Benchmarks disagree by up to **4x**, so treat the figures below as rough ranges ([Playio](https://blog.playio.co/mobile-game-ecpm-benchmarks-2026)). Tier-1 rewarded eCPMs run about **$15–30** and interstitials about **$5–8** (Playwire 2025). One older 2024 dataset puts US Android rewarded at **$30.25** ([Playio](https://blog.playio.co/mobile-game-ecpm-benchmarks-2026)). One source suggests floor prices of **$1–3 for India interstitials** and **$0.30–1 for Pakistan and Bangladesh**. The same source gives illustrative ARPDAU of **US ~$0.15 vs India ~$0.03**, though it cites no sources ([RevenueFlex](https://revenueflex.com/blog/app-monetization-emerging-markets-strategy/)). I could not find reliable figures for Sri Lanka or Nepal.

| Market | Rewarded eCPM | Interstitial eCPM | Illustrative ARPDAU |
|---|---|---|---|
| US / Tier-1 | $15–30 | $5–25 | ~$0.10–0.15 |
| India | much lower (no reliable figure) | $1–3 (floor) | ~$0.03 |
| Pakistan / Bangladesh | lower still | $0.30–1 (floor) | n/a |

My own arithmetic: **10,000 Indian daily players earn about $300/day; the same number in the US earns about $1,000–1,500/day**. South Asia gives you cheap volume, cheap testing and an audience for regional themes. Tier-1 brings in most of the revenue, and reaching those players usually takes paid user acquisition, which is what a publisher provides.

**Ad placements.** Rewarded ads work best at the end of a level ("x3 coins"), for a retry or extra life, to skip something, as chest speed-ups, and as offers on the home screen. Always show the reward clearly up front ([ironSource/LevelPlay](https://is.com/community/academy/ad-placements/the-best-rewarded-video-ad-placements)). For this game, that means x3 coins after a round, escaping the cage once, starting as seeker with a gadget, and trying a premium skin for one round. **Do not repeat Supersonic's mistakes.** Ads after every level and on being caught, and ability pads that trigger an ad, were its top complaints, and the developer later cut ad frequency ([App Store](https://apps.apple.com/gb/app/hide-n-seek/id1491654968)). Show an interstitial only every 2–3 rounds, cap the frequency, and sell **"No Ads" at about ₹99/$0.99**.

**Ad mediation.** AppLovin MAX is used in **73% of the top-downloaded ad games**. MAX, LevelPlay and AdMob together hold over 90% of the market ([PocketGamer.biz](https://www.pocketgamer.biz/nine-facts-about-the-mediation-space-in-2025)). As a solo developer, start with **AdMob with bidding** or LevelPlay, which you may already be using for your other games. Switch to whatever stack a publisher uses if you sign with one.

## Maps should multiply hiding spots, and Indian settings set you apart

Fortnite's guidance is that grouping similar objects lets hiders blend in, and big groups make it tense when a hunter comes close ([Epic](https://dev.epicgames.com/documentation/fortnite/design-a-prop-hunt-game-in-fortnite-creative)). Competitors' maps stick to familiar places. Hide Online has Factory, School, Cafe, Hangar and seasonal maps. Roblox HnS Extreme uses giant-scale versions of a bedroom, kitchen, workshop, backyard and attic ([Sportskeeda](https://sportskeeda.com/roblox-news/everything-know-roblox-hide-seek-extreme)). The table below is my design proposal, ordered as a release sequence.

| Map | Key hide / interact objects |
|---|---|
| **House (starter)** | beds (under), bunk beds (top), dining table with tablecloth, sofa, wardrobe, curtains, bathtub with curtain, laundry basket, toy box, doors |
| **School** | rows of desks and benches, teacher's table, lockers, stage curtain, library shelves, sports mats |
| **Train / railway station** | upper/middle/lower berths (natural bunk hiding), luggage piles, tea stall, mail bags |
| **Kerala tharavad (nalukettu)** | underside of the wooden kattil, pathayam granary, courtyard pillars, rolled palm-leaf mats, coconut heap, pond steps |
| **Mall** | clothing racks, rows of mannequins (stand still to pass as one), fitting rooms, food-court tables |
| **Hospital** | curtained cubicles, beds with sheets, stretchers, laundry carts |
| **Temple festival / bazaar** | stalls, kudamattam umbrellas, a moving decorated elephant, sack piles, saree racks, autorickshaws |
| **Giant-scale kitchen / bedroom** | a tiny character hiding among plates, shoes and toys |
| **Seasonal** | haunted house with flashlight-only seeker vision (Halloween); Onam, Diwali and Christmas reskins |

Interactive objects that work on any map:

- doors that make noise when opened or closed
- light switches that darken a room
- closets with a seeker search animation
- squeaky floor tiles
- vents and crawl tunnels that reduce the seeker's vision
- a breakable vase as a noise hazard

Gadgets, used sparingly:

- **Seeker:** glue trap, placeable camera and sprint, as in Roblox ([Sportskeeda](https://sportskeeda.com/roblox-news/everything-know-roblox-hide-seek-extreme)).
- **Hider:** decoy clone, smoke, and a short disguise as a prop (a light prop-hunt).

## Conclusion

You are not competing to make a better hide-and-seek game. You are competing on distribution and retention, which means a 2–3 minute loop that players want to repeat, skins and maps that keep them coming back, and a way to reach Tier-1 players. The practical plan has four stages:

1. **Months 1–2:** Build a vertical slice in Unity: a house map, the tilted camera, joystick plus hide button, bot hiders and seeker, cage-rescue, coins, 10 skins and AdMob.
2. **Soft launch:** Release in India and nearby South Asian countries to tune D1 retention (aim for 40%+) cheaply.
3. **Pitch publishers:** Record gameplay video and submit it for CPI tests at Supersonic, Kwalee, Homa, CrazyLabs and Voodoo. Supersonic has published a solo developer in exactly this genre before.
4. **If a publisher passes:** Lean into the Indian-theme niche (train, tharavad, festival maps) and organic growth on YouTube and Shorts.

Add online friend rooms only after retention is proven. Two things are still unverified: current publisher terms and CPI bars, and real eCPMs for South Asia. Check both before committing money.
