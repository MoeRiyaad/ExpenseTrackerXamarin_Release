# Budget Buddy

A privacy-focused expense and budget tracker for Android. Track income and expenses, set and monitor a monthly budget, get payment reminders as real phone notifications, see how you're doing at a glance, and manage everything by typing plain-English commands to a built-in assistant.

Your data stays on your device. An **optional, end-to-end encrypted cloud backup** is there if you want it.

## Download

Grab the latest APK from the **[Releases](../../releases)** page and install it on your Android device.

> This repository is a distribution point for release builds. The source code is maintained privately.

### Installing
1. Download the `.apk` file from the latest release
2. The first time, Android may ask you to allow installs from your browser or file manager (Settings → Apps → Special access → Install unknown apps)
3. Open the downloaded file and tap Install

Requires **Android 8.0** or newer.

## Features

- **Home**: balance overview, budget progress bar (green on track, red when over), payment reminders, recent transactions, and a **Money Wise dashboard**: a 0 to 100 score with a tip, your savings rate, how much you can safely spend per day, how your current budget is being used by category, and a 6-month income-vs-expense chart
- **Budget**: set a monthly budget, track it by calendar month or your own payday, and save/load complete budget setups
- **Balance Sheet**: a full transaction ledger with an income-vs-expense chart and running total
- **Payment reminders**: a real notification at 9 AM on the day each payment is due, every month, even after your phone restarts
- **Moe Assist**: type things like *"spent 250 on groceries"*, *"what's my balance"* or *"remind me every 20th to pay for the phone"*; it understands several instructions at once, percentages and quick maths, and works entirely on your device with no internet needed
- **Profile**: currency for virtually every country, light/dark theme, and a one-tap privacy mode that hides every amount on screen

## Security & privacy

**By default, nothing leaves your phone.** There is no account, no server, no analytics and no ads. Cloud backup is optional and only runs if you sign in and tap *Back up now*.

### If you use cloud backup

Your backup is **encrypted on your phone before it is uploaded.** The cloud only ever stores unreadable data: never an amount, a transaction name, a conversation or a setting. Someone who broke into the database, or Google itself, would see only scrambled bytes.

- **Strong encryption**: AES-256-GCM, with a key made from a passphrase only you know
- **Slowed-down guessing**: the passphrase is stretched with 600,000 rounds of PBKDF2-SHA256 and a fresh random salt for every backup
- **Tamper detection**: if a backup is altered in any way, restoring it fails rather than loading changed data
- **Your passphrase never leaves your phone**: it isn't uploaded or stored, and it's separate from your sign-in password
- **Private by rule**: each account can reach only its own backup
- **Encrypted in transit**: everything travels over HTTPS

### What this can't do

No software can honestly promise to be unhackable, and Budget Buddy hasn't been audited by an independent security firm. What it is built to guarantee is more specific: **if the cloud were breached, your financial data would still be unreadable without your passphrase.**

- **If you forget your backup passphrase, the backup can't be recovered**, by you or anyone. There is deliberately no reset.
- **Choose a strong passphrase.** Several unrelated words is better than a single word or a date; a weak one is easier to guess.
- **The cloud can still see** your account email, when you backed up, and roughly how big the backup is, but not what's in it.
- **On your phone**, your data is protected by Android's own security and your screen lock. A phone infected with malware, or rooted, could expose it.

## Feedback

Found a bug or have an idea? Open an [issue](../../issues) on this repository.

## Developed by

**Muhammed Riyaad**: [Portfolio](https://moeriyaad.github.io/MoeRiyaad_Portfolio/index.html)
