---
title: Keeping a US Phone Number Alive from Japan
tags: [phones, 2fa, before-departure]
date: 2026-09-12
updated: 2026-09-12
---

When you move to Japan you lose your US phone number unless you actively keep it alive. This matters because a large number of banks, brokerages, and online services use SMS-based two-factor authentication (2FA) tied to a US number — losing that number can lock you out of accounts until your next US trip. A live US number also doubles as sufficient coverage for annual visits back.

This must be set up **before leaving the US**.

## The Core Mechanism: Wi-Fi Calling, Not Roaming

The right approach is a **real US carrier SIM with Wi-Fi Calling enabled**, not international roaming and not a VOIP number.

With Wi-Fi Calling active, your phone treats any internet connection (your Japanese carrier's data or any Wi-Fi) as the carrier signal. Bank 2FA texts arrive exactly as they would in the US — at no roaming cost. This is the setup expat and prepaid-carrier communities consistently recommend.

**Why a real SIM beats VOIP for 2FA:** Banks and financial institutions increasingly block SMS short-code messages (the 5–6 digit OTP codes) to VOIP numbers. Real-world reports confirm Chase, Ally, and Wells Fargo have refused Google Voice for 2FA. A real MVNO SIM carries "carrier trust" and receives short codes normally.

## What is an MVNO?

An MVNO (Mobile Virtual Network Operator) is a carrier that does not own its own cell towers. Instead it leases access to the infrastructure of a major carrier (AT&T, Verizon, or T-Mobile) and resells it under its own brand, typically at a lower cost and without long-term contracts.

For expat purposes, MVNOs are attractive because they offer the same "carrier trust" as the major networks — meaning banks and financial institutions treat their SIM numbers the same as a Verizon or T-Mobile number — while being far cheaper for a mostly-dormant line. The tradeoff is that customer support is thinner and some features (like Wi-Fi Calling compatibility across all handset models) can be inconsistent depending on which underlying network the MVNO uses.

## Carrier Options

Run the US number as a **secondary eSIM** alongside your Japanese carrier's SIM, with data roaming off. The US line handles voice and SMS; your Japanese SIM handles data.

| Carrier | Network | eSIM | Dormant cost | US-visit plan | 2FA reliability | Notes |
|---|---|---|---|---|---|---|
| **[Tello](https://tello.com)** | T-Mobile | Yes | $5/mo (300 min, no data) | Upgrade month-to-month | Strong | Best all-around fit; easy toggling; expat-recommended for banking 2FA |
| **[US Mobile](https://usmobile.com)** | Verizon / AT&T / T-Mobile (choose) | Yes | Low | Upgrade month-to-month | Good (test first) | Network flexibility is useful if your US destination has weak T-Mobile; verify bank 2FA before moving |
| **[Mint Mobile](https://mintmobile.com)** | T-Mobile | Yes | Moderate | Included in plan | Strong | Plans sold in multi-month blocks — less flexible for a mostly-dormant line |
| **[Ultra Mobile PayGo](https://www.ultramobile.com/paygo/)** | T-Mobile | **No** (physical SIM only) | Lowest | Limited top-ups only | Good | Cheapest option but physical SIM only is a drawback for a secondary eSIM setup |
| **[Google Voice](https://voice.google.com)** | VOIP | N/A | Free (one-time port fee) | No cellular | **Weak / risky** | Not recommended as a primary 2FA line; many banks block it |

**T-Mobile-network MVNOs are generally preferred** for Wi-Fi Calling from abroad — T-Mobile tends to be more permissive than AT&T/Verizon when it comes to Wi-Fi Calling working on a range of handsets overseas. US Mobile is an exception since it lets you choose the underlying network.

**Avoid the "Snooze" / number-parking options** some carriers offer — these typically suspend your plan entirely, meaning you won't receive SMS at all. Keep an active talk/text plan to receive 2FA.

**Google Voice and NumberBarn** are cheap but VOIP-based. Treat them as secondary numbers only, never as your primary 2FA channel.

## Recommendation

**Tello on T-Mobile** is the most straightforward fit: low dormant cost, eSIM support (including re-provisioning from Japan), strong 2FA track record, and simple month-to-month toggling to a fuller plan for US visits.

If your US visits take you to areas with poor T-Mobile coverage, **US Mobile on Verizon** is the stronger alternative — but verify that your specific banks accept 2FA from that line before you move.

## Before-Departure Action Plan

1. **Choose a carrier and port in your existing US number.** Porting in is important — don't let your current number lapse before porting.
2. **Activate as an eSIM** so it runs as a secondary line alongside your Japanese SIM.
3. **Enable Wi-Fi Calling** and register a US E911 address (required by US carriers for Wi-Fi Calling; a friend or family member's address works).
4. **Test 2FA in airplane mode + Wi-Fi only.** Put the phone in Airplane Mode, connect to Wi-Fi, and trigger a real 2FA code from each of your banks and critical services. Confirm it arrives. Do this before you leave.
5. **Move as many accounts as possible to authenticator-app (TOTP) 2FA** (e.g. Google Authenticator, Authy) or a hardware key. The SIM remains your fallback for institutions that only support SMS.

## Caveats

- **2FA over Wi-Fi from abroad is not 100% guaranteed for every bank.** Short-code delivery depends on how each bank's SMS aggregator routes to the MVNO's network. Always test with your actual institutions before relying on it.
- **Prices change frequently** — especially promotional rates. Verify current pricing at signup.
- **US payment method:** Some MVNOs require a US credit/debit card or US billing address. Confirm requirements before moving and keep a US card active.
- **Activating from abroad is harder.** Some carriers restrict new activations from outside the US. Set everything up before departure. (Tello is known to support overseas activation; others may require a VPN.)

## References

> ⚠️ Claims marked **[unverified]** could not be confirmed directly from the carrier's website at time of writing — the sites blocked automated access. Verify manually before relying on specific plan details.

| Source | Link | What it covers | Status |
|---|---|---|---|
| US Mobile plans | [usmobile.com/plans](https://usmobile.com/plans) | Three networks, eSIM, Wi-Fi Calling included, no-contract | ✅ Verified |
| Tello | [tello.com](https://tello.com) | T-Mobile network, eSIM, Wi-Fi Calling, $5/mo plan (300 min, no data) | ✅ Verified |
| Mint Mobile plans | [mintmobile.com/plans](https://mintmobile.com/plans) | T-Mobile network, eSIM, multi-month plan structure | ⚠️ Unverified |
| Ultra Mobile PayGo | [ultramobile.com/paygo](https://www.ultramobile.com/paygo/) | T-Mobile network, $3/mo PayGo, physical SIM only | ⚠️ Unverified |
| Google Voice | [voice.google.com](https://voice.google.com) | VOIP, port-in fee, no short-code guarantee | ⚠️ Unverified |
| Howard Forums | [howardforums.com](https://www.howardforums.com) | Community discussion on T-Mobile MVNOs for Wi-Fi Calling abroad | ⚠️ Unverified — no specific thread linked |
| Bogleheads forum | [bogleheads.org/forum](https://www.bogleheads.org/forum/index.php) | Expat phone/2FA discussion | ⚠️ Unverified — no specific thread linked |
