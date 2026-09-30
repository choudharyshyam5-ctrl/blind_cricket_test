# Blind Cricket Pro Ultimate

An audio cricket game for the browser, with spoken commentary, screen-reader announcements, team matches and a virtual cricket career.

## Play

- [Live game](https://choudharyshyam5-ctrl.github.io/Blind_cricket/)
- [Test build](https://choudharyshyam5-ctrl.github.io/blind_cricket_test/)

No installation is needed. Google sign-in and cloud features need an internet connection. "Offline" match modes mean playing against the computer, not a guarantee that the whole website works without internet.

**Test-build warning:** the test site currently uses the same Firebase project as the live game. Use a separate test Google account and browser profile, not your main progress account or the phone holding unsynced progress.

This README describes the test INDEX checked on September 30, 2026. New features listed here should not be assumed to be available on the live game until the tested build is promoted. Firebase features also need the matching published security rules.

## How to play

1. Open the game and select **Continue with Google**.
2. Choose **Play versus computer**, or create a squad and choose **Team versus computer**.
3. Set the format, overs and wickets where available. Choose your toss call and start. The toss winner chooses batting or bowling.
4. When batting, select a shot from **0 to 6 runs**. The selected runs are scored unless you are out. Higher-scoring shots have a higher wicket risk.
5. A B1 batter scores double the selected runs. In team mode this follows the batter on strike; outside team mode it follows your profile category.
6. When bowling, choose **Straight**, **Yorker**, **Bouncer** or **Spin**.
7. At the end, read the result and select **Download Scorecard** for a text scorecard.

Formats include short matches, T20, One Day and Test. Test matches use four innings, a shared 450-over limit, declarations, follow-on decisions and possible draws.

### Teams and player records

Open **Menu > My Squad** to build an 11-player XI. Set each player's name, B1/B2/B3 category and role: Batsman, Bowler, Allrounder or Wicketkeeper. The test build requires at least 4 B1 and 3 B2 players, with no more than 4 B3, plus enough eligible bowlers for the format.

- After a wicket, **Choose your batter** lists the remaining players.
- At the start of each over, select an eligible bowler before continuing.
- Bowlers have format limits, including 4 overs in T20 and 10 in 50-over One Day matches.
- Strike changes on base shot results 1, 3 and 5, and at the end of an over.
- **Download Scorecard** includes individual batting and bowling for both sides and a Player of the Match chosen from your XI.
- **Menu > XI Records** shows records from completed team matches. These records are private to your signed-in account.

**Team Create** creates a team name and ID. The ID is not yet an online invitation or a shared coach/owner progress dashboard. Opponent squads and historical season names are computer simulations, not claims about real players' blind-cricket classifications. A basic **Coach Profile** is available from level 4.

## Career, challenges and tournaments

Play matches to earn XP, virtual match rewards, salary and career unlocks. Career progress depends on the requirements shown in **Career**, not only on XP. The profile tracks match and format records, and career rewards can add collection items.

- **Daily Challenge:** one three-over target, with one virtual bonus per day. Targets grow with career level.
- **Friend challenges:** players make separate attempts against the computer and compare scores. This is not real-time multiplayer.
- **Offline Tournaments:** win three computer-match rounds. A loss or quit ends the tournament. Unlock requirements and virtual prizes appear on each entry.
- Tournament choices include India A, Asia Cup, World Cup, simulated IPL seasons and other leagues, subject to their unlock requirements.
- **IBPL Auction / Owner Mode**, from level 6, is a simulated player-buying screen with a separate virtual budget. It is not a live auction or a complete owner-management season.

## Shop and collections

Use **Shop** to buy cricket items with your virtual wallet. Prices change with career level. **My Collection** shows owned items and durability. Equipment is collectible; gameplay stat bonuses are not implemented yet.

To gift or sell an item to another player:

1. Enter their **Player ID**, select **Look up Player ID**, and check the displayed name.
2. Choose gift or sale, check the virtual sale price and confirm the offer.
3. The item is reserved while the request is pending.
4. The recipient opens **Shop > Item requests** and accepts or declines. Accepted sales transfer virtual money and the item; declined requests return the reserved item.

Gifts do not yet arrive automatically in the recipient's collection. Item-sale offers do not yet appear as a **Buy** notification. The current flow uses Shop requests. Selling an item back to the game is a separate option.

## Virtual life and investments

Build a life around your cricket career. Start with small purchases, earn virtual match rewards and salary, then work towards your first apartment or a business with your own brand name. You can keep a home, rent out an extra house and build a collection of virtual properties and businesses as your career level rises.

Open **Menu > Virtual Life**, or follow the link in Shop.

All money, rent, profits, rewards and purchases are virtual. Nothing can be withdrawn or exchanged for real money. There is no real investment or payment service.

### Getting started

1. Play matches to build your virtual wallet and career level.
2. Open Virtual Life and check the catalog. Each item shows its price and required level; you need both enough money and the right level.
3. Choose an asset and review the confirmation. Small purchases include headphones and an energy drink pack. Later unlocks include a bike, apartment, house, villa, car, branded cloud kitchen, cafe, academy, hotel and sportswear company.
4. For a business, first enter your brand name in **Business brand name**. Buying your own business is supported; investing in another player's hotel is not yet supported.
5. Check **Own assets** and the recent virtual transactions after buying. You can sell an asset back to the game, or rent out an extra house once you have a home to keep.

For example, an apartment costs virtual ₹40,000 at level 4. A family house costs virtual ₹1,20,000 at level 5. If you own both, keep one as your home and rent out the other. Renting the ₹40,000 apartment makes it eligible for virtual ₹240 monthly income. These are game rules, not real property prices or returns.

### Income and value

- Keep one personal home before renting out an extra house.
- Rented houses earn 0.6% of catalog cost per eligible month.
- Businesses earn 0.4% of catalog cost per eligible month.
- Monthly income is credited once in an India calendar month when you open the game, capped at virtual ₹1,00,000. Missed months are not paid later.
- Selling an asset back to the game pays 60% of catalog cost.
- Virtual net worth is wallet balance plus the catalog value of owned life assets. It is not the amount you would receive by selling everything.
- Recent virtual transactions appear in Virtual Life.

Player-to-player property shares and investment in another player's business are not implemented.

## Leaderboards and privacy

**Top 10 leaderboard** is an opt-in ranking by match wins.

**Richest cricketers** has a separate opt-in under the leaderboard screen. It shares your name, virtual net worth and house, hotel and business counts. Turning on the older match leaderboard does not turn on wealth sharing.

Public **Player lookup** is a separate profile setting, enabled by default in this build. Players can turn it off. Lookup is used to check recipients before sending item offers.

Wealth sharing needs the matching Firestore rules. If saving or sharing fails, read the error and check cloud status; do not assume that a checked box means the choice was saved.

## Audio and accessibility

Settings include text-to-speech, commentary, sound effects, background music and volume controls. Commentary packs include English, Hindi, Urdu, Telugu, Tamil, Kannada and Bengali; individual clip coverage varies. Screen-reader announcements and text commentary remain available.

Match shortcuts include **B** to bat, **Ctrl+B** to bowl and **A** for an accessibility summary. Buttons can also be used directly. Mobile browser or screen-reader shortcuts may differ.

## Save, resume and recovery

Use the same Google account to return to your progress. **Resume Saved Match** appears on Home or in the Resume menu when a valid checkpoint is available. An active offline tournament can also be continued.

A phone copy and cloud copy can differ. The build stops conflicting full-profile saves rather than silently replacing cloud progress. Compare the displayed copies before choosing recovery. Recovery is a deliberate replacement with a backup, not an automatic merge of both histories, and needs matching security rules.

**If your phone has unsynced progress, do not clear browser/site data or log out to troubleshoot.** Keep that copy until the save problem is checked. A local checkpoint is not proof that its cloud save succeeded.

## Feedback, notifications and admin

Signed-in players can use **Feedback / Query** to send a message to the game owner. The message includes the signed-in name and email.

The admin page lists saved player profiles and feedback. Admin can send one reply per feedback entry. The player reads that reply in **Notifications**, alongside incoming friend challenges, and can mark it as read.

These are in-game notifications while the page is open, not browser push notifications when the game is closed. Admin update/announcement broadcasts are not included in the current test INDEX.

## Pending work

These are pending or deferred ideas, not a release-date promise:

- Admin update/announcement broadcasts.
- Automatic gift delivery and sale notifications with a Buy action.
- Player-submitted commentary/sound uploads with review before use.
- Expanded individual player profiles and coach/team-owner progress views by team ID, including following multiple teams.
- Larger tournament squads with selection of a playing XI.
- Tour travel/progression and a fuller post-international league/owner system beyond the current simulated entries.
- Player-to-player property/business investment.
- Closed-page browser push notifications are not included in the current no-paid-features build.

Before promoting the test build, check sign-in, published rules, saves and recovery, wealth sharing, team matches, scorecards, item trades and sounds with separate test accounts.

## Deployment notes

This project uses an `index.html` browser app, GitHub Pages, Firebase Authentication and Firestore. Uploading a new INDEX does not publish Firestore rules.

Compare the currently published rules before changing them: the live and test sites share a Firebase project. Check that the test Pages domain is allowed for sign-in. The current test build uses the live repository's sound files; restore the intended relative sound root when promoting the INDEX to production.

This README can be saved as **README.md** in the repository root. Updating it does not enable any pending feature.

## Sound credits and contact

Sound effects and commentary clips were collected from various different online sources to make the game enjoyable for the blind cricket community. No copyright infringement is intended. If you own a sound used here and want it removed, please contact the game owner through **Feedback / Query** so it can be reviewed and removed.

For any feedback, question or sound-removal request, sign in, open **Feedback / Query**, write your message and select **Submit**. The game owner can reply in your in-game Notifications.
