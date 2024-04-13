---
date: 2024-01-20
categories:
    - This Week in Privacy
authors:
    - jonaharagon
---

# This Week in Privacy #5

Welcome back to *This Week in Privacy*, our weekly series where we cover the latest updates with what we're working on within the Privacy Guides community, and this week's top stories in the data privacy and cybersecurity space.

Privacy Guides is a non-profit which researches and shares privacy-related information, and facilitates a community on our [forum](https://discuss.privacyguides.net/?ref=blog.privacyguides.org) and Matrix where people can ask questions and get advice about staying private online and preserving their digital rights.

## Privacy Guides Updates

A small update for our translation team this week, we've resolved our issues with Crowdin, which allowed us to publish the updated version of the website we've been waiting for for several weeks. You can check out the changelog for v3.19 of the website [here](https://github.com/privacyguides/privacyguides.org/releases/tag/v3.19).

For our contributors, the fix involves a change to how we write admonitions in the source code of the website. If you're writing a new page or contributing to an existing one, you can read more about the proper format for admonitions in our [writers guide](https://www.privacyguides.org/en/meta/admonitions/).

## New Recommendations

v3.19 of the website finally published our information on **uBlock Origin Lite** (mentioned in [TWIP #1](https://blog.privacyguides.org/2023/12/09/this-week-in-privacy-1)) and **Brave's forgetful browsing** feature (mentioned in [TWIP #2](https://blog.privacyguides.org/2023/12/16/this-week-in-privacy-2)), so if you were waiting for information about those recommendations to be published, you can read them on privacyguides.org now.

We also updated our Skiff Mail recommendation to reflect their new support for PGP, which is a great step forward in the world of interoperable email encryption. Again, you can read the full [changelog for v3.19](https://github.com/privacyguides/privacyguides.org/releases/tag/v3.19) of privacyguides.org if you want to know about all the changes.

## Privacy News

Moving on to news from around the privacy and cybersecurity space...

In a follow up to the story we shared last week about China cracking AirDrop encryption in order to track individual AirDrop users, *CNN* reports that [Apple has been aware of tracking concerns with AirDrop since at least 2019](https://edition.cnn.com/2024/01/12/tech/china-apple-airdrop-user-encryption-vulnerability-hnk-intl/index.html):

> Security researchers warned Apple as early as 2019 about vulnerabilities in its AirDrop wireless sharing function that Chinese authorities claim they [recently used](https://www.cnn.com/2024/01/10/tech/china-apple-airdrop-encryption-hnk-intl/index.html) to track down users of the feature, the researchers told CNN, in a case that experts say has sweeping implications for global privacy.
> A group of Germany-based researchers at the Technical University of Darmstadt, who first discovered the flaws in 2019, told CNN Thursday they had confirmation Apple received their original report at the time but that the company appears not to have acted on the findings. The same group published a [proposed fix](https://www.usenix.org/system/files/sec21-heinrich.pdf) for the issue in 2021, but Apple appears not to have implemented it, the researchers said.

The Swiss magazine *Republik* has [accused the Swiss government of massive online surveillance of their citizens](https://www.swissinfo.ch/eng/business/swiss-government-accused-of-massive-online-surveillance/49117880):

> The Swiss Federal Intelligence Service (SRC) is allegedly monitoring the digital activities of the Swiss population, particularly on their mobile phones and computers, according to the German-language magazine Republik.ch on Tuesday. What's more, Swiss spies are said to be storing far more information than they promised when the new intelligence law was introduced. The SRC denies these accusations. The Swiss Government is allegedly able to access the messages and emails of the population thanks to the Swiss Federal Intelligence Service (SRC), at least according to the German-language media [Republik.ch](https://www.republik.ch/2024/01/09/der-bund-ueberwacht-uns-alle).

A study conducted by *Consumer Reports* and *The Markup* indicates that [Facebook receives information from "thousands of companies" about each of its average users](https://www.consumerreports.org/electronics/privacy/each-facebook-user-is-monitored-by-thousands-of-companies-a5824207467):

> Using a panel of 709 volunteers who shared archives of their Facebook data, Consumer Reports found that a total of 186,892 companies sent data about them to the social network. On average, each participant in the study had their data sent to Facebook by 2,230 companies. That number varied significantly, with some panelists’ data listing over 7,000 companies providing their data.

Brave Browser is "simplifying" their privacy protections, [removing their "Strict" fingerprinting protection mode from their browser](https://brave.com/privacy-updates/28-sunsetting-strict-fingerprinting-mode):

> With desktop and Android version 1.64 in a couple of months (and in today’s Nightly release for testing), Brave will sunset Strict fingerprinting protection mode. This does not affect Brave’s industry-leading fingerprinting protection capabilities for users. Instead, it will allow us to focus on improving privacy protections in Standard mode and avoid Web compatibility issues.

Privacy Guides currently recommends using Strict fingerprinting protections in Brave, as do many other privacy-centric configuration guides for Brave Browser. We are looking into into what this change will mean for our guide and recommendations, and we'll release an additional update about this soon.

In what is hopefully not new news to anyone here, [Google is admitting they track more about your browsing than some people might think in Incognito Mode](https://www.ghacks.net/2024/01/16/google-updates-chromes-incognito-mode-disclaimer-to-admit-it-is-tracking-users):

> Google is rolling out a change to the Incognito Mode disclaimer of the company's Chrome web browser. It admits in it that it is tracking users even while the mode is active. The company [settled a $5 billion privacy lawsuit](https://www.ghacks.net/2023/12/29/google-settles-its-5-billion-privacy-lawsuit-over-incognito-mode-tracking) over tracking in Incognito Mode in December 2023.

## Security News

In a first for Qualcomm devices, the [Samsung Galaxy S24 is receiving 7 years of updates](https://arstechnica.com/gadgets/2024/01/the-galaxy-s24-gets-seven-years-of-updates-1300-titanium-ultra-model):

> Samsung is matching Google's new update plan and offering "seven years of security updates and seven generations of OS upgrades." Previously, it gave [four years](https://news.samsung.com/global/samsung-sets-the-new-standard-with-four-generations-of-os-upgrades-to-ensure-the-most-up-to-date-and-more-secure-galaxy-experience) of updates.

We generally don't [recommend](https://www.privacyguides.org/en/android) Samsung devices, but this change could have a major impact in the Android hardware space overall. Fairphone notably had to resort to an "industrial" chip in their latest phone just to receive 5 years of updates from Qualcomm, but this could push Qualcomm to update all of their newer devices for much longer than before. Time will tell whether this level of support will be available to companies other than Samsung in the future.

Kaspersky released a [new tool which analyzes the Shutdown.log file on iOS devices to scan for Pegasus malware](https://securelist.com/shutdown-log-lightweight-ios-malware-detection-method/111734):

> [...] we’ve analyzed and confirmed the reliability of detecting a Pegasus malware infection using the Shutdown.log artifact stored in a sysdiag archive. The lightweight nature of this method makes it readily available and accessible. Moreover, this log file can store entries for several years, making it a valuable forensic artifact for analyzing and identifying anomalous log entries. Again, this is not a silver bullet that can detect all malware, and this method relies on the user rebooting the phone as often as possible.

Kaspersky notes that typical methods of [detecting mobile spyware](https://www.privacyguides.org/en/device-integrity) rely on either scanning a full encrypted backup of the device, or performing network traffic analysis on the device in question, both of which can be time-consuming and difficult. This new tool scans system log files which are readily available in iOS and are much more lightweight than full backups.

## Community News

One of our readers noted that a creator on YouTube expressed confusion about how we make recommendations about tools like [VPNs](https://www.privacyguides.org/en/vpn). I'll briefly cover the transparent process here in response:

1. **New tools and providers are recommended by our [community](https://discuss.privacyguides.net/c/site-development/suggestions/6).** Often people will ask why we haven't reviewed a certain tool, and the answer is usually that our community simply didn't care enough about that tool to suggest it in the first place. We have a section on our forum where people can suggest and vote for tools they think should be covered, and then we review them.
2. **Suggestions are evaluated by our team.** One or two of our [team members](https://www.privacyguides.org/en/about) will test out these tools and take notes about how they do or do not fit our criteria, and these notes are shared on our forum. The team member will mark a suggestion as either [approved](https://discuss.privacyguides.net/tag/approved) (awaiting a pull request) or [rejected](https://discuss.privacyguides.net/tag/rejected). This step is not the final approval for a tool.
3. **A pull request (first draft) is submitted.** Somebody—typically but not always the team member from the previous step—will write a draft recommendation, section, or page on the website and submit it on [GitHub](https://github.com/privacyguides/privacyguides.org/pulls).
4. **Pull Requests are evaluated by our team.** At this point, two team members other than the one who wrote the pull request will perform a final evaluation of the recommendation. They verify every statement being published, make sure the tool meets our criteria and nothing slipped through in the preliminary review on our forum, and perform a final pass through of the draft. Approvals or requests for changes are indicated on GitHub.
5. **Approved PRs are merged into the main site.** After a minimum of two individual approvals from contributors other than the author of the PR, a recommendation can be published on the website. This process ensures the information available is reliable as possible, and was published in accordance to all our policies. Every team member has the individual ability to block a PR at any time with a "Request for Changes" note until their concerns are addressed.

Privacy Guides has strict conflict of interest policies when it comes to submissions, and of course we don't make recommendations based on affiliate programs (which we don't participate in), sponsors, or other financial incentives. Privacy Guides is a non-profit organization in the United States with a legal obligation to fulfill the following [mission statement](https://opencollective.com/privacyguides):

> The **Privacy Guides** team is providing services, tools, and knowledge to protect your privacy against global mass surveillance. Our website is free of advertisements and not affiliated with any listed providers.
>
> The purpose of Privacy Guides is to educate our community on the importance of privacy online and government programs internationally that are designed to monitor all of your online activities. We do not operate Privacy Guides for personal profit, and all funds will be used to further our mission in one form or another.

Activities outside the scope of that statement are prohibited.

Privacy is not a zero-sum game, but unfortunately some content creators see our independent process as a threat to their [business model](https://blog.privacyguides.org/2019/11/20/the-trouble-with-vpn-and-privacy-review-sites), and would rather publish their "speculations" and create drama instead of checking their facts, so this is a one-stop place to check their facts for them instead of debating each one individually, which we don't have time to do. Although, if anyone does have a specific question about something which is not covered here, a question on our forum will always receive a response!

## TWIP Live 🔴

All the updates from *This Week in Privacy* will be shared here on the blog every week, so subscribe with your favorite RSS reader if you want to stay tuned. However, for people who prefer audio, we're going to be trying out a podcast-style recording of these updates every week, livestreamed on our YouTube channel.

- [Listen to *This Week in Privacy #5* on YouTube](https://www.youtube.com/watch?v=2i9a_-d1Aao)

We're trialing *This Week in Privacy* for a month to see whether we and the community finds these sorts of updates to actually be valuable. *If* we do continue to publish these updates after that, we'll publish the audio version of the show as a standard RSS feed outside of YouTube separately.

**Update Jan 21, 2024:** [*This Week in Privacy* is now available via RSS](https://fm.neat.tube/@thisweekinprivacy) for use with any podcast client!

## In the next TWIP

Will we continue to publish these updates? We'll see! We are hoping to publish a new TWIP update every Saturday, but we won't be able to do so without your help. If you find a news story you'd like us to share, or you're working on anything in the privacy space which our community would be interested in, please get in touch on our forum to share your update and be featured in next week's publication.
