# 2026-04-28: ISOC SPI 2026 late-lodgement strategy

## TL;DR

RISE missed the SPI 2026 deadline (23 April 21:00 UTC). The cause was a misunderstanding that the 1-page Fluxx registration form was the application itself. It was not. The actual SPI grant application is a separate multi-page form behind a login, requiring completion before the deadline. Only the registration was completed; the application form was never opened.

Companion file `2026-04-28-isoc-spi-late-lodgement-drafts.md` contains the three letters drafted for sending.

## What is on the record (Gmail, gio.bacareza@rise.ph)

- **22 Apr 15:27 UTC** "New Registration Received - Internet Society Foundation" from `do-not-reply.grants07-us-east-1@fluxx.io`. Body: "Thank you for submitting your registration information. Internet Society Foundation staff will review your registration within 1-2 business days."
- **22 Apr 15:39 UTC** Gio sent expedite email to `grants@isoc.foundation` (typo'd domain, see Failure Analysis). Subject: "Registration review – expedite request – SPI 2026."
- **22 Apr 15:48 UTC** Gio emailed `fluxx_help@isocfoundation.org` saying "I recently submitted a grant application... reset password failed." Ticket 4525:2175959.
- **22 Apr 15:48 UTC** Auto-ack from Fluxx Helpdesk.
- **22 Apr 16:48 UTC** "New User Information" from Fluxx with personalized password setup link. Arrived 1 hour after Gio had already escalated to support; Gio was in support-channel mode and did not act on it.
- **22 Apr 16:49 UTC** "Registration Completed" notification from Fluxx.
- **22 Apr 16:49 UTC** Evan (`fluxx_help@isocfoundation.org`) replied: "I saw you submitted a registration which I've approved which will create your user account."
- **23-25 Apr** Three Gmail delivery-failure notifications for the bounced expedite email to `grants@isoc.foundation`.
- **24 Apr 00:51 UTC** Fluxx password-reset email after Gio's first successful forgot-password attempt.
- **24 Apr 00:55 UTC** Gio first logged in. Could not find any application. Wrote: "upon logging into the portal, I am unable to locate my application."
- **24 Apr 13:04 UTC** Evan replied: "To start an application, navigate to the 'Application and Grants Portal'..."
- **26 Apr 23:35 UTC** Gio replied: "I thought you had accepted the application..."
- **27 Apr 14:04 UTC** Evan replied (decisive): "Registrations are separate from applications. Registrations are only to gain access to the portal whereas the application forms is what you would use to apply for grants. So as of now you do not have any application started or submitted, but given your registration was approved and account created - you can login and start one."
- **28 Apr 05:50 UTC** Gio drafted reply (still in Drafts, not sent): "Oh no! I have misunderstood..."

## Corrected timeline (plain English)

| PHT (Gio local) | UTC | Event |
|---|---|---|
| 22 Apr 23:27 | 22 Apr 15:27 | Gio submitted the 1-page Fluxx registration form. Past Claude framed this as "that's it, wait." |
| 22 Apr 23:39 | 22 Apr 15:39 | Past Claude drafted, and Gio sent, an expedite email. Address was typo'd by past Claude as `grants@isoc.foundation` instead of `grants@isocfoundation.org`. |
| 22 Apr 23:48 | 22 Apr 15:48 | When login would not work, Gio opened a Fluxx help ticket (4525:2175959). |
| 23 Apr 00:48 | 22 Apr 16:48 | "New User Information" email with password setup link arrived. Gio was already in support-channel mode and did not act on it. |
| 23 Apr 00:49 | 22 Apr 16:49 | "Registration Completed" + Evan's reply ("I saw you submitted a registration which I've approved"). Gio read "approved" as application acceptance and stood down. |
| 23-25 Apr | 22-25 Apr | Expedite email bounced repeatedly on the typo'd domain. Gio did not realize until much later. |
| 24 Apr 05:00 | 23 Apr 21:00 | **SPI deadline passed.** |
| 24 Apr 08:55 | 24 Apr 00:55 | Gio first logged into Fluxx after password reset. Could not find any application. |
| 27 Apr 22:04 | 27 Apr 14:04 | Evan finally clarified plainly: registration is not the application; nothing was submitted. |

## Failure analysis

**Past Claude errors (own these explicitly in any future session):**

1. Failed to communicate in plain English at the moment Gio submitted that the 1-page form was registration only, and that a separate multi-page application form was still required before the 23 April deadline. When Gio expressed surprise that "it was just 1 page," past Claude said "that's it, wait" rather than "this was just registration, wait for approval, then there is a second multi-page form to fill before the deadline."
2. Drafted the expedite email using a typo'd domain (`grants@isoc.foundation` instead of `grants@isocfoundation.org`). The belt-and-suspenders escalation that was supposed to catch any timing problem therefore bounced and never reached anyone at ISOC Foundation.
3. Recorded the typo'd address in two project files (the 4/22 snapshot and the 4/22 research note), perpetuating the error in the project record.

**Fluxx UX issues that compounded:**

1. The registration form contains grant-content-coded fields ("SPI Project Summary" with 550-character limit, "Organization Mission") that read as substantive application content rather than registration prerequisites.
2. The "Thank you for submitting your registration information" auto-email does not flag a remaining application step or the deadline.
3. The "Registration Completed" auto-email confirms access but does not say "now complete your grant application before [deadline]."
4. There is no between-step nudge email between registration approval and the deadline.
5. Evan's helpdesk reply ("I saw you submitted a registration which I've approved which will create your user account") was easily read as application acceptance rather than registration approval.

## Strategy for late lodgement

**Decision-makers.** Late lodgement requires the **SPI program lead** or **ISOC Foundation grants manager**. Evan (Fluxx Helpdesk) cannot grant it himself but can escalate.

**Multi-channel push:**

1. **Reply to Evan** in the existing thread asking for explicit escalation to the SPI program lead.
2. **Direct cold letter** to `grants@isocfoundation.org` (correct domain) addressed to the SPI program lead.
3. **Warm-intro request to Naveed Haq** (`haq@isoc.org`, Senior Director Infrastructure and Connectivity at ISOC). Higher-leverage: senior, has prior context on the SPI proposal from a previous conversation with Gio.
4. **Warm-intro request to Warren Finch** (`finch@isoc.org`, IXP Development Expert at ISOC) for SPI program lead's name and a friendly heads-up. Broader-net safety.
5. **Optional follow-up if silence by EOD 4/29:** Identify program lead by name via web research; send personal follow-up. Optional third-party support letters from APNIC Foundation, PhNOG, FICTAP, DE-CIX if earlier channels stall.

**Send order:** Warren first (gives him ~1 hour to surface a name); then Evan reply; then cold letter to grants@isocfoundation.org. Send all three in the same window if Warren is slow.

**Goodwill case (priority order):**

1. Fluxx form UX is genuinely defective for first-time applicants (550-char "SPI Project Summary" on registration form, no Step 2 nudge, no deadline reminder in any auto-email).
2. Good-faith timing documented in Fluxx's own system (registered 30 hours before deadline, escalated to support 21 minutes after).
3. Bounced expedite email is on the record as a multi-channel good-faith attempt.
4. RISE's institutional SPI fit: GetaFIX (AS23942, ~1,952 networks across 3 sites, peak >1 Tbps), live FICTAP MOA, RIPE Atlas probe via Warren Finch, prior APNIC Foundation engagement (Project School Internet, Cebu).
5. Speed-to-lodge: hours, not weeks. Application content already drafted internally (`docs/ISOC Grant SPI.md`, `docs/revised-ISOC-SPI-v2.md`).

## Companion files

- `2026-04-28-isoc-spi-late-lodgement-drafts.md`: the three letters ready to send.
- `docs/research/2026-04-22-spi-fluxx-registration-and-attachment-requirements.md`: original (now-superseded) registration research, kept for reference. Contains the typo'd address in a quoted form for archival accuracy.
- `.claude/snapshots/2026-04-22-235843_isoc-spi-fluxx-registration-and-draft-softening.md`: original snapshot of the registration session. Also contains the typo'd address.
