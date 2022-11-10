---
date: 2022-11-10
categories:
    - Software
authors:
    - matchboxbananasynergy
tags:
    - PSA
    - Signal
    - Instant Messengers
links:
    - Signal Configuration Guide: https://www.privacyguides.org/real-time-communication/signal-configuration-hardening/
    - Real-Time Communication: https://www.privacyguides.org/real-time-communication/
license: BY-SA
---
# Important Changes to Signal Registration and Registration Lock

Signal has changed how it handles registration. This primarily affects people who are using a number that they don't have exclusive access to for Signal.

## How It Used to Work

As outlined in our previous [Signal Configuration & Hardening Guide](https://blog.privacyguides.org/2022/07/07/signal-configuration-and-hardening/#signal-pin), if you registered a number with Signal, set up Registration Lock and checked into the app at least once every 7 days, nobody could use the number you'd claimed and try to re-register it for themselves without knowing your Registration Lock PIN.

## How It Works Now

As outlined in this [issue](https://github.com/signalapp/Signal-Android/issues/12595#issuecomment-1310752097) on the Signal-Android GitHub repository, if someone tries to register with that number and is able to get the SMS code, they can kick you out of your Signal account. At that point, you have to re-register by receiving an SMS for that number, and inputting your Signal PIN. If you are unable to do this, the Registration Lock is not enforced after 7 days. Someone who tries to register after that will be prompted to enter the Signal PIN once more. If the correct PIN is not entered, the app will prompt you to create a new PIN, and the account is wiped and the number can be claimed by a person who can receive an SMS code for it.

>If Alice registers number X and enables reglock, but Bob later proves ownership of number X (by registering and completing the SMS code), then Alice will >be unregistered. However, if a reglock is present, Bob still won't be able to register immediately if he does not know the reglock code. This allows >reglock to still function as a way to prevent someone else from taking over your account.
>
>However, by unregistering Alice, this starts a 7-day timer. After 7 days, if Alice doesn't re-register, then the reglock is removed and Bob will be free to register the number without needing to know the reglock. But if Alice still truly does own the number, she can simply re-prove ownership and things should go back to normal for her.
>
>This is important because phone number can (and are) re-used among cell carriers. If someone gets a new phone number from their carrier, they should not be prevented from registering with Signal indefinitely because the previous owner has reglock.
>
>The intention of reglock is to prevent hijacking of numbers you actually own, not to guarantee the number for yourself for life.

While this change makes sense from the perspective of making it so you cannot "hold a number hostage" as long as you keep checking in, it is particularly important for people who've used disposable phone numbers to know this.

We recommend migrating to a phone number that you own and will be able to own for the foreseeable future in order to avoid getting locked out of your account and losing your contacts.

---

*Special thanks to the [Molly](https://molly.im) community who made us aware of this change soon after it went live.*
