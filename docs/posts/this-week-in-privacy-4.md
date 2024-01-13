---
date: 2024-01-13
categories:
    - This Week in Privacy
authors:
    - jonaharagon
---
# This Week in Privacy #4

Welcome back to *This Week in Privacy* (#4)! This is our weekly series where we cover the latest updates with what we're working on within the Privacy Guides community, and this week's top stories in the data privacy and cybersecurity space.<!-- more -->

Privacy Guides is a non-profit which researches and shares privacy-related information, and facilitates a community on our [forum](https://discuss.privacyguides.net) and Matrix where people can ask questions and get advice about staying private online and preserving their digital rights.

## Privacy Guides Updates

We're [looking for additional feedback](https://discuss.privacyguides.net/t/fediverse-why-how-recommendation-on-pg/16060) on how the *fediverse* plays into your privacy setup and recommendations. Is it an improvement over the existing alternatives, or is public social networking too much of a danger to privacy in any context? Let us know what you think about platforms like Mastodon, Pixelfed, and Lemmy on our forum.

## Privacy News

[Film studios are demanding Reddit unmask users who participated in piracy-related forums](https://arstechnica.com/tech-policy/2024/01/film-studios-demand-ip-addresses-of-people-who-discussed-piracy-on-reddit/):

> The studios are asking that the court require Reddit to provide “IP address log information from 1/1/2017 to present” for six anonymous Reddit users who talked about piracy on Reddit. [...] Reddit responded to the studios' subpoena with a letter on January 2 stating that the subpoena “does not satisfy the First Amendment standard for disclosure of identifying information regarding an anonymous speaker.” [...] Another reason Reddit refuses to comply with the film producers' request is that “none of the posts depicted in Exhibit A to the subpoena appear to relate to movies that we understand are the subject of" the copyright infringement claims.

In more lawsuit news, the U.S. Supreme Court denied Elon Musk's [request to consider whether X (formerly Twitter) can publicly disclose how often federal law enforcement seeks information about users](https://finance.yahoo.com/news/us-supreme-court-rejects-x-144342353.html):

> The justices declined to hear X's appeal of a lower court's ruling holding that the FBI's restrictions on what the company could say publicly about the investigations did not violate its free speech rights under the U.S. Constitution's First Amendment. [...] "History demonstrates that the surveillance of electronic communications is both a fertile ground for government abuse and a lightning-rod political topic of intense concern to the public," X's lawyers wrote in its petition to the Supreme Court.

[China claims it's cracked AirDrop encryption](https://www.bloomberg.com/news/articles/2024-01-09/china-says-cracked-apple-s-airdrop-to-identify-message-sources?sref=ExbtjcSG) and can identify message sources:

> A government-backed firm in China [claims that it’s cracked Apple’s encrypted Airdrop feature](https://sfj.beijing.gov.cn/sfj/sfdt/ywdt82/flfw93/436331732/index.html), allowing police to access the phone numbers and emails of those using it to share undesirable content.

According to the EFF, [Patreon is seeking to overturn a long-standing U.S. law which safeguards the privacy of your video viewing history](https://www.eff.org/deeplinks/2024/01/eff-asks-court-uphold-federal-law-protects-online-video-viewers-privacy-and-free):

> For decades, the Video Privacy Protection Act (VPPA) has safeguarded people’s viewing habits by generally requiring services that offer videos to the public to get their customers’ written consent before disclosing that information to the government or a private party. The VPPA, however, is under attack by Patreon. That service for content creators and viewers is facing a lawsuit in a federal court in Northern California, brought by users who allege that the company improperly shared information about the videos they watched on Patreon with Facebook.

[Google will *generously* (lol) let EU users decide how much data-sharing they are OK with](https://www.theverge.com/2024/1/12/24036312/google-digital-markets-act-services-user-data-opt-out), in response to the EU’s Digital Markets Act (DMA). This new policy only applies to data being shared between Google's own services, and has nothing to do with Google collecting data or sharing it with third parties:

> The new policy [...] allows users to opt out of data sharing across all, some, or none of a select number of Google’s services. The services listed include YouTube, Search, ad services, Google Play, Chrome, Google Shopping, and Google Maps. But the policy isn’t watertight — Google will still share user data when it’s necessary to complete a task (e.g., if you’re paying for a purchase on Google Shopping with Google Pay) in order to comply with the law, stop fraud, or protect against abuse.

## Security News

[Framework's accountant was hacked](https://www.bleepingcomputer.com/news/security/framework-discloses-data-breach-after-accountant-gets-phished/), exposing the personal information of (an undisclosed number of) laptop purchasers:

> Framework Computer disclosed a data breach exposing the personal information of an undisclosed number of customers after Keating Consulting Group, its accounting service provider, fell victim to a phishing attack. [...] As part of a subsequent investigation, the company identified all customers whose information was exposed in the attack and notified them of the incident via email.

A customized version of the Mirai botnet malware called [NoaBot has been installing cryptomining software on Linux devices](https://arstechnica.com/security/2024/01/a-previously-unknown-worm-has-been-stealthily-targeting-linux-devices-for-a-year/):

> For the past year, previously unknown self-replicating malware has been compromising Linux devices around the world and installing cryptomining malware that takes unusual steps to conceal its inner workings, researchers said. [...] Rather than performing DDoSes, the new botnet installs cryptocurrency mining software, which allows the attackers to generate digital coins using victims’ computing resources, electricity, and bandwidth.

[Tutanota upgraded their encryption from AES-128 to AES-256](https://discuss.privacyguides.net/t/tutanota-upgrades-encryption-from-aes-128-to-256/16143) in a step to bring "quantum-safe" encryption to their products in the future:

> We’ve now switched on AES 256 encryption by default for all new emails sent via Tuta. This is great security improvement and the next step towards quantum-safe encryption. [...] On our road to achieve quantum security 1 we are now updating our asymmetric cryptography (currently RSA 2048), in a next step we are focusing on rotating the existing encryption keys and key verification. [...] The same will be possible with the asymmetric RSA 2048 keys which will be replaced with both X25519 and Kyber-1024 turning the protocol into a hybrid (classical and quantum-safe) public key protocol.

* The Privacy Guides community notes that [AES-128 is already generally considered quantum-safe, but this update is a step in the right direction](https://discuss.privacyguides.net/t/tutanota-upgrades-encryption-from-aes-128-to-256/16143/3?u=jonah) when it comes to modernizing their security:

    > This change is not as exciting as their marketing team is making it out to be (on account of AES 128 already being quantum-safe), but replacing RSA 2048 will be a significant improvement to their encryption when they get to that.

In more quantum-related news, a new attack dubbed [KyberSlash is putting quantum encryption projects at risk](https://www.bleepingcomputer.com/news/security/kyberslash-attacks-put-quantum-encryption-projects-at-risk/), although not all projects using Kyber are vulnerable to key leaks:

> Multiple implementations of the Kyber key encapsulation mechanism for quantum-safe encryption, are vulnerable to a set of flaws collectively referred to as KyberSlash, which could allow the recovery of secret keys. [...] Mullvad says KyberSlash does not impact its VPN product because they're using unique key pairs for each new tunnel connection, making it impossible to perform a series of timing attacks against the same pair. BleepingComputer has contacted Signal to learn about the actual impact of KyberSlash on its cryptography and users' communications, as well as the project's remediation plans, but a comment wasn't immediately available.

## Community News

[The Proton Pass web app is now available for everyone](https://www.reddit.com/r/ProtonPass/comments/194a67f/the_proton_pass_web_app_is_now_available_for/):

> Use any browser to quickly manage your passwords, aliases, credit cards, TOTP codes, and notes at https://pass.proton.me.

The EFF released their new [Street Level Surveillance](https://sls.eff.org/) online portal:

> [...] a standalone website featuring expanded and updated content on various technologies that law enforcement agencies commonly use to invade Americans’ privacy. The hub has new or updated pages on automated license plate readers, biometric surveillance, body-worn cameras, camera networks, cell-site simulators, drones and robots, face recognition, electronic monitoring, gunshot detection, forensic extraction tools, police access to the Internet of Things, predictive policing, community surveillance apps, real-time location tracking, social media monitoring, and police databases.

Divested Computing Group, which develops privacy/security projects such as DivestOS and Mull Browser, [is continuing to fundraise this month](https://divested.dev/pages/donate#fundraiser2024) to fund future development, stating:

> DivestOS and the Divested projects as they currently stand are ultimately unsustainable. My goal for 2023 was to acquire a grant to continue my work, I was unsuccessful. Today I am announcing a fundraiser of raising $12,000 USD by end of February. It may be a stretch to ask, but I hope you all have found sufficient value in my work to keep these projects going. If it is unsuccessful I will switch to a full-time job and the Divested projects will take a backseat.

## TWIP Live 🔴

All the updates from *This Week in Privacy* will be shared here on the blog every week, so subscribe with your favorite RSS reader if you want to stay tuned. However, for people who prefer audio, we're going to be trying out a podcast-style recording of these updates every week, livestreamed on our YouTube channel.

- [Listen to *This Week in Privacy #4* on YouTube](https://www.youtube.com/watch?v=SRidkcaoJnI)

We're trialing *This Week in Privacy* for a month to see whether we and the community finds these sorts of updates to actually be valuable. *If* we do continue to publish these updates after that, we'll publish the audio version of the show as a standard RSS feed outside of YouTube separately.

## In the next TWIP

Will we continue to publish these updates? We'll see! We are hoping to publish a new TWIP update every Saturday, but we won't be able to do so without your help. If you find a news story you'd like us to share, or you're working on anything in the privacy space which our community would be interested in, please get in touch on our forum to share your update and be featured in next week's publication.
