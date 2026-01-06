JavaScript শেখার সময় সবচেয়ে বড় যে ভুলটা প্রায় সবাই করে, সেটা হলো—
**Practice না করা**।

অনেকেই **কোর্স করে, ভিডিও দেখে, নোট মুখস্থ করে** মনে করে JavaScript শিখে ফেলেছে।
কিন্তু বাস্তব সত্যি হলো—
**Practice ছাড়া JavaScript শেখা সম্ভব না**।

মুখস্থ বিদ্যা বেশি দিন থাকে না।
আমাদের মাথায় সব সময় নতুন নতুন আইডিয়া ঘোরে—
কিন্তু সেই আইডিয়া যদি সাথে সাথে পরীক্ষা না করা যায়, তাহলে ধীরে ধীরে সব হারিয়ে যায়।

---

## কেন Practice না করলে JavaScript শেখা যায় না

ধরো তুমি JavaScript শিখছো।
অনেক টাকা খরচ করে কোর্স করছো।
কিন্তু প্রতিদিন যদি নিজে হাতে script লিখে, run করে, ভুল দেখে ঠিক না করো—
তাহলে শেখাটা শুধু কাগজেই থেকে যাবে।

**JavaScript এমন একটা language—**
যেটা না লিখলে, না ভাঙলে, না test করলে বোঝা যায় না  
👉 কোন script কেন কাজ করছে  
👉 কোথায় error হচ্ছে  
👉 real website এ গেলে কী সমস্যা হবে

---

## Laptop না থাকলে Practice বন্ধ? একদমই না

এখন একটা real life situation ভাবো—

তুমি কোথাও বন্ধুদের সাথে আড্ডা দিচ্ছো।
হঠাৎ মাথায় একটা **JavaScript আইডিয়া এলো।**
অথবা **ChatGPT** থেকে একটা script generate করলে।

এখন প্রশ্ন—
**Script টা test করবে কীভাবে?**

**Laptop নেই।**
**PC নেই।**
বাড়ি গিয়ে test করতে গেলে ততক্ষণে মাথা ঠান্ডা।

**আগে হলে এখানেই সব শেষ।
এখন আর না।**

---

## Tools Browser দিয়ে Mobile দিয়েই Real Practice

Tools Browser ব্যবহার করলে তুমি—

- **নিজের JavaScript script বানাতে পারো**
- **যেকোনো website এ inject করে test করতে পারো**
- **Script কাজ করছে নাকি না, সাথে সাথে বুঝতে পারো**
- **Script save করে রাখতে পারো, হারাবে না**
- **পরে বাড়ি গিয়ে laptop এ final code বসাতে পারো**

সবচেয়ে গুরুত্বপূর্ণ বিষয়—
**এতে website বা server side এ কোনো ক্ষতি হয় না**।
সবকিছু শুধু তোমার মোবাইলেই locally run করে।

---

## Server এ code বসানোর আগে Mobile দিয়ে Test কেন জরুরি

ধরো তুমি নিজের বা client এর website এ JavaScript add করতে চাও।

JavaScript তো programming language—
ভুল হতেই পারে।

এখন যদি তুমি সরাসরি server এ code বসাও আর বারবার error হয়—

- অন্য code নষ্ট হতে পারে
- server reload করতে হয়
- chair–table এ বসে সময় নষ্ট
- মাথা গরম

**Solution?**  
আগে mobile দিয়ে inject করে test করো।
সব ঠিক থাকলে তারপর server এ final code বসাও।

Easy. খুব easy.

---

## Tools Browser এ JavaScript Inject করার Step-by-Step

**Step 1:** Tools Browser open করো  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076217.png)

**Step 2:** যে website এ test করতে চাও সেটা open করো, আমি **w3schools.com ওপেন করলাম।**  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076917.png)

**Step 3:** Tools button এ click করো  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076918.png)

**Step 4:** Custom tab এ যাও  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076919.png)

এই জায়গাটাই হলো তোমার **JavaScript Practice Ground**  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076921.png)

---

## Javascript কীভাবে Create করবে

- **Custom page** এর মেনু থেকে **Create tools** এ ক্লিক করো  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076922.png)

- Script এর একটা **Title** দাও  
- **Description লেখো**  
- **Raw JavaScript** paste করো  
তারপর **CREATE** বাটনে ক্লিক করো  
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076927.png)

**গুরুত্বপূর্ণ কথা:**  
Tools Browser নিজে থেকেই **Script tag handle করে**।  
তাই **script tag লিখবে না**।  
শুধু raw JavaScript paste করো।

![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076954.png)

```javascript
(function () {
    var divs = document.getElementsByTagName("div");
    for (var i = 0; i < divs.length; i++) {
        divs[i].style.backgroundColor = "#000000"; 
    }
})();
```

![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076928.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076929.png)

---

## Script কাজ করছে নাকি না – বুঝবে কীভাবে

- **console.log**
- **success message**
- **error message**

![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076938.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076939.png)

---

## Predefined JavaScript দিয়ে Practice আরও সহজ

![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076940.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076941.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076944.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076945.png)
![img](https://raw.githubusercontent.com/soumitra88875/tools-browser-blog-image/main/3076946.png)

**এটাই real learning।**

---

## শেষ কথা

JavaScript শেখার সবচেয়ে বড় শত্রু হলো—
**Practice না করা**।

**JavaScript শেখার জন্য Mobile এখন যথেষ্ট।**

Tools Browser Download link:  
https://play.google.com/store/apps/details?id=com.soumitra.toolsbrowser

ধন্যবাদ সবাইকে। সবাই ভালো থাকবেন সুস্থ্য থাকবেন।
