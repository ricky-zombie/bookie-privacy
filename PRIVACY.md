# Bookie Privacy Policy

_Last updated: October 7, 2026_

**The short version.** Bookie keeps your books on your device. We have no servers, no accounts, no analytics, no advertising and no tracking, so there is nothing of yours for us to collect, sell or share. Bookie goes online in only three situations, each of which you start or switch on yourself and each of which is described below.

## Who this covers

"Bookie" is an iPhone and iPad app for bookkeeping and accounting. "We" means Bookie's developer. This policy describes what the app does with information. Because the developer receives none of it, most of the usual privacy questions (what we store about you, who we share it with, how to ask us to delete it) have the same answer: nothing leaves your device through us.

## What stays on your device

Everything you put into Bookie is stored only on the device you are using:

- **Your books:** the chart of accounts, journal entries, schedules, reconciliations, exchange rates, and the names and roles of the people you add as users.
- **A tamper-evident audit log** of what was done in the books, by whom, and when. It records actions and amounts, not the contents of your documents.
- **Documents you import** (photos, scans, PDFs, CSV and OFX files) are read on the device. Text is recognised with Apple's Vision framework and PDFKit, and nothing is uploaded.
- **Exports you create** (CSV, OFX, Excel) are written to a temporary protected folder, handed to the share sheet so that you choose where they go, and deleted afterwards. Once you send a file somewhere, that place's own policy applies.

### How it is protected

- The books file is encrypted with AES-GCM. Its key lives in the iOS Keychain, is usable only on this device and only after it has been unlocked once, and is not included in backups.
- The books file and audit log are marked for iOS file protection and are excluded from iCloud and computer backups.
- Bookie can require Face ID, Touch ID or your device passcode every time it opens. Bookie never sees your face, fingerprint or passcode; iOS tells Bookie only whether you passed.
- Each user's 6-digit PIN is stored only as a salted, slowed-down hash, never as the PIN. There is **no PIN recovery**: an Admin can reset another user's PIN, but nobody can recover the last Admin's PIN.
- The app hides its contents in the app switcher.

### Limits you should know about

Bookie keeps one set of books on one device. Roles and PINs separate duties between people who share that device; they do not protect the books from someone who has the device unlocked and the Admin's PIN. Because there is no server, there is also no cloud copy: **if you delete the app or lose the device without a copy of your exports, the books are gone.** Deleting the app removes the books and audit log. A small encryption key may remain in the Keychain; it is useless without the file.

## When Bookie goes online

Bookie makes a network request in only these three cases. If you never use these features, the app never connects.

1. **Downloading the on-device AI model (only if you ask).** Bookie can use a small language model that runs entirely on your device. When you confirm the download, the app fetches the model files (about 0.7 GB) from Hugging Face. The request names the model; it contains none of your data. Hugging Face can see your IP address and the time of the request and handles them under its own policy. After the download, questions to this model never touch the network.
2. **Asking Claude (only if you add your own key and confirm each time).** If the on-device model can't answer, Bookie can send that one question and the specific data it needs to Anthropic's Claude API. This happens only if you have entered your own Anthropic API key in Settings (an Admin permission) **and** you confirm, in a sheet that shows exactly what will be sent, every single time. Nothing is ever sent automatically. Your key is kept in the Keychain and goes only to Anthropic, directly from your device. Anthropic's terms and privacy policy govern what happens to that request; Bookie's developer never receives it.
3. **Updating exchange rates (only if an Admin turns it on).** In Settings an Admin can allow online rate updates, which is off by default. When you then tap Update, Bookie downloads the European Central Bank's public daily reference rates from a fixed address on ecb.europa.eu. The request contains no information from your books; the ECB can see your IP address and the time under its own policy. With the setting off, Bookie makes no request at all and rates are typed in by hand.

Bookie does not use cookies, advertising identifiers, analytics or crash-reporting services, and it contains no third-party tracking. The one other connection is one you make yourself: the link to this policy in Settings opens it in your browser, not inside Bookie.

## Permissions Bookie may ask for

- **Camera:** to scan receipts, statements and ledgers. Images are processed on the device.
- **Photos:** only the photos you choose, to read account balances from them.
- **Face ID:** to keep the books private.
- **Files:** only the files you pick to import.

You can change these at any time in iOS Settings.

## Information from Apple

If you use TestFlight or opt in to share analytics or crash data with developers in iOS Settings, Apple may provide the developer with aggregated, anonymous diagnostics. That comes from Apple, not from Bookie, and is governed by Apple's policies.

## Children

Bookie is a professional bookkeeping tool and is not directed at children under 13. The developer does not knowingly collect information from anyone.

## Your rights

The developer holds no personal information about you, so there is nothing to request, correct or delete. Everything Bookie stores is on your device, under your control: you can export it, change it within the app's rules, or delete the app to remove it. If you have used the optional services above, you can exercise your rights with Hugging Face, Anthropic or the ECB under their own policies.

## Changes to this policy

If Bookie's handling of information changes, this page will be updated and the date at the top changed before the new behaviour ships. Earlier versions are kept in the project's version history.

## Contact

Questions about this policy can be sent to rickyzombie@icloud.com.
