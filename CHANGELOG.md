# Changelog

All notable updates to **Apex Eagle Lab (정수리 독수리 연구소)** since the first prototype.
Newest first.

---

## v3.1 · Eagle Farm
- 🌼 **New room: Eagle Farm**: an open room for everyone (no invite code, up to 48), reached from the lobby. A Jeju-style wall of loosely stacked black basalt stones runs all the way around it. Inside are a tall cornfield with a scarecrow, a striped tulip bed, sunflower fields, a veggie patch with big vegetables, a red tractor and a waist-high rapeseed field at the back. The sky and light follow the time of day. Leave through the wooden gate, or tap the wine-red barn (marked with an exit sign) and confirm to go back to the lobby.
- 🐄 **Grazing livestock instead of desks**: on the farm you're one of ten chubby animals with no clothes, just a coloured collar and a big shiny gold bell: spotted cow, brown cow, alpaca, sheep, black sheep, goat, donkey, horse, pig and chicken. The sheep and alpacas are fluffballs, and the chicken walks on two legs. Six animals stand in a ring around each of eight big hay or grass piles. While you focus, they lower their heads to the middle, crown to crown, and munch. On a break, they lift their heads and look around. Name tags sit above their heads. Your farm animal is saved separately from your lab character, and glasses aren't offered on the farm.
- 🥕 **Veggie patch breaks**: on a break, tap the veggie patch and your animal walks over to one of its seven rows. Tap any vegetable to eat it: it hops into your animal's mouth with a "nom nom" bubble and grows back after 2 minutes. You can't go to the patch while focusing.
- 💤 **Naps in the patch**: at the patch, press "Take a nap (5 min)". Your animal folds its legs and lies down with its eyes closed. The camera zooms in and stays there until the 5 minutes are up.
- 👀 On the farm the bench view is called **Farm view**.
- 🎃 **Lab characters**: added pumpkin, made the sweet potato longer and more sweet-potato-like, and moved the cows to the farm.

## v3.0 · Look around the storage
- 🌇 **Library light follows the time**: the library's lighting now matches the window view (day, sunset 6–8 pm, night after 8 pm). The space outside the building is plain black.
- 🏙 **Wider view from the library**: the glass walls show the city from farther away, so the towers look distant. If a library picture is missing, the lab's window view is used instead of a black window.
- 🎓 **Mortarboard sits on top of every head**: the host's cap no longer sinks into big heads like broccoli or mushrooms.
- 🖼 **Fixed the Hall of Fame portrait**: after someone changed character, the portrait could lose its face and lab coat. Shared character parts are no longer cleaned up by mistake.
- 👀 **Look around the reagent storage**: drag left or right to turn and see the shelves on each side.
- 🍺 **Fridge closes again**: tap anywhere on the open fridge to close it.
- 👥 **Friends' online status only in the Friends panel**: the lobby no longer lists who's online. Status is only checked while the panel is open, which also saves reads.
- 🔴 **Friend request count on every Friends button**: the red number now also shows on '👥 Friends' in the reagent storage, counting every request you haven't answered yet.
- 📱 **Simpler iPhone shortcut guide**: removed the icon image download.

## v2.9 · New view from the window
- 🏰 **New 3D Ghent skyline**: the window (and the library's glass walls) now shows an original 3D scene built for this app: three towers, a sea of tiled roofs and stepped gables. Day with clouds, a pink-orange sunset, and a starry night with floodlit towers and lit windows. The scene's source is in `sources/window-view.html`.
- 🧹 **Smoother long sessions**: characters and the trophy portrait now free their 3D memory when they're rebuilt or someone leaves, so the lab doesn't slow down after hours open. The trophy portrait only redraws its hours, not the whole character, every few minutes.
- 🎞 **Smoother battery saver**: when you haven't touched the screen for 8 seconds, the lab now draws 30 times a second instead of 4, so flames and animals stay smooth. Touching or moving the camera brings back full speed right away.
- ⚡ **Lighter buttons**: removed the frosted-glass blur behind buttons and panels (it was redrawn every frame over the 3D view). Panels are slightly more opaque instead.

## v2.8 · Phone-friendly lab
- ⚡ **Faster lab entry**: from the lobby, creating or entering a lab (or the VIP Club) no longer reloads the page. Rooms checked just before a reload aren't checked twice, and your records and chat load in parallel.
- 🏷 **Shorter name tags**: just flag, name and what they're doing (📝 Writing, ☕ On a break, 💤 Napping). Tap a tag to see level, field, today's time, awards and the friend button.
- 📱 **Screen stays on while you focus** (on browsers that support it), so the phone doesn't lock mid-session.
- 🔋 **Battery saver**: when you're not touching the screen, the 3D view redraws less often (4 times a second while focusing).
- ☰ **Menu button on phones**: the top buttons fold into one menu, with a red badge for friend requests.
- Compact room chip, shorter status line and smaller title on phones.
- 🪑 Chairs are easier to tap, and the seat prompt has **Take a free seat**.
- Reagent storage fits portrait screens; the chat box moves above the phone keyboard; zooming into the whiteboard on a phone shows a tip to drag or rotate.

## v2.7 · English that fits
- Signs, posters and labels in the 3D lab now shrink their text to fit, so longer English words no longer run off the edge (e.g. the confocal sign and the reagent storage signs).
- 📱 New eagle icon for iPhone Shortcuts (`sources/shortcut-icon.png`). The **Icon image** button in the iPhone shortcut guide opens it.

## v2.6 · Shorter chat, self-cleaning labs
- 💬 Chat messages now disappear after **12 hours** (was 24).
- 💥 Labs that have been empty for 24 hours are now blown up automatically, even if nobody tries to enter them again. Whenever someone logs in, the app quietly checks for abandoned labs and removes them along with their records and chat.

## v2.5 · Calves join the lab
- 🐄 New characters: **Spotted calf** and **Brown calf** 🐮.
- The eagle no longer has the toy loop on top of its head.
- 🧴 Reagent storage: the biohazard bin moved forward and its lid opens sideways, so it no longer hits the autoclave. Eagle No.1's portrait is updated.

## v2.4 · Pick your task at every session
- **Today's task is chosen when you press Start focus**, every session. Clicking a chair now seats you right away.
- 🇧🇪 "Dutch homework" is now **🌎 Language study**. The textbook is a yellow language book; members living in Belgium keep the Dutch (Nederlands) textbook.
- **Fewer database writes**: your records are saved when you enter, take a break, or leave, not every 5 minutes. While the screen is off, time is kept on your device and saved at the next save point.
- The class motto frame no longer has the red sticker, and yellow buttons use the same font as the others.
- 🧴 Reagent storage: same fonts as the lab (signs and labels in IBM Plex Sans KR), character back to 80% size, biohazard logo printed directly on the orange bin, and the fridge door opens the other way.

## v2.3 · Gloves on, one seat per eagle
- **One account, one place**: opening the same account in another browser or tab disconnects the older one, with a button to switch back.
- **Easier seating**: entering a room asks you to click the chair you want. The seating window now shows your nickname, country and field from sign-up and only asks for today's task, then **Sit at the bench**. The dock button is always **Character**.
- **Language follows your account**: the language you chose is saved to your account and used again on any device.
- 🧤 Every character now wears **light-blue lab gloves**.
- 🧴 **Reagent storage**:
  - Titles use A2Z ExtraLight and everything else A2Z SemiBold.
  - Your character is smaller, so the signs behind stay visible.
  - **My records** fits between the title and the buttons on any screen size, and time by activity opens with a tap.
  - New **portrait of Eagle No.1** (the developer) above the autoclave. Tap it to read the story of the lab.
  - The bin has a proper **biohazard symbol**.
  - Tap the **fridge** to open it. There may be beer cans rolling around. 🍺

## v2.2 · Ready to grow
- Nicknames are now loaded only for the people you actually see: your lab mates, friends and the developer. The app no longer downloads every member's name on each visit, so the cost of opening the app stays flat as more people sign up.
- Finding a friend by nickname looks up that one nickname directly.
- New default nicknames ("Eagle N") use a single member count instead of the full member list.
- Switching rooms remembers your profile, records and recently seen names for a while, so it doesn't fetch them again.

## v2.1 · Phone-friendly focus & lighter data use
- **Pick up where you left off**: if your phone closes the app mid-session, reopening the same room puts you back in your seat and continues your focus session (within 3 hours).
- **Away-time check**: if the screen was off for 20+ minutes during focus, you're asked whether you kept studying. Choose "No" and that time is left out of your focus time, sessions and level.
- Your own leftover connection from before the app closed no longer takes your seat.
- The attendance list is now loaded when you enter a room and when you open Attendance or My journey, instead of streaming every update. People at the bench still update live. This keeps the lab well within the free database limits as more people join.

## v2.0 · Levels, characters & my reagent storage

### ⭐ Levels & awards
- Everyone starts at **Lv.1** and goes up one level for every **10 finished sessions**.
- Awards at **Lv.10** 🥉, **Lv.20** 🥈 and **Lv.30** 🥇. Levels show on name tags, and **tapping someone's name tag** opens their card with level, field and awards (plus the friend button).
- Earlier sessions in each room are counted once, so existing members don't start from zero.

### 🎨 Characters
- The default is a **yellow eagle**.
- Your character, color and new **👓 glasses** are saved to your account and follow you into every room. No more picking them each time you enter.
- Change them anytime: **🎨 Change character** in the reagent storage, or the **Character** button inside a room.

### 🧴 My reagent storage
- Bigger room with a **fridge**, a rattling **autoclave** puffing steam, and a **biohazard bin** for notes to the developer.
- Your character stands in the middle and waves. 👋
- **📊 My records**: days attended, total focus time, sessions, level progress, and time per activity (thesis, reading, Dutch homework, …).
- The view stays fixed, even after opening and closing panels.
- All text in the storage uses the subtitle font. The **iPhone shortcut** now lives only here.

### 🎓 Lab hosts
- The person who created a lab wears a **graduation cap**.

### Smaller things
- The neon sign follows your language ("졸업하고 싶다" ↔ "Please let me graduate").
- The developer menu shows how many people are online right now.

## v1.9 · Name tags, naps & veggie touch-ups
- Name tags (with status) now always float **above each character's head**, in every view.
- **Tap someone's name tag to add them as a friend.** If they already sent you a request, you can accept it right there.
- Friend requests show a **red badge** on the 👥 button and in the lobby.
- **Zzz…** floats above eagles napping in the bed. 💤
- The 🫑 bell pepper is bumpier and chunkier.
- English names: the endive is now **Chicory**, and the neon sign reads **"Please let me graduate"**.
- New home-screen icon: the eagle in the reagent storage.

## v1.8 · Ghent by day and night
- The view of Ghent outside the windows now follows your local time:
  - **6:00–18:00**: daytime
  - **18:00–20:00**: 🌇 sunset sky
  - **20:00–6:00**: 🌃 navy night sky with stars and the towers lit up
- Shared links now show the English name first: **Apex Eagle Club · 정수리 독수리 연구소**.

## v1.7 · Reagent storage, more libraries & iPhone shortcut

### 🧴 Reagent storage
- A new narrow storeroom packed with reagent bottles and boxes, reachable from the lobby **before entering a room**.
- Everything personal in one place: **👥 Friends**, **👤 My account** (nickname, country, field, PIN), **❓ How to use** and **📱 iPhone shortcut**.
- Tap the corners at the back of the room or the buttons at the bottom. **🚪 Back to lobby** takes you back.

### 📚 Library
- **Exit door**: tap the door under the EXIT sign to leave the library.
- **Overflow libraries**: when a library reaches 100 people, a new one opens (Eagle Library 2, 3, …). New arrivals go to the least crowded library.
- Friends can follow you into any library.

### 📱 iPhone
- New **📱 iPhone shortcut** guide: add the lab to your home screen from Safari, or build a Shortcuts-app shortcut for Siri and study-time automations.
- The home-screen icon is now the eagle. The guide also lets you open the icon image to use in a shortcut.

### ✨ Smaller fixes
- Long lists in popups (like the guide) are wider and easier to read: smaller title, and wrapped lines stay indented under their bullet.
- The guide now mentions friends, the reagent storage and the library door.

## v1.6 · Friends & rest options

### 👥 Friends
- Add friends by **nickname**, or tap **[+ Friend]** next to someone in the Attendance "Now" tab.
- Friendships are **mutual**: the other person has to accept. You can cancel, decline or unfriend.
- A badge on the 👥 button shows how many friend requests are waiting.
- The friends list shows each friend's status: ⚪ offline, 🟢 in the lobby, or which lab or library they're studying in.
- **Join a friend without a code**: tap **[Join]** to go straight to their lab or the library. Not available for the 👑 VIP Club.
- Online friends also show up in the lobby, with a Join button.

### 🛏 Rest options
- Pressing **Rest** now lets you choose:
  - **🛏 Go to bed (5-min rest)**: your eagle naps in the bed and the view stays on the bed.
  - **😶 Zone out**: rest at your seat.
- If someone else is already in the bed, only "Zone out" is offered.

---

## v1.5 · New characters & chat cleanup
- New characters: 🌶 red chili, scallion, 🍆 eggplant, 🍄 mushroom, 🌽 corn.
- Chat messages are **permanently deleted after 24 hours**.

## v1.4 · Developer tools & fixes
- The developer menu shows a **badge with the number of pending VIP requests**.
- Fixed: the nickname chosen at sign-up now stays the same when entering a lab.
- When you rest and the bed is free, your eagle goes to the bed, and the view stays on the bed while you nap.

## v1.3 · Lab life
- **Real rain sounds** (CC0, copyright-free).
- Name labels float **above each character's head**, with a **country flag** instead of a color dot. Flags appear next to names everywhere: labels, attendance, chat and member lists.
- New "head to head" message when a focus session starts.
- **← Back** buttons in every side panel.
- **Bed zoom**: a 5-minute nap with a "Back to reality" button.
- More things to zoom into: fume hood, culture room, codon poster, Western blot poster, photo wall.
- **Feedback via the biohazard bin**: write a note, crumple it and throw it in. 🗑
- The whiteboard notice can only be edited by the developer (zoom in, then click the board).
- New 🛠️ developer menu with feedback, VIP requests and the member list.
- **Onboarding guide** for new members.

## v1.2 · The big lab update
- A popup explains the focus session before it starts, and asks for confirmation if you try to quit a session halfway.
- 🔥 **Fire effect** for eagles on a focus streak.
- The timer now shows "until next rest or focus".
- "Care" is renamed **"Feed"**. 💦 Water plants and 🫘 feed animals directly when you're close to them.
- The window now has a real city view.
- The neon sign can be edited by anyone in the lab.
- 🎶 **Ambient sounds**: white noise, gentle music and rain.
- 😠 **Angry button**: your eagle waves its arms.
- New lab details: bed, coffee, piles of papers, codon poster, photos and a Western blot poster.
- 📚 **Library**: a big shared study room with 100 seats. No code needed.
- Screenshots (📸 Capture) no longer include popups, and your name appears under the title.
- Empty labs are **deleted after 24 hours** with no one inside. The lab owner can leave freely.

## v1.1 · Lobby, rooms & languages
- **Korean / English**: choose at first launch, switch anytime in settings.
- **New lobby** with three options:
  - **Create a new lab**: you get a 6-character code to share.
  - **Enter a lab with a code**: open labs are not listed, so you can only join with a code.
  - **👑 Eagle VIP Club**: only for members approved by the developer.
- Sign-up asks for your **country** (shown as a flag) and **field of study** (shown while you focus).
- Nicknames can be up to 20 characters. The default English nickname is "Eagle N".
- English title: **Apex Eagle Lab**.
- **Leave lab** button in the room, and you can also leave by opening the door to the hallway.
- Water and feed plants and animals directly when you walk up to them.
- The monthly top-studier frame can be zoomed in.
- Bigger rapeseed flowers, fully visible up close.
- Link preview thumbnail for sharing on KakaoTalk, Notion and other apps.

## v1.0 · Public launch
- Moved from a single prototype to a public website on **GitHub Pages** with **Firebase**.
- Accounts with a nickname and a 4-digit PIN, so you can log in from any device.
- Study records, chat and presence are shared live between everyone in the lab.

## v0.1 · First prototype
- A 3D lab where eagles sit together at a bench and study head to head.
