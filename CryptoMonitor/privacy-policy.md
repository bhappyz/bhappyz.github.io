---
title: Crypto Monitor privacy policy
---

# Crypto Monitor privacy policy

_Last updated: 6 September 2026_

Crypto Monitor is a free Android app that shows cryptocurrency
prices from public exchange APIs and raises alarms when a price crosses a line
you set. This page explains what the app does with data. The short version:
**the app has no account system, no analytics, no advertising and no server of
its own. Everything you enter stays on your phone.**

## What the app stores on your device

The following is kept in the app's private storage on your phone only. It is
never uploaded anywhere, and it is deleted when you uninstall the app.

- The pairs you watch and the exchange each one comes from.
- Alarms you set and the log of alarms that fired.
- Recent prices and today's candles, kept so the chart and the change since
  open work offline.
- Your settings (refresh intervals, sounds, voice announcements, background
  mode, the exchange-list update URL).

You can clear all of it at any time from Android's _Settings > Apps > Crypto
Monitor > Storage > Clear storage_.

## Network requests the app makes

The app talks directly to two kinds of servers. As with any internet request,
those servers can see your IP address and the time of the request.

1. **Cryptocurrency exchanges.** To fetch a price, the app calls the public,
   unauthenticated market-data endpoint of the exchange you chose (for example
   Binance, Kraken or Coinbase). The request contains only the trading pair
   symbols you asked for. No exchange account or API key is involved. Each
   exchange has its own privacy policy governing what it logs.
2. **The exchange-list update.** About twice a day the app checks a small
   JSON file on the app's website (hosted on GitHub Pages) for an updated
   list of exchange endpoints. You can change or disable this in
   _Settings > Exchange list_.

The app does not contact any other server. It sends no crash reports, no
usage statistics and no device identifiers.

## Permissions and why they are needed

| Permission | Why |
|---|---|
| Internet | Fetch prices from exchanges and the exchange-list update. |
| Notifications | Show price alarms and, if you opt in, a persistent price row. |
| Vibrate | Alarm feedback. |
| Run at start-up | Re-arm scheduled background refreshes after a reboot. |
| Foreground service (special use) | _Live_ background mode: keeps checking prices at your chosen interval while the app is closed, with a visible notification. |
| Wake lock | Finish a refresh that started while the screen was off. |
| Ignore battery optimisations | Optional. Offered in Settings so _Live_ mode is not stopped by the system on phones with aggressive battery management. The app works without it. |

The app does not request location, contacts, camera, microphone, storage or
any advertising identifier.

## Voice announcements

Prices read aloud use the text-to-speech engine already installed on your
phone (usually Google's). The text is sent to that engine on the device. If
the engine you chose synthesises speech in the cloud, its own privacy policy
applies.

## Children

The app is not directed at children and collects no personal data from anyone.

## Changes to this policy

Any change will be published on this page and noted in the app's release
notes. Because the app collects nothing, changes are expected to be rare.

## Contact

Questions about this policy: <cryptomonitorapp@proton.me>
