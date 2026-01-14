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

**1. App Settings » Custom Block List**

📸 (Screenshot: Custom Block List page)

তারপর Custom Block List পেজ থেকে 

1. **menu** তে যাও
---
---
2.তারপর**add new** button e click করো।

---
---
এখানে শুধু domain বা Full url path দাও:

**এক্সাম্পল:**
ads.network.com
অথবা 
https://ads.network.com/djjdbm

3. **Save করো।**

📸 (Screenshot: Domain added & saved)

এখন সেই server থেকে আর কিছু লোড হবে না —
না ads
না popup
না redirect
না adult content


---

## 🔍 যদি না জানো কোন Ads Company?

**Method 1** — Inspect Tool

Website খুলে যাও →

i. **Tools →**
---
---
ii. **Inspect →**
---
---

খুঁজো:

ads
banner
iframe
redirect
.js

**তুমি পাবে এরকম:**
https://ads.somecompany.com/script.js
অথবা অন্য ভাবেইও থাকতে পারে তুমি নিজে confirm হইয়েনেও কোনটা ads url

---

**Method 2** — ChatGPT (সবচেয়ে সহজ)

Page source পুরো কপি করো
ChatGPT-তে paste করো
লিখো:

> **“এই website কোন কোন URL থেকে ads বা popup লোড করছে?”**



ChatGPT বলবে কোন **domain Ads দিচ্ছে।**

তারপর chatgpt যখন তোমাকে url বা ads company domain return করবে তখন 
সেই domain Custom Block List-এ add করে দাও।


---

## 🎯 Banner Ads (চোখের সামনে থাকা Ads) hide করা

অনেক সময়
Redirect নেই
Popup নেই
কিন্তু বড় বড় **Banner Ads** থাকে।

এগুলো hide করা যায় Parent Container দিয়ে। html code modify করে।
 চলো দেখি Tools browser দিয়ে এই কাজটা কিভাবে করা যায়।

---

**Step 1:**

যে Website এর bannar ads hide করতে চাও সেই ওয়েবসাইট load করো।
আমি w3school load করলাম।

---
---

i) তারপর **Tools** → button এ ক্লিক করো

---
---
ii) Tools page থেকে **Edit Element** tool e ক্লিক করো।

---
---

Banner এর উপর tap করো। কিন্তু যদি Bannar ads যদি ifram বা shadow dom er ভেতর থাকে 
তাইলে ক্লিক কাজ করবে নাহ। এই অবস্থায় banner ads এর পাশে বা background element এ ক্লিক 
করার try করো।

---
---


**Step 2:**
যে html return পাবে সেই

HTML-এ banner ads Parent Container খুঁজো

Ads সাধারণত iframe বা dynamic script থেকে আসে —
ওগুলো modify করা যায় না।

কিন্তু Ads যেই জায়গায় বসে, সেই Parent div hide করা যায়।

সাধারণত এমন হয়:

> <div id="ads-container">  
> <div class="banner-ad">  
  এই ID বা Class কপি করো।

---
📸 (Screenshot: Parent container highlighted)
---

**Step 3:**

এবার আসল কাজ 
app Menu → Local JavaScript page open করো 

---
---
এবার এই page থেকে 
**✔ Entire Site**
এ টিক চিহ্ন দেও।

তারপর মেনু থেকে
**→ Create new**

---
---

নিচের JS বসাও
(এটা ID এবং Class — দুটোই support করে):

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
তুমি Inspector থেকে কপি করা নাম দিয়ে replace করবে।

Save করো।



---

**Step 4:**

Website Reload করো 🔄
Banner ads gone 😌

যদি কাজ না করে, তার মানে ভুল Parent নিয়েছো —
সঠিক Parent নিলে **100% কাজ করবে।**


---

## 🌍 Real Life Example

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

Tools Browser দিয়ে তুমি পাবে:

Safe browsing

Clean websites

No embarrassment

Full control

সব কিছু নিজের হাতে।

---

## Tools Browser – Latest Version Download

👉 **Tools Browser Download করুন এখান থেকে:**  
🔗 [Play Store থেকে Download করুন](https://play.google.com/store/apps/details?id=com.soumitra.toolsbrowser)

---

💡 Final Advice

ইন্টারনেটে ভালো content আর খারাপ ads আলাদা করা খুব দরকার।

Tools Browser তোমাকে সেই control দেয়।
