# An ad-blocking guide

&emsp;**This is the guide for blocking ads, and potentially trackers, malware, social media, adult and gambling websites.[^1]**  

&emsp;This guide is made to help partially remove ads from your everyday digital life. **Do note that no adblockers guarantee 100% digital ads being removed from what you see everyday.** Ads are shown in one way or another. It has immensely evolved from mere images, and there are millions of geniuses specialized in keeping it evolving.  

### 1. Browser extensions

&emsp;These are designed as extensions to work alongside your browser. These extensions can basically interact with, read, modify any web page you visit. Therefore, it is best that you use well-known and trust-worthy extensions. Some of them are listed below. Do note that each of these do have their own downsides.

- **uBlock Origin (Firefox/Brave)[^2]:** **open-source**, extremely **lightweight**, highly customizable, exceptionally efficient. It works fully on Firefox; it is gone from Chrome, and its brother is comparatively weaker.[^3]

- **uBO Lite (Google Chrome):** Essentially a **stripped down** version of uBlock Origin with Manifest V3 support in mind.[^3] It has weaker filtering, and it is realistically your only option if you want the uBlock Origin experience on Google Chrome. ***Recommended for Google Chrome users.***  

- **AdGuard (extension)**: polished, feature-rich, smooth, offers great ad and element blocking, script-blocking and dedicated protection against anti-adblock scripts. ***Recommended for the majority of users.***  

### 2. DNS

&emsp;These act as part of your connection. They are essentially your contact list for your Internet (with a few **asterisks**): on your contacts app, you look up "Mom," press call, and it calls your mom's phone number. on the Internet, you type in "google.com," press [Enter], and it redirects you to server's IP address. Ads are also stored in remote servers, and to display ads, your computer has to connect to the server, get the ad image and links, then show it on your computer. A DNS that blocks ads essentially delete all the entries for servers that store ads. It doesn't eradicate the server out of existence, just like how you delete your ex's number: you delete the name, but the number still exists, still "callable."  

&emsp;**DNS ad-blocking is far more limited than browser extensions or specialized programs.** For example, first-party ads like YouTube ads or in-app ads **cannot be blocked.[^4]** DNS **cannot hide page elements**, which may show where the ads supposedly are as blank boxes. DNS mostly use less resources than browser extensions, but whether it is considerable or not depend entirely on your machine. uBlock Origin comes closest to DNS in terms of resources, and it is far more capable than DNS by nature. These are some popular DNS options:  

- **AdGuard DNS**: your go-to pick with mainstream blocklists and modern encryptions.  

- **Control D (free)**: modern, low latency.  

&emsp;For most people, one of these is enough. For those who seek control over their Internet, you can look into DNS providers that offer features such as logging your connection, customizing blocklists, etc. Here are some of the most popular options:  

- **NextDNS (free/paid):** granular, customizable, mature. You can decide whether your log is kept, where to keep your log, how long your log is kept. **300k** queries a month on Free plan. Note that while they claim to not share your DNS logs, **they have not been audited.**  

- **Control D (paid)[^6]:** also granular and low-latency. They also have geo-unblocking, but **do NOT treat it as a VPN replacement.⁷** They use their own lists, and the lists aren't public either.  

- **AdGuard DNS:** polished, beginner-friendly, usually sold as part of the ecosystem. It purely focuses on filtering, and they are limited. Upselling their users is part of their marketing: **300k** queries on the Starter tier; **10M** queries and 20 devices on the more expensive tier  

&emsp;*For privacy enthusiasts: Control D is developed by the same team behind Windscribe VPN (which is based in Canada). Control D claims that they don't store your DNS queries or information, but **that's their own claim**. AdGuard (which is based in Cyprus) is at the time of writing **not fully audited by a third-party**, even though they also promise a strict no-logging policy. If you're serious about privacy, hosting a DNS yourself is a great alternative. Pi-hole and AdGuard Home are some of the most popular options. Most people do it with a Raspberry Pi, some even with an old phone. It shouldn't take much resources.*  

### 3. Specialized apps/software

&emsp;Dedicated ad-blocking software are generally more capable than DNS, while somewhat incomparable with browser extensions.[^7] Unlike extensions, **dedicated apps cover the whole system,** meaning ads from other apps, game launchers or desktop clients are **likely** to be blocked.[^5] Dedicated apps can strip elements/scripts even from browsers with no extensions (or incompatible extensions like Google Chrome.) You can control which apps will have ads blocked and which won't, and when you setup the software, there's no need to configure each browser separately anymore.

&emsp;**Dedicated software can sometimes use even more resources than browser extensions.** Most of the great options on the market are paid. On Android, there's only one VPN slot, meaning that you can only run one VPN at a time (which you should); dedicated apps can take your only VPN slot, meaning that you can't run your VPN at the same time as the ad-blocker.[^8] It's also the **trust factor**: to properly utilize the potential of software, dedicated desktop apps like AdGuard need to essentially read your traffic. That means that it can see what websites you go to, what messaging apps you use, and even your bank providers. These are some trustworthy software:

- AdGuard (cross-platform): **PAID,** mainstream, trustworthy, well-established and polished.

&emsp;For Android, specifically,

- RethinkDNS: combines DNS filtering with firewall rules for system-wide blocking, and trustworthy.

- AdGuard (as mentioned above.)

&emsp;For iPhone,

- AdGuard (as mentioned above.)

&emsp;These are some options that may help your digital life a bit easier. Do note that **no methods/software/extensions guarantee 100% of ads to be blocked.** 

&emsp;***Tips:*** On mobile devices (iPhones, iPads/Android devices,) some websites go as far as to "casually remind" users to disable ad-blockers with full-screen pop-ups that essentially renders the website unusable. For those who have this problem, do note that this is not hard to get around. There are many workarounds:

##### 1. On Android devices

&emsp;The solution depends mostly on your browser of choice. Google Chrome is usually the default choice on Android, but it doesn't support any kinds of extensions.  

- **Use Brave.** Your no-brainer choice with ad-blocking in mind. It doesn't require any kind of setup.  
- **Use Firefox with uBlock Origin.** Firefox is one of the most mainstream choices with add-ons support, including the full **uBlock Origin.** It is the closest you can get to the desktop experience, and it handles most anti-adblock pop-ups.  

##### 2. On Apple devices

&emsp;**All browsers are forced to use Apple's WebKit** on iOS/iPadOS, meaning Google Chrome, Firefox or even Brave are all fundamentally **Safari**.

- **Use a Safari Blocker that supports userscripts (wBlock or AdGuard.)** You might access such websites on your PC with uBlock normally, but you might have the same issue as mentioned on your iPhone. You might have used DNS, or even Safari's built-in tracking prevention, but the pop-up remains. This is because uBlock on browsers on your PC essentially injects **anti-adblock scriptlets**. Apple's WebKit and Safari Content Blocker API by nature only allow static declarative rules, which essentially means that basic blockers **cannot run scriptlets**. A blocker like wBlock or Wipr would **likely** fix this problem.  
- **Use Brave (or another web browser.)** Brave is among the most popular browsers that enforces their very own code and protection mechanisms above the WebKit base.

[^1]: To block trackers, malware, adult, and gambling, you may need to enable/apply specific blocklists (such as HaGeZi or OISD), modify specific settings, or use more specialized programs (such as BetBlocker or BlockP) and DNS resolvers.

[^2]: Brave is among the most well-known among Chrome-based browsers who still fully support uBlock Origin. Helium and Thorium are also solid alternatives.

[^3]: Google pushed Manifest V3 to Google Chrome, which makes uBlock Origin **dysfunctional**. Its brother **uBO Lite** works on Google Chrome, but with weaker filtering. The community viewed this as a step towards fighting ad-blockers. Some Chrome-based browsers offer support for uBlock Origin like Helium or Brave.

[^4]: **Whether DNS can block in-app ads like mobile game ads depend entirely on how the ads are fetched.** For example, the ad images are fetched from remote servers in **some** mobile game apps. If that's the case, DNS could block the domains, essentially blocking the ads. **Keep in mind that app developers have many ways to implement ads, in which DNS cannot block.**

[^5]: Technically, Control D offers a 14-day free trial with no credit card required. After the free trial, you can still use the DNS, but you will lose access to all the features, including logging, or customizable block lists, essentially rendering itself as equivalent of normal non-adblocking DNS like Google or Cloudflare.

[^6]: This is not a consumer VPN (which is more reliable on geo-blocking,) is paid tier only, and is not guaranteed to work with services that actively fight geo-unblocking. **Treat this claim with a grain of salt.** Your traffic to those domains passes through Control D’s infrastructure, and using their geo-unblocking feature may violate the terms of some services. If anything, this is more of a marketing claim than functional. It is a convenient add-on, rather than an actual replacement. If you need geo-unblocking, please consider a VPN instead.  

[^7]: Dedicated software does something better, while others are worse than extensions. It's like comparing apples and oranges: software wins on wider coverage, while extensions can do just as well or even better in filtering exclusively on browsers. **It depends on your priority.**

[^8]: Dedicated apps on Android generally do offer two modes: VPN mode and DNS mode. VPN mode is what takes up your only VPN slot, but it is more capable than DNS. DNS mode means just using the ad-blocking DNS, which is far less capable than what the VPN mode can actually offer.
