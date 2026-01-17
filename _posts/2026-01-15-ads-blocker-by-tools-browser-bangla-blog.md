---
layout: post
title: "Ads Blocker, Firewall-Style Protection: Tools Browser দিয়ে Redirect, Popup ও Banner Ads Control করার সম্পূর্ণ গাইড"
date: 2026-01-15 16:10:00 +0530
thumbnail: https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_thumb.png
---

আজকের ইন্টারনেটে আমরা সবাই একই সমস্যায় পড়ি —
Popup ads, auto-open tabs, adult banners, fake download buttons, casino links।

বিশেষ করে যখন আমরা
একটা ভালো website পড়ছি
আর হঠাৎ পাশে যদি family বা child থাকে —
Adult বা misleading ads দেখানো খুব embarrassing হয়ে যায় 😓

Tools Browser এই সমস্যার জন্যই বানানো হয়েছে।


---

## 🧠 Tools Browser কীভাবে কাজ করে?

Tools Browser কোনো website-এর ভেতরের ads কাটে না।
কোনো publisher-এর ক্ষতি করে না।

এটা করে **User-side URL Protection**।

মানে —

> কোন কোন server (URL) তোমার ফোনে লোড হবে
> 
> আর কোনগুলো হবে না
> 
> সেটা তুমি নিজে control করো।



এইটা ঠিক **firewall বা antivirus** এর মতো কাজ করে।


---

## 🔐 Smart Protection — Master Switch

প্রথমে Tools Browser ওপেন করেন:

1. App Settings এ যান→
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img1.jpg)
---

3. Site Settings এ যান→
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img2.jpg)

---
  
5. Smart Protection (টিক চিহ্ন দিন)
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img3.jpg)

---

এটা চেক ✅ on korle 

Redirect ads block

Popup ads block

Fake download block

Adult site redirect block

Tracking & malicious script block

সব একসাথে ব্লক হইয়ে যাবে।


---

**⚠️ খুব গুরুত্বপূর্ণ নিয়ম**

Smart Protection = Master Switch

Smart Protection **যদি OFF থাকে**
তাহলে:

Custom Block List

Ads Block

Redirect Block

**সব বন্ধ থাকে।**

সহজভাবে বললে:

> **Engine বন্ধ থাকলে Steering কাজ করে না 🚗**



তাই সবসময়:
Smart Protection → ON রাখতে হবে।


---

## 🧱 Custom Block List – নিজের মতো করে Ads Company block করা

ধরেন আপনি দেখলেন এই ধরনের URL লোড হচ্ছে:

ads.network.com
pop.redirect.xyz
adult-cdn.site

এখন আপনি ভাবলেন —
এই URL গুলো তো আসলে কোনো কাজের না।
বরং এগুলো থেকেই আসে popup, adult banner, fake download button, redirect 😓
যদি এগুলো একবারে
চিরতরে ব্লক করে রাখা যেতো
তাইলে তো ব্রাউজিংটা কত শান্ত, পরিষ্কার আর safe হতো, তাই না? 🔐
এই সমস্যার সমাধান করার জন্যই
Tools Browser দিয়েছে শক্তিশালী একটা ফিচার —
> Custom Block List
এটা ব্যবহার করতে যান:

**1. App Settings » Custom Block List**
> প্রথমে custom block list এ টিক চিহ্ন দিন
> তারপর custom block list লেখাতে ক্লিক করুন
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img4.jpg)
---

তারপর Custom Block List পেজ থেকে 

1. **Menu** তে যাও
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img5.jpg)

---
2.তারপর**Add new** button e click করুন।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img6.jpg)
---
এখানে শুধু domain বা Full url path দিন:

**এক্সাম্পল:**
ads.network.com
অথবা 
https://ads.network.com/djjdbm

3. **Add button এ ক্লিক করুন।**
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img7.jpg)
----

এখন site টা reload করে দেখুন।
এখন সেই url থেকে আর কিছু লোড হবে না —
>না ads
>না popup
>না redirect
>না adult content


---
**অনেক সময় এমন হয় —**
আমরা বুঝতেই পারি না
এই annoying ads গুলো
আসলে কোন **domain** বা কোন **company** থেকে আসছে 😕
কোনটা block করলে
**ads বন্ধ হবে —**
সেটাও আন্দাজ করা যায় না।
এই রকম situation-এর জন্যই
**Tools Browser এ আছে একটা smart system,**
যেটা আপনাকে দেখিয়ে দেবে —
ঠিক কোন Ads Company
আপনার ফোনে
content পাঠাচ্ছে।
## 🔍 যদি না জানেন কোন Ads Company?

**Method 1** — Inspect Tool

যে website টার ads block করতে চান সেটা load করুন তারপর→

i. **Tools →**
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img8.jpg)
---
ii. **Inspect →**
---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img9.jpg)
---

এবার এই inspect page থেকে খুঁজে বের করুন।

>ads
>banner
>iframe
>redirect
>.js

**আপনি পাবেন এরকম:**
https://ads.somecompany.com/script.js
অথবা অন্য ভাবেইও থাকতে পারে আপনি নিজে confirm করেনিন কোনটা ads url

---

**Method 2** — ChatGPT (সবচেয়ে সহজ)

Page source পুরো কপি করো
ChatGPT-তে paste করো
লিখো:

> **“এই website কোন কোন URL থেকে ads বা popup লোড করছে?”**



ChatGPT বলবে কোন **domain Ads দিচ্ছে।**

তারপর chatgpt যখন আপনাকে url বা ads company domain return করবে তখন 
সেই domain Custom Block List-এ add করে দিন। 


---

## 🎯 Banner Ads (চোখের সামনে থাকা Ads) hide করা

অনেক সময়
>Redirect নেই
>Popup নেই
>কিন্তু বড় বড় **Banner Ads** থাকে।

এই ধরনের ads
আলাদা tab খুলে না,
কিন্তু চোখের সামনে থেকেই
পেজের design নষ্ট করে দেয়
এবং পড়তে খুব বিরক্তিকর লাগে।
ভালো খবর হলো —
এই Banner Ads গুলোও
Tools Browser দিয়ে
hide করা যায়।
এটা করা হয়
ওই ads গুলোর Parent Container ধরে
**HTML code modify করে।**
চলেন দেখি
Tools Browser ব্যবহার করে
এই কাজটা
কিভাবে করা যায় 🚀

---

**Step 1:**

যে Website এর bannar ads hide করতে চান সেই ওয়েবসাইট load করুন।
আমি random একটা site load করলাম।
নিচের image টা দেখুন banner ads show হইয়েছে।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img10.jpg)
---

i) তারপর **Tools** → button এ ক্লিক করুন।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img11.jpg)
---
ii) Tools page থেকে **Edit Element** tool e ক্লিক করুন। অথবা direct inspect করে banner ads parent id খুঁজেতে পারেন। আমি ইজি method দেখাবো। **Edit Element** tool

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img12.jpg)
---

এখন যে Banner Ads hide করতে চান,
সেই Banner-এর উপর tap করুন।
তবে একটা বিষয় মনে রাখতে হবে —
যদি Banner Ads টি
iframe বা shadow DOM এর ভেতরে থাকে,
তাহলে সরাসরি Banner-এর উপর tap করলে
কাজ নাও করতে পারে।
এই অবস্থায় —
Banner-এর ঠিক পাশের কোনো element
বা তার background area-এ tap করার চেষ্টা করুন।
এতে করে Tools Browser ঠিক parent container ধরে নিতে পারবেন 🎯

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img13.jpg)
---


**Step 2:**
যে html return পাবেন সেই

HTML-এ banner ads Parent Container খুঁজুন 

Ads সাধারণত iframe বা dynamic script থেকে আসে —
ওগুলো modify করা যায় না। এর উপর ক্লিক কাজ করে না।

কিন্তু Ads যেই জায়গায় বসে, সেই Parent div বা iframe hide করা যায়।

সাধারণত এমন হয়:
```html
<div id="ads-container">  
<div class="banner-ad">
<iframe id="banner-ad">
```

বা অন্য কিছু নামে থাকতে পারে।
  এই ID বা Class কপি করো।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img14.jpg)

---

**Step 3:**

এবার আসল কাজ 
app Menu → Local JavaScript page open করুন।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img15.jpg)
---
এবার এই page থেকে 
**✔ Entire Site**
এ টিক চিহ্ন দিন।

তারপর মেনু থেকে
**→ Create new**

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img16.jpg)
---

নিচের JS বসান 
(এটা ID এবং Class —  যেটা আপনি পাবেন সেই অনুযায়ী js copy করে নিন। 
আমি id পেয়েছি তাই **document.getElementById** js টা কপি করলাম):

```javascript
// Hide by ID
var adById = document.getElementById("ads-container");
if (adById) {
adById.style.display = "none";
}
```

```jacascript

// Hide by Class
var adsByClass = document.getElementsByClassName("banner-ad");
for (var i = 0; i < adsByClass.length; i++) {
adsByClass[i].style.display = "none";
}
```

👉 এখানে "ads-container" অথবা "banner-ad"
আপনি Inspector থেকে কপি করা নাম দিয়ে replace করবেন।

Save করুন।

---
![Thumbnail](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/ads-blocker/blog6_img17.jpg)
----

---

**Step 4:**

Website Reload করেন 🔄
Banner ads gone 😌

যদি কাজ না করে, তার মানে ভুল Parent নিয়েছেন —
>সঠিক Parent নিলে **100% কাজ করবে।**


---

## ⚠️ Warning

যদি ভুল করে কোনো
ভুল ID বা ভুল Class ধরে hide করেন,
তাহলে শুধু Banner নয় —
ওই ID / Class ব্যবহার করা
অন্য element গুলিও hide হয়ে যেতে পারে।

কখনো কখনো এমনও হতে পারে —
পুরো page-টাই blank বা ভাঙা মনে হবে 😨

এই রকম কিছু হলে ভয় পাওয়ার দরকার নেই।

আপনি যে জায়গা থেকে
JS script add করেছিলেন
(যে site এখনো load আছে),
**সেখানেই গিয়ে
ওই script টা remove করে দিন।**

এতেই আপনার ওয়েবপেজ
আবার আগের মতো
normal হয়ে যাবে ✅

---

## 🌍 Real Life Example

ধরেন আপনি একটি:

Education site

Job portal

ব্যবহার করছেন,
কিন্তু হঠাৎ **adult** বা **casino banner** আসে।

Tools Browser দিয়ে:

Banner hide

Redirect block

Popup block

কিন্তু মূল website ঠিক মতো কাজ করে।


---

**⚖️ এটা কেন 100% Legal?**

Tools Browser:

কোনো website hack করে না

কোনো ads delete করে না

কোনো publisher ক্ষতি করে না

এটা শুধু বলে:

> “এই URL আমার ফোনে লোড হবে না”



ঠিক firewall এর মতো।


---

## 📥 Tools Browser ব্যবহার করো

Tools Browser দিয়ে আপনি পাবেন:

Safe browsing

Clean websites

No embarrassment

Full control

সব কিছু নিজের হাতে। এই crontrol একমাত্র tools browser এই আছে।

---

## Tools Browser – Latest Version Download

👉 **Tools Browser Download করুন এখান থেকে:**  
🔗 [Play Store থেকে Download করুন](https://play.google.com/store/apps/details?id=com.soumitra.toolsbrowser)

---

## 💡 Final Advice

ইন্টারনেটে ভালো content আর খারাপ ads আলাদা করা খুব দরকার।

Tools Browser তোমাকে সেই control দেয়।
