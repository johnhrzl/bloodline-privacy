# Bloodline – Privacy Policy

Public privacy policy for the Android game **Bloodline**
(package `com.john.bloodline`), required by the Google Play Console.

Live page: https://johnhrzl.github.io/bloodline-privacy/

## Kept in sync with the app

The Play Console cross-checks this document against the Data Safety form.
Contradictions between the two are a common reason for rejection, so when the
app's data handling changes, this page changes with it. Currently declared:

- no account with us, no password, no server of ours
- the save game lives on the device — and, **if the player is signed in to
  Google Play Games**, as a copy in that player's own Google account, which we
  cannot read or delete
- **Google Play Games Services** as an independent controller (player ID,
  public player name, submitted scores and achievements)
- Google AdMob as an independent controller (advertising ID, approximate
  location from IP, device and usage information)
- one full-screen ad that is **not** optional: after a death, once an heir has
  been chosen
- optional analytics via **PostHog** (EU servers, processor under a DPA), off
  until the player agrees, tied to a random identifier and nothing else
- **Firebase Crashlytics** for crash reports, behind the same consent switch
  as the analytics above – error, Android version, device model, nothing else
- an in-game **bug report** the player composes and sends from their own mail
  app; the game itself transmits nothing, and the full text is shown before
  sending
- eight Android permissions after the manifest merge — `INTERNET`,
  `ACCESS_NETWORK_STATE`, `AD_ID`, three `ACCESS_ADSERVICES_*`, `WAKE_LOCK`,
  `FOREGROUND_SERVICE` — all classed **normal**, none of them a runtime prompt,
  all but the first two contributed by Google's advertising library
- intended for players aged 18 and over

Controller details match those used for AI Tycoon.

### Data Safety must say the same

The one row that changed with cloud save: **save game — collected: yes,
shared: no, purpose: app functionality.** "Collected" because the data leaves
the device; "not shared" because it goes to the player's own Google account
and not to a third party for that party's own purposes.

## Why this is a separate repository

The game's source is not public. This repository contains nothing but the
policy page, so publishing it exposes no code — only the document that has to
be publicly reachable anyway.
