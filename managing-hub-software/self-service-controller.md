---
title: "Self-Service (Kiosk) Controller"
excerpt: "The self-service controller is for unattended environments"
toc: true
---

The self-service (kiosk) controller is designed for environments where customers/players manage their own games.

## Using Kiosk Mode

## Changing Game Defaults

## Adding Credits

A self-service controller can be run in free play mode, where there's no cost to play. It can also use a credits-based system, where players must swipe a game card, pay with a credit card, or insert bills or coins.

Each device that can collect credits must be connected to the MagneTag system in a similar way to armor vests. Each device must be assigned to the specific controller that the credits will count towards. A single station may have multiple credit devices, like both a bill reader and coin-op device.

Each device grants credits in different ways. For instance, a credit card reader may just grant 1 credit for the full game cost; a coin-op device may provide different numbers of credits for different types of coins (e.g. 1 credit for a nickel, 5 credits for a quarter, etc.).

When using a credit system, the configuration looks something like this:

```
"CreditsPerMatch": 3,
"CreditsMultiplier": 0.25,
"CreditsFormatString": "0.00",
"CreditsNoneHeading": "Please insert $%CreditsNeeded% to begin playing.",
"CreditsNoneMessage": "",
"CreditsPartialHeading": "Please insert $%CreditsUnpaid% to begin playing.",
"CreditsPartialMessage": "It costs $%CreditsNeeded% to play, and you've paid $%CreditsPaid% so far."
```
