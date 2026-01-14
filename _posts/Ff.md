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

> `কোন কোন server (URL) তোমার ফোনে লোড হবে
> `আর কোনগুলো হবে না
> `সেটা তুমি নিজে control করো।



এইটা ঠিক **firewall বা antivirus** এর মতো কাজ করে।


---

## 🔐 Smart Protection — Master Switch

প্রথমে Tools Browser ওপেন করো:

1. App Settings →
---
---

3. Site Settings →
---
---
  
5. Smart Protection (টিক চিহ্ন দিন)
---
---

📸 (Screenshot: Settings page)

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

ধরো তুমি দেখলে এই ধরনের URL লোড হচ্ছে:

ads.network.com
pop.redirect.xyz
adult-cdn.site

Tools Browser এ যাও:

1. App Settings » Custom Block List

📸 (Screenshot: Custom Block List page)

এখানে শুধু domain দাও:

ads.network.com

Save করো।

📸 (Screenshot: Domain added & saved)

এখন সেই server থেকে আর কিছু লোড হবে না —
না ads
না popup
না redirect
না adult content


---

🔍 যদি না জানো কোন Ads Company?

Method 1 — Inspect Tool

Website খুলে যাও →
Tools → Inspect / Page Source

📸 (Screenshot: Inspect menu)
📸 (Screenshot: Page source view)

খুঁজো:

ads
banner
iframe
redirect
.js

তুমি পাবে এরকম:

https://ads.somecompany.com/script.js

এইটাই ads server।


---

Method 2 — ChatGPT (সবচেয়ে সহজ)

Page source পুরো কপি করো
ChatGPT-তে paste করো
লিখো:

> “এই website কোন কোন URL থেকে ads বা popup লোড করছে?”



ChatGPT বলবে কোন domain Ads দিচ্ছে।

সেই domain Custom Block List-এ দাও।


---

🎯 Banner Ads (চোখের সামনে থাকা Ads) hide করা

অনেক সময়
Redirect নেই
Popup নেই
কিন্তু বড় বড় Banner Ads থাকে।

এগুলো hide করা যায় Parent Container দিয়ে।


---

Step 1

Website খুলে
Tools → Element Inspector

📸 (Screenshot: Element inspector tool)

Banner এর উপর tap করো।


---

Step 2

HTML-এ তার Parent Container খুঁজো

Ads সাধারণত iframe বা dynamic script থেকে আসে —
ওগুলো modify করা যায় না।

কিন্তু Ads যেই জায়গায় বসে, সেই Parent div hide করা যায়।

সাধারণত এমন হয়:

<div id="ads-container">  
<div class="banner-ad">  এই ID বা Class কপি করো।

📸 (Screenshot: Parent container highlighted)


---

Step 3

Menu → Local JavaScript
✔ Entire Site
→ New Script

📸 (Screenshot: Local JavaScript menu)

নিচের JS বসাও
(এটা ID এবং Class — দুটোই support করে):

// Hide by ID
var adById = document.getElementById("ads-container");
if (adById) {
adById.style.display = "none";
}

// Hide by Class
var adsByClass = document.getElementsByClassName("banner-ad");
for (var i = 0; i < adsByClass.length; i++) {
adsByClass[i].style.display = "none";
}

👉 এখানে "ads-container" অথবা "banner-ad"
তুমি Inspector থেকে কপি করা নাম দিয়ে replace করবে।

Save করো।


---

Step 4

Website Reload করো 🔄
Banner ads gone 😌

যদি কাজ না করে, তার মানে ভুল Parent নিয়েছো —
সঠিক Parent নিলে 100% কাজ করবে।


---

🌍 Real Life Example

ধরো তুমি একটি:

Education site

Job portal

Government form

ব্যবহার করছো,
কিন্তু হঠাৎ adult বা casino banner আসে।

Tools Browser দিয়ে:

Banner hide

Redirect block

Popup block

কিন্তু মূল website ঠিক মতো কাজ করে।


---

⚖️ এটা কেন 100% Legal?

Tools Browser:

কোনো website hack করে না

কোনো ads delete করে না

কোনো publisher ক্ষতি করে না

এটা শুধু বলে:

> “এই URL আমার ফোনে লোড হবে না”



ঠিক firewall এর মতো।


---

📥 Tools Browser ব্যবহার করো

Tools Browser দিয়ে তুমি পাবে:

Safe browsing

Clean websites

No embarrassment

Full control

সব কিছু নিজের হাতে।


---

💡 Final Advice

ইন্টারনেটে ভালো content আর খারাপ ads আলাদা করা খুব দরকার।

Tools Browser তোমাকে সেই control দেয়।

Be safe. Browse smart. Stay in control. 🛡️ Ei same post ata kichu nah palte convert to GitHub skyll post er jonne r amk .md file edeo code gulo code marker diye dibe. Bold text ** then head ## r ja ja marker j ekhan ja dokrar
