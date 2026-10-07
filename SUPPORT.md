# Bookie Support

_Last updated: October 7, 2026_

Bookie keeps double-entry books on your iPhone or iPad. Answers to the most common questions are below. If yours isn't here, write to **rickyzombie@icloud.com**. We reply as soon as we can.

## Getting help

When you write, it helps to include your device and iOS version, Bookie's version (shown in the App Store), and the steps that led to the problem. **Please don't send PINs, account numbers or screenshots of real books.** If you need to show a problem, use Settings > Sample books to reproduce it with sample data.

## Getting started

### How do I set up my books?
On first launch Bookie asks you to create the Admin: a name and a 6-digit PIN that isn't a repeat or a run like 123456. The Admin then adds everyone else under Settings > Users & roles and chooses what each person can do. Add an Accountant to enter entries and a Reviewer to approve them, then use the Ledger tab and the + button to make your first entry.

### Why can't I approve my own entry?
That is deliberate. An entry moves from draft to submitted to posted, and the person who created it can never be the one who approves it. This is the basic control that stops one person entering and posting the same transaction. Sign in as someone else with the Reviewer or Admin role to approve it.

### I'd like to look around with some data in it.
As Admin, open Settings > Sample books > Load sample books. It adds a fictional coffee roaster's books for the last three months. You can remove them again from the same place until you add entries of your own.

## PINs and the lock

### I forgot my PIN.
Ask an Admin to reset it: Settings > Users & roles, choose the person, then Reset PIN. If you are the only Admin and you have forgotten your PIN, **it cannot be recovered**; there is no back door, by design. Add a second Admin as soon as you can so that this never happens, and keep regular exports (see below).

### Why does Bookie ask for Face ID or my passcode?
Bookie locks itself when you leave the app, and unlocks with Face ID, Touch ID or your device passcode. An Admin can change how soon it locks, or turn the requirement off, under Settings > Security. Your PIN identifies you inside Bookie on top of this.

### It says too many wrong PINs.
After five wrong PINs a profile is locked for a minute. Wait, or ask an Admin to reset your PIN, which also clears the lock.

## Your data

### Does Bookie sync between devices or back up to iCloud?
No. Bookie has no servers and keeps one set of books on one device, encrypted, and left out of backups. That is what keeps your data private, and it means **there is no cloud copy**. If you delete the app or lose the device, the books go with it.

### How do I keep a copy?
Use Ledger > Export to CSV or OFX regularly, for example after each month-end, and save the files somewhere you trust through the share sheet. The journal CSV can be imported back (as drafts for approval), and the OFX statement can be read by other accounting software.

### How do I get my data out?
Ledger > Export to CSV or OFX offers the journal, the chart of accounts, the trial balance and a bank-style statement of one account. The Books tab can also export statements to Excel.

## Everyday accounting

### I posted something wrong. How do I fix it?
Posted entries are permanent. Open the entry and choose Reverse this entry, give a reason, and post the corrected entry. If the entry is in a closed period, an Admin must reopen the period first (with a reason, which is recorded in the audit log).

### How do I close a month?
Ledger > Period-end closing prepares the closing entries, which someone else approves. Closing waits while scheduled adjusting entries are unprepared or still drafts, so deal with Ledger > Adjusting entries first. Then use Close period to lock the month.

### How do I record prepaid insurance, unearned revenue or depreciation?
Enter the payment or receipt as a normal entry, then create a schedule under Ledger > Adjusting entries. Each month Bookie drafts the entry that moves the amount across, for approval. Accruals, which can reverse themselves on the first of the next month, are there too.

### How do I import a bank statement?
Ledger > Import statements and entries accepts OFX, QFX and CSV files from your bank, and journal CSV files. Choose which account the statement belongs to and which account the other side of each line should go to. Everything arrives as drafts, and lines you've already imported are skipped.

### How do I reconcile?
Ledger > Bank reconciliation. Pick the account, the statement date and the statement's ending balance, then tick the lines that appear on the statement until the difference is zero. Loading the statement file ticks matches for you, and lines the books don't have, such as bank fees, can be booked right there as drafts.

### How do foreign currencies work?
Accounts can be held in a foreign currency while the books stay in US dollars. Add rates under Ledger > Currencies and exchange rates; each entry keeps the rate it was made with. At month-end, revalue the foreign accounts from the same screen.

## Online features

### Does Bookie connect to the internet?
Only in three cases, each started or switched on by you: downloading the optional on-device AI model, asking Claude a question with your own API key (you confirm exactly what is sent, every time), and fetching the European Central Bank's public exchange rates if an Admin turns that on in Settings. See the [privacy policy](https://ricky-zombie.github.io/bookie-privacy/) for the details.

## About Bookie

### Is Bookie tax or legal advice?
No. Bookie is a bookkeeping tool. Check anything important, especially answers from the optional AI features, against your own records and a qualified professional.

### Where is the privacy policy?
At [ricky-zombie.github.io/bookie-privacy](https://ricky-zombie.github.io/bookie-privacy/), and in the app under Settings > Privacy.

## Contact

rickyzombie@icloud.com
