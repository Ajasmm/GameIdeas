# Ludo Tactics Run game design

Nov 23, 2026 · @PAAKKAAN

Ludo Tactics Run is Ludo with a roguelike run and tactical pieces, with no story. It is a paid Steam game for one player against AI, with same-screen and online friend play as extras. The name is a working title until a Steam check is done.

## Pitch

**One line:** roll two dice, choose which piece gets which number, cut your rivals, and build a crazy upgrade combo across 8 boards.

**5-second clip hook:** a horse piece jumps over two enemies, lands on a fire square, and three rival pieces fly back to base as the score multiplies.

## How this game stays different

The closest existing game is [Ludaro](https://store.steampowered.com/app/3613030/Ludaro/) by EvolX Games: a 1v1 Ludo card battler with health, damage and status effects, free with ads on [Google Play](https://play.google.com/store/apps/details?id=com.evolxgames.ludaro&hl=en_IN) and planned for Steam in 2026. Our game is real 4-player Ludo with roguelike upgrades, so every rule below keeps us out of the card-battler lane.

|  | Ludaro | Our game |
| --- | --- | --- |
| Format | 1v1 duel with health and damage | Classic 4-colour Ludo race |
| Core skill | Cards and status effects | Two dice; you choose which piece gets which number |
| Pieces | Pawns with powers | 5 roles you can read by shape (horse, guard, elephant, runner, thief) |
| Rewards | Reward wheel, card packs | Shop: pick 1 of 3 upgrades you can see on the board |
| Friends | Online 1v1 PvP with leagues and chests | 2 to 4 on one screen, plus Steam invites |
| Business | Free with ads on mobile | Paid, no ads, fully offline |
| Look | 2D | Low-poly 3D board with physical dice |

**Do:**

- Keep the win rule as pure Ludo: bring all 4 pieces home first. A cut only sends a piece back to base.
- Make the two-dice choice the headline rule in the trailer, the store text and the tutorial.
- Put every upgrade on the board where the player can see it: a different die, a changed piece, a coloured square.
- Treat same-screen play for 2 to 4 people as a main feature, not an extra. Ludaro cannot offer this.
- Lead the store page with one line: real Ludo with friends on one screen, plus roguelike upgrades.
- Show the 3D cut moment (pieces flying back to base) in the first second of every clip.

**Do not:**

- No health bars, damage numbers, poison, freeze or bleed.
- No card deck or hand of cards. Charms are passive rules, shown as small tokens beside the board.
- No reward wheel, chests, leagues, hero unlocks through grind, or anything that looks like a free mobile game.
- No ads and no in-app purchases.
- Do not use the words "deckbuilder" or "card battler" in tags or store text.

Wishlist Ludaro and watch its Steam launch. Its review count will show how much demand a Ludo roguelike has before our build is finished.

## Core rules

The rules take about one minute to learn.

- There are 4 colours, each with 4 pieces. Bring all your pieces home to win the board, the same as Ludo.
- You roll 2 dice each turn. You choose which piece uses which number, or give both numbers to one piece. This is the main tactics rule: less luck, more thinking.
- A 6 on either die opens a piece from base.
- Landing on an enemy cuts it back to base. Safe squares (stars) protect pieces, the same as Ludo.
- Each board has a turn limit. If you do not finish in time, the run ends. This is the roguelike pressure.

## Piece roles

You start with 4 basic pieces and unlock roles during the run. Launch has 5 roles.

| Piece | Power | Weakness |
| --- | --- | --- |
| Runner | +1 to any number it uses | Easy to cut |
| Horse | Jumps over pieces without being blocked | Cannot cut on a jump |
| Guard | Blocks the lane; enemies cannot pass | Moves only up to 3 |
| Elephant | Pushes the piece in front back 3 squares | Slow (half movement) |
| Thief | Steals 1 coin each time it cuts | Goes home if cut |

## A run

One run takes about 25 to 35 minutes.

1. Choose a starting set, for example Speed (2 runners) or Wall (2 guards).
2. Play 8 boards against AI opponents. Boards 3, 6 and 8 are boss boards.
3. After each board, go to the shop. You earn coins from cuts, from finishing fast, and from pieces brought home.
4. Choose 1 of 3 offers.
5. Between boards, choose the next stop on a map: normal board, elite board (harder, better reward), shop, or a mystery event.
6. If you lose, the run ends. You unlock new pieces or charms for next time.

Upgrades come in four types:

| Type | What it changes | Examples |
| --- | --- | --- |
| Dice | How you roll | Loaded die (choose a number once per board), double die, a 6 opens 2 pieces |
| Piece | One of your pieces | Change its role, give it an extra life |
| Board | Squares you own | Fire trap, speed lane, rent square (enemies who land lose a turn or pay coins) |
| Charm | A passive rule | Every cut gives x2 score, guards also cut |

The board upgrades are where the property idea lives. It is one upgrade type, not a full Monopoly system, so the rules stay simple.

## Boss boards

Each boss board has one special rule, shown before the board starts.

- **Flood board:** the outer lane sinks every 3 turns.
- **Mirror board:** the enemy copies your last move.
- **Snake board:** some squares slide you backwards.
- **Rotating board:** home entrances shift.
- **Champion:** the enemy also has role pieces and upgrades.

## Modes

Every mode works offline except online friend play.

| Mode | Players | Notes |
| --- | --- | --- |
| Run | 1 against AI | The main product |
| Daily run | 1 against AI | Same seed for everyone, global leaderboard, needs no live players |
| Local party | 2 to 4 on one screen | Against each other or the AI; each player drafts upgrades between boards |
| Online | 2 to 4 friends | Steam invite, one player hosts, no public matchmaking at launch |

The AI has three levels: Easy, Normal and Cunning. Cunning cuts aggressively and blocks with guards.

## What players like

Each feeling below is borrowed from a game that already proved it.

| Feeling | Borrowed from | How it shows up here |
| --- | --- | --- |
| Combo explosion | Balatro | Charms stack: cut = x2, fire square cut = +5, thief steals |
| Revenge and betrayal | Ludo, Mario Party | Cutting a piece that is one square from home |
| Clever over lucky | Into the Breach, chess | Two dice and the choice of which piece gets which number |
| Rent sting | Monopoly | Your trap squares hurt others, in a short match |
| One more run | Slay the Spire | Unlocks and different builds each time |

The design also fixes Ludo's three biggest complaints: too much luck, games that run too long, and nothing to do while waiting for a 6.

## Rules help and tutorial

A player should never be stuck on a rule.

- Board 1 is the tutorial, in 3 steps: roll, assign dice, cut.
- Hold or hover on any piece, square or charm to see a short explanation.
- A "?" button shows the current board's special rule at any time.
- Before you confirm a move, the game previews where each piece will land and who gets cut.
- Localisation is text only, with no voice: English, Hindi, Malayalam, Tamil, Spanish, Portuguese, Simplified Chinese, Russian and German.

## Look and feel

The game is a low-poly 3D board on a table, with chunky wooden pieces.

- Physical dice roll on screen.
- Pieces fly off and bounce back to base when cut. This is the best clip moment.
- Each boss board has its own colour and setting: a village courtyard, a monsoon roof, a temple floor, a train compartment.
- All art, music and store images are hand-made or bought, not AI-generated, to avoid the Steam AI label.

## Scope

The estimate is 4 to 6 months for single-player and local play, plus 1 to 2 months for online friend play. Price is about $7.99 to $9.99, with a free demo of the first 3 boards. Both are estimates.

**Launch content:** 5 piece roles, about 40 upgrades and charms, 8 board types, 5 bosses and 3 AI levels.

| Who | Builds |
| --- | --- |
| Claude Code | Rules engine, AI, shop, save system, daily seed, localisation tables, help screens |
| Ajas | Boards, pieces, dice, animations, game feel, clip moments |

## Risks and checks

Do these checks before starting the build.

- [x] Search Steam for "ludo roguelike", "ludo tactics" and "dice board roguelike", and open the existing "Ludo Tactics" page. The earlier check was a limited search.
- [ ] Pick a final name that no other Steam game uses.
- [ ] Test the rules with someone who has never played, and keep roles to 5 at launch.
- [ ] Make the Cunning AI feel smart, not cheating. Show its dice openly.

Two more risks to plan for:

- Ludo is not well known outside South Asia. Describe it in store text as "the classic race board game" (Parcheesi in the US), and show gameplay in the first second of the trailer.
- Ludo, chess, and the ideas of buying squares and charging rent are free to use. Do not use the Monopoly name, board design, money look or character art. This is general information, not legal advice.
