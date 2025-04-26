# “জাভাস্ক্রিপ্ট ES6: একদম শুরু থেকে এক্সপার্ট”

# অধ্যায় ১: জাভাস্ক্রিপ্ট কী এবং কেন?
# ১.১: জাভাস্ক্রিপ্ট কী?

জাভাস্ক্রিপ্ট হলো একটি প্রোগ্রামিং ভাষা যা মূলত ওয়েব পেজে ডায়নামিক (চলন্ত, ইন্টার‍্যাকটিভ) জিনিস তৈরি করার জন্য ব্যবহৃত হয়।

যখন তুমি কোনো ওয়েবসাইটে:

একটা বাটনে ক্লিক করলে কিছু হয়

টাইমার চলে

চ্যাট বক্সে মেসেজ পাঠাও

মাউস নড়াচড়া করলে কিছু অ্যানিমেশন হয়

তখন এসব কিছুর পেছনে কাজ করে JavaScript।

১.২: জাভাস্ক্রিপ্ট কিভাবে কাজ করে?
তোমার ব্রাউজারে একটা JavaScript Engine থাকে (যেমন Chrome এ V8)।
এই Engine জাভাস্ক্রিপ্ট কোডকে পড়ে এবং কাজ করে।

যেমন:
<button onclick="alert('Hello!')">Click me</button>

তুমি যখন এই বাটনে ক্লিক করো, তখন alert('Hello!') জাভাস্ক্রিপ্ট কোড রান হয়।

# ১.৩: HTML, CSS ও JavaScript এর সম্পর্ক

কাজ	ভাষা
কংকাল / স্ট্রাকচার	HTML
রূপ / ডিজাইন	CSS
প্রাণ / কাজ করা	JavaScript
তিনটি মিলে একটা পূর্ণাঙ্গ ওয়েব পেজ তৈরি হয়।

# ১.৪: কেন JavaScript শিখবো?
১. ওয়েব ডেভেলপমেন্ট শিখতে হলে বাধ্যতামূলক
২. ফ্রন্টএন্ড ও ব্যাকএন্ড দুই দিকেই ব্যবহৃত হয়
৩. অনেক জনপ্রিয় লাইব্রেরি ও ফ্রেমওয়ার্ক (React, Vue, Angular) সব JavaScript ভিত্তিক
৪. চাকরি বা ফ্রিল্যান্সিং — দুই জায়গায়ই চাহিদা

# ১.৫: JavaScript দিয়ে কী কী করা যায়?
ইন্টার‍্যাকটিভ ওয়েবসাইট

গেম

মোবাইল অ্যাপ (React Native)

সার্ভার প্রোগ্রামিং (Node.js)

ডেটা ভিজ্যুয়ালাইজেশন

কৃত্রিম বুদ্ধিমত্তা (AI) ইনটিগ্রেশন




# অধ্যায় ১: জাভাস্ক্রিপ্ট – এক জীবন্ত ভাষার গল্প ....
ধরো, একটা মানুষ আছে — তার নাম "ওয়েবসাইট"।

এই মানুষটার হাড়গোড় বানায় HTML,
তাকে রঙিন জামা কাপড় পরায় CSS,
আর প্রাণ—হাসি, কান্না, কথা বলা, কাজ করা—সব করে দেয় JavaScript।

তুমি যখন একটা বাটনে ক্লিক করো, আর সাথে সাথে কিছু ঘটে—
বুঝে নিও, পেছন থেকে JavaScript বলছে:

“আরে তুমি ক্লিক করছো! এই নাও তোমার রেজাল্ট।”

অধ্যায় ২: ES6 – নতুন যুগের জাভাস্ক্রিপ্ট
সময় বদলায়, প্রযুক্তিও বদলায়।
আগে JavaScript একটু বেয়াড়া ছিলো—মানে যা খুশি করত, গলদ ছিলো।

২০১৫ সালে এল ES6 — এটা এমন এক সংস্করণ যেটা জাভাস্ক্রিপ্টকে আরও পরিণত বানালো।
ES6 মানে হলো "নতুন নিয়ম-কানুন, নতুন সাজ-সজ্জা"।

চলো, দেখি কেমন সেই সাজ।

# ২.১: let, const – দুই ভাই
আগে আমরা লিখতাম:

var name = "Auly";
var মানে তুমি একটা বাক্স বানাও, তাতে কিছু রাখো। কিন্তু দরজা খোলা থাকে—যার ইচ্ছে নেয়, দেয়। অনেক সময় ঝামেলা হয়।

# তাই ES6 বলল:
# "দুই নতুন বাক্স দিচ্ছি—let আর const"

let name = "Auly";   // দরকার হলে নাম পাল্টাবে
const pi = 3.1416;   // এইটা চিরস্থায়ী সত্য—পাল্টানো যাবে না
২.২: Arrow Function – ছোট কবিতা
আগে একটা কাজ করার জন্য লিখতে হতো অনেক লাইন:

function greet(name) {
  return "Hello " + name;
}
# ES6 বলল:
# "তুমি তো কবি, কম লাইনে কাজ শেষ করো না?"


const greet = (name) => Hello ${name};
এমনকি যদি আরগুমেন্টও না থাকে:
const sayHi = () => "Hi there!";
২.৩: Template Literals – শব্দের খেলাঘর
তুমি যদি আগের মতো লিখো:


let msg = "Hello " + name + ", how are you?";
নতুন ES6 তোমাকে বলল, কবিতার মতো লিখো:


let msg = Hello ${name}, how are you?;
একই বাক্যে ভিন্ন শব্দ ঢোকাও সহজে।

# ২.৪: Destructuring – অংশ থেকে পুরোটা চিনে ফেলা
# একটা জিনিসের ভেতর থেকে সরাসরি প্রয়োজনীয় অংশ তুলে আনার নাম Destructuring.

const person = { name: "Auly", age: 22 };

const { name, age } = person;
// এখন সরাসরি name ও age ব্যবহার করা যাবে


# অধ্যায় ৩: স্প্রেড, রেস্ট আর ফাংশনের খেলা
জাভাস্ক্রিপ্টে অনেক কিছু আছে যেন জাদুর মতো।
এই অধ্যায়ে আমরা শিখবো তিনটা জাদুর মতো জিনিস:

১. Spread Operator
২. Rest Operator
৩. ফাংশন কীভাবে কাজ করে, আর কিভাবে তুমি নিজের মতো বানাতে পারো

৩.১: Spread Operator (…) — ছড়িয়ে দাও
ধরো, তোমার কাছে একটা থালা আছে।
এই থালায় আছে কিছু ফল:

const fruits = ["apple", "banana", "orange"];
তুমি এখন আরেকটা থালা বানাতে চাও, যেটাতে আগের ফলগুলো থাকবে, সাথে নতুন কিছু।

আগে কী করতে হতো?


const newFruits = [fruits[0], fruits[1], fruits[2], "mango"];
ঝামেলা!

# ES6 বলল: নাও, Spread দিয়ে ছড়িয়ে দাও:


const newFruits = [...fruits, "mango"];
এখানে ...fruits মানে হলো:
“fruits নামের থালাটা খুলে দাও, ভিতরের সব ফল বের করে আনো”

আরে বাহ! ছড়ানো একটা মজা!

# ৩.২: Rest Operator (…) — সবকিছু একত্র করো
এটা একটু উল্টো।

ধরো, তুমি একটা ফাংশন বানাও যেটা অনেকগুলো সংখ্যা যোগ করে।

আগে একটা নির্দিষ্ট পরিমাণ সংখ্যা নিতে হতো:


function add(a, b, c) {
  return a + b + c;
}
কিন্তু তুমি তো জানো না কতগুলো সংখ্যা আসবে!

ES6 বলল: "…rest" দিয়ে সব কিছুকে একটা বস্তায় ভরে নাও:


function add(...numbers) {
  let sum = 0;
  for (let num of numbers) {
    sum += num;
  }
  return sum;
}

add(1, 2, 3);        // 6
add(10, 20, 30, 40); // 100
তুমি যত ইচ্ছা সংখ্যাই দাও, “...numbers” সবার জন্য একটা ব্যাগ!


# ৩.৩: ফাংশন — নিজের বানানো জাদুকর
ফাংশন মানে তুমি নিজের বানানো এক জাদুকর।

ধরো তুমি একটা গান গাও:

function sing() {
  console.log("La la la...");
}
এখন তুমি সেই গান গাওয়াতে চাইলে:

sing(); // La la la...
তুমি চাইলে এই জাদুকরকে কিছু দিয়ে দিতে পারো:

function greet(name) {
  console.log(Hello, ${name}!);
}

greet("Auly"); // Hello, Auly!
এটা এমন, তুমি “name” নামের একটা উপহার দাও, আর সে সেই নাম ধরে ডাকে।

# Bonus: Arrow Function – নতুন ঢঙের কবিতা  একই কাজ নতুনভাবে:

const greet = (name) => {
  console.log(Hello, ${name}!);
}
এই হলো Arrow Function — কম কথায় বেশি কাজ।

# এই অধ্যায়ে যা শিখলে (Recap):
... মানে দুইটা ভিন্ন ম্যাজিক — একবার ছড়িয়ে (Spread), একবার একত্র (Rest)

ফাংশন হলো তোমার নিজের বানানো যন্ত্র — তুমি বললে কাজ করবে

ফাংশনে তুমি চাইলে উপহার পাঠাতে পারো (argument), আর সেটা দিয়ে কাজ করাবে |



# অধ্যায় ৪: অবজেক্ট, ডিস্ট্রাকচারিং আর ক্লাস — জাভাস্ক্রিপ্টের চরিত্র গঠন
জাভাস্ক্রিপ্টকে যদি একটা সিনেমা ধরা হয়, তাহলে এই অধ্যায় তার চরিত্র নির্মাণের গল্প।
মানে, তুমি যাদের নিয়ে কাজ করবে, তাদের সব বৈশিষ্ট্য, আচরণ, সবকিছু এখানেই গড়ে তুলবে।

# ৪.১: অবজেক্ট (Object) — একটি চরিত্রের খতিয়ান
তুমি যেমন — নাম আছে, বয়স আছে, পছন্দ অপছন্দ আছে —
তেমনি জাভাস্ক্রিপ্টেও একেকটা জিনিসকে "Object" দিয়ে বানানো যায়।

# উদাহরণ:

const poet = {
  name: "Auly",
  age: 24,
  write: function() {
    console.log("আমি কবিতা লিখি...");
  }
};
# এই poet কে যদি বলো তার নাম কী?

console.log(poet.name); // Auly

# তাকে বলো লেখো তো:

poet.write(); // আমি কবিতা লিখি...
# Object মানে হলো: একটা জিনিস যেটার অনেক গুণ আছে।

# ৪.২: Destructuring — বড় কাহিনির ছোট ছোট অংশ টেনে বের করা
তুমি যদি পুরো poet Object থেকে শুধু নাম আর বয়স নিতে চাও, তাহলে কী করো?

আগে করতে হতো:

const name = poet.name;
const age = poet.age;

# ES6 বলল: ছোট করে নাও ভাই!

const { name, age } = poet;
console.log(name); // Auly
console.log(age);  // 24
# একে বলে Destructuring — বড় কিছু থেকে ছোট ছোট টুকরা তুলে নেওয়া।

# আরেকটা উদাহরণ: Array Destructuring

const colors = ["red", "green", "blue"];
const [firstColor, secondColor] = colors;
console.log(firstColor);  // red
console.log(secondColor); // green


# ৪.৩: ক্লাস (Class) — নিজের মতো চরিত্র বানাও
তুমি যদি নিজেই একটা Object এর কাঠামো তৈরি করতে চাও,
তাহলে তুমি একটা Class বানাতে পারো।

# Class মানে হলো – প্ল্যান। আর Object মানে হলো – সেই প্ল্যান থেকে বানানো জিনিস।

চলো উদাহরণ দেখি:

class Poet {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  write() {
    console.log(${this.name} লিখছে কবিতা...);
  }
}
এখন তুমি চাইলে কবিদের বানাতে পারো:

const poet1 = new Poet("Auly", 24);
const poet2 = new Poet("Rafiq", 30);

poet1.write(); // Auly লিখছে কবিতা...
poet2.write(); // Rafiq লিখছে কবিতা...
এখানে constructor() হলো জন্মদাতা — Object তৈরির সময় চালু হয়।
আর this.name মানে হলো — ওই Object এর নিজের নাম।


# এই অধ্যায়ের সারাংশ:

জিনিস	মানে	উদাহরণ
Object	একাধিক গুণ-সম্পন্ন বস্তু	const person = {name: "Auly"}
Destructuring	Object/Array থেকে অংশ বের করা	const {name} = person
Class	চরিত্র বা Object তৈরির খাঁচা	class Poet { ... }



# অধ্যায় ৫: Promise আর Async – সময়ের সাথে খেলা
তুমি তো জানো, কবিতা যেমন ধীরে ধীরে হৃদয়ে গেঁথে যায়,
তেমনি কিছু কিছু কাজ আছে যেগুলো একটু সময় নেয়।

জাভাস্ক্রিপ্ট বলল —

“আমি সবসময় সোজাসুজি চলি না ভাই। কিছু কাজ থাকে যেগুলো এখনই শেষ হবে না, একটু পরে হবে।”

এইরকম দেরি করে শেষ হওয়া কাজকে বলে Asynchronous কাজ।

# ৫.১: প্রমিস (Promise) — ওয়াদা রইলো!
ধরো তুমি এক বন্ধুকে বললা:

“তুই যদি কবিতা লিখে আনিস, আমি তোকে চা খাওয়াবো।”

বন্ধু বললো:
“প্রমিস করলাম।”

এটাই হলো JavaScript এর Promise!

let myPromise = new Promise(function(resolve, reject) {
  let poemWritten = true;

  if (poemWritten) {
    resolve("চা খাওয়ানো হবে!");
  } else {
    reject("তুই তো কবিতা আনিস নি!");
  }
});
এখন তুমি যদি সেই প্রমিসে বিশ্বাস রাখতে চাও:

myPromise
  .then(function(message) {
    console.log("Success:", message);
  })
  .catch(function(error) {
    console.log("Error:", error);
  });

 # ৫.২: async/await — ধৈর্যের খেলা
তুমি যদি প্রমিসের ওপর বসে চুপচাপ অপেক্ষা করতে চাও, তাহলে async/await ব্যবহার করতে পারো।

async function bringTea() {
  try {
    const result = await myPromise;
    console.log(result);  // চা খাওয়ানো হবে!
  } catch (error) {
    console.log(error);   // তুই তো কবিতা আনিস নি!
  }
}

bringTea();
এখানে await মানে:
"আমি অপেক্ষা করছি যতক্ষণ না তুমি প্রমিস রাখো।"

# এই অধ্যায়ের মূল কথা:
Promise হলো একটা ওয়াদা — পরে গিয়ে ঠিক বা ভুল হবে

.then() দিয়ে তুমি বলো, "ওয়াদা পূর্ণ হলে কী হবে"

.catch() দিয়ে বলো, "ওয়াদা ভাঙলে কী হবে"

async/await হলো — ধীরে সুস্থে, ধৈর্যের সাথে, গল্পের মতো অপেক্ষা


# অধ্যায় ৬: মডিউল, ইমপোর্ট আর এক্সপোর্ট — নিজের কোড ভাগ করে পৃথিবীকে দাও
ধরো, তুমি একটা বড় কবিতার বই লিখছো।
তুমি কি সব কবিতা এক পাতায় লিখবে?
না! তুমি বলবে —

“এই পাতায় প্রেমের কবিতা, ওই পাতায় প্রকৃতির কবিতা…”

একইভাবে, জাভাস্ক্রিপ্টেও আমরা বড় কোডকে ছোট ছোট ফাইলে ভাগ করে রাখি।
আর এই ভাগ করা, আদান-প্রদানের পুরো ব্যাপারটাকেই বলে Modules।

# ৬.১: export — কোডকে বাইরের দুনিয়ায় পাঠাও
ধরো, একটা poem.js ফাইল আছে। এখানে তুমি একটা ফাংশন লিখছো:

// poem.js
export function writePoem() {
  console.log("আমি একটি সুন্দর কবিতা লিখছি...");
}
এখানে export মানে হলো —
"এই ফাংশনটা বাইরে পাঠানো হচ্ছে, যাতে অন্য ফাইল থেকে ব্যবহার করা যায়।"

তুমি চাইলে একটা ভেরিয়েবলও export করতে পারো:

export const poetName = "Auly";

# ৬.২: import — অন্যের লেখা নিজের কোডে এনে ব্যবহার করো
এখন তুমি আরেকটা ফাইলে (ধরো main.js) ওই ফাংশন আনতে চাও।

// main.js
import { writePoem, poetName } from './poem.js';

writePoem();            // আমি একটি সুন্দর কবিতা লিখছি...
console.log(poetName);  // Auly
এটাই হলো মডিউল সিস্টেম!
তুমি নিজের কোডকে ভাগ করে রাখছো —
আর যেখানে দরকার, শুধু দরকারি অংশটুকু নিয়ে নিচ্ছো।

# ৬.৩: Default Export — একবারে একটাই পাঠাও
তুমি চাইলে একটা ফাইলে একটামাত্র জিনিস default দিয়ে পাঠাতে পারো।

// poet.js
export default function poemStyle() {
  console.log("গভীর আবেগে ভরা ছন্দে লিখি কবিতা...");
}
এখন ইমপোর্ট করার সময় নাম চেঞ্জ করে নিতে পারো:

// main.js
import poem from './poet.js';

poem(); // গভীর আবেগে ভরা ছন্দে লিখি কবিতা...
এই অধ্যায়ের সারাংশ:

# কাজ	কীভাবে	মানে
export	export function...	অন্য ফাইলকে কিছু পাঠানো
import	import { name } from...	অন্য ফাইল থেকে কিছু আনা
default export	export default ...	একটাই জিনিস পাঠানো, ইচ্ছেমতো নামে আনা যায়|


# অধ্যায় 7: ES6 এর বাকি কিছু গুরুত্বপূর্ণ বিষয়
তুমি যেভাবে আগের অংশগুলো শিখেছো, এবার সেভাবে class, modules, generator, iterators, map ও set সম্পর্কে বুঝবো।

# 7.1: ক্লাস (Classes) — নতুনদের জন্য সহজ ওয়ার্কফ্লো
এটি ES6 এ নতুনভাবে এসেছে। আগে জাভাস্ক্রিপ্টে prototype নিয়ে কাজ করা লাগতো, কিন্তু class এর মাধ্যমে কোড লেখা অনেক সহজ হয়ে গেছে।

ক্লাস এর মাধ্যমে তুমি object-oriented programming (OOP) স্টাইলের কোড লিখতে পারো।

// ক্লাস তৈরি
class Poet {
  constructor(name, age) {
    this.name = name;
    this.age = age;
  }

  // method তৈরি
  writePoem() {
    console.log(${this.name} কবিতা লিখছে...);
  }
}

// ক্লাস ব্যবহার
const poet1 = new Poet('Auly', 24);
poet1.writePoem(); // Auly কবিতা লিখছে...
এখানে Poet ক্লাস তৈরি করেছি এবং constructor এর মাধ্যমে name আর age প্রপার্টি সেট করেছি। তারপর writePoem() মেথড তৈরি করেছি, যাতে কবি কবিতা লেখে।

# 7.2: মডিউলস (Modules) — কোড ভাগ করে কাজ করা
আমরা আগেই শিখেছি যে modules দিয়ে আমরা কোড ভাগ করে রাখতে পারি। এখানে দুইটি ফাইলের উদাহরণ:

poem.js (অন্য ফাইলে):

export const poetName = 'Auly';
export function writePoem() {
  console.log(${poetName} কবিতা লিখছে...);
}
main.js (ব্যবহারকারী ফাইল):

import { poetName, writePoem } from './poem.js';

console.log(poetName);   // Auly
writePoem();            // Auly কবিতা লিখছে...
এখানে export দিয়ে কিছু data এবং function পাঠানো হয়েছে, আর import দিয়ে আমরা সেগুলো ব্যবহার করছি।

# 7.3: জেনারেটর (Generators) — স্টপ & রেসুম এর মজা
জেনারেটর ফাংশনগুলোর মধ্যে তুমি yield ব্যবহার করতে পারো, যাতে ফাংশন থেকে কিছু value ফেরত পায়। তুমি যখন চাও, তখন yield দিয়ে return করতে পারো, তারপর আবার ফাংশন চালু করতে পারো।

function* poemGenerator() {
  yield 'প্রথম কবিতা';
  yield 'দ্বিতীয় কবিতা';
  yield 'তৃতীয় কবিতা';
}

const poems = poemGenerator();

console.log(poems.next().value);  // প্রথম কবিতা
console.log(poems.next().value);  // দ্বিতীয় কবিতা
console.log(poems.next().value);  // তৃতীয় কবিতা
এখানে * দিয়ে ফাংশনকে generator বানানো হয়েছে, এবং next() দিয়ে next value পাওয়া যাচ্ছে। yield একে একে value ফেরত দেয়।

# 7.4: ইটারেটরস (Iterators) — যেকোনো কোডে আগাতে থাকো
iterators হচ্ছে Object বা array এর মধ্যে একে একে চলা। এটি এমনভাবে কাজ করে যেন তুমি একবারে একটা করে value এক্সেস করতে পারো।

ধরা যাক, তোমার কাছে একটা array আছে:

let poems = ['Poem 1', 'Poem 2', 'Poem 3'];

let iterator = poems[Symbol.iterator]();

console.log(iterator.next().value);  // Poem 1
console.log(iterator.next().value);  // Poem 2
console.log(iterator.next().value);  // Poem 3
এখানে Symbol.iterator দিয়ে poems array এর ইটারেটর তৈরি করেছি। এরপর next() দিয়ে একে একে আইটেমগুলো পেয়েছি।

# 7.5: Map — Key/Value দিয়ে ডাটা সংরক্ষণ
Map এ তুমি key/value পেয়ার দিয়ে ডাটা সংরক্ষণ করতে পারো। এটা অনেক ভালো, কারণ Map এমনভাবে কাজ করে যা object এর চেয়ে বেশি সুবিধাজনক।

let poetMap = new Map();

poetMap.set('Auly', 'Poet');
poetMap.set('Kamal', 'Writer');
poetMap.set('Rana', 'Artist');

console.log(poetMap.get('Auly'));  // Poet
console.log(poetMap.has('Rana'));  // true
console.log(poetMap.size);         // 3
এখানে set() দিয়ে key/value পেয়ার যোগ করেছি, get() দিয়ে value বের করেছি, আর has() দিয়ে চেক করেছি key আছে কিনা।

# 7.6: Set — ইউনিক মান সংরক্ষণ
Set দিয়ে তুমি শুধুমাত্র ইউনিক মান (duplicates ছাড়া) সংরক্ষণ করতে পারো।

let poetsSet = new Set();

poetsSet.add('Auly');
poetsSet.add('Kamal');
poetsSet.add('Auly'); // Duplicate value

console.log(poetsSet);  // Set { 'Auly', 'Kamal' }
এখানে add() দিয়ে ডাটা যোগ করেছি। Set আউটপুট দেখায়, duplicate মানগুলো রাখা হয়নি।

# 7.7: Object Destructuring (এটা কিছুটা আগে বলেছিলাম)
Object Destructuring দিয়ে তুমি একসাথে অনেকগুলো প্রপার্টি বের করতে পারো:

const poet = {
  name: 'Auly',
  age: 24,
  genre: 'Poetry'
};

const { name, age } = poet;
console.log(name);  // Auly
console.log(age);   // 24
এখানে {} ব্রেস ব্যবহার করে object এর প্রপার্টি বের করেছি একসাথে।

# এখন তুমি পুরো ES6 শিখে ফেলেছো!
তুমি এখন JavaScript এর অনেক শক্তিশালী ফিচার বুঝতে পারো, যেমন:

Classes দিয়ে ক্লাস বানানো

Modules দিয়ে কোড ভাগ করে রাখা

Generators দিয়ে প্রগ্রাম স্টপ করা

Iterators দিয়ে array/object ট্রাভার্স করা

Map ও Set দিয়ে ইউনিক ডাটা ও key-value পেয়ার ম্যানেজ করা



# অবশ্যই! এখন পর্যন্ত তুমি JavaScript ES6 এর বেশ কিছু গুরুত্বপূর্ণ বিষয় শিখেছো। নিচে সবগুলোকে একটি লিস্ট আকারে দেয়া হলো:

# JavaScript ES6 শিখেছি:

# 1. Let ও Const
       _ let ও const ব্যবহার করে ভ্যারিয়েবল ডিক্লেয়ার করা।

       _ const এর মাধ্যমে অপরিবর্তনীয় মান সেট করা।

# 2. Arrow Functions (এ্যারো ফাংশন)

      _ এ্যারো ফাংশন ব্যবহার করে সংক্ষিপ্তভাবে ফাংশন লেখা।

# 3. Template Literals (টেমপ্লেট লিটারাল)

       _ Backticks ব্যবহার করে মাল্টিলাইন স্ট্রিং এবং ডাইনামিক ভ্যালু ইনজেক্ট করা।



# 4. Destructuring

       _ Array ও Object এর ডাটা সরাসরি বের করা।

# 5. Spread & Rest Operators

        _ Spread (...) দিয়ে array বা object এর ভ্যালু এক্সটেন্ড করা।

        _ Rest (...) দিয়ে ফাংশনে অনেক আর্গুমেন্ট নেয়া।

# 6. Default Parameters (ডিফল্ট প্যারামিটারস)

        _ ফাংশনে ডিফল্ট মান সেট করা।

# 7. Promises & Async/Await (প্রমিস ও অ্যাসিঙ্ক/অওয়েট)

        _ Promises ব্যবহার করে অ্যাসিঙ্ক্রোনাস কোড লেখা।

        _ Async/Await এর মাধ্যমে সহজভাবে অ্যাসিঙ্ক্রোনাস কোড লেখা।

# 8. Classes (ক্লাসেস)

        _ Class ও Constructor ব্যবহার করে অবজেক্ট তৈরি করা।

# 9. Modules (মডিউলস)

      _ export ও import দিয়ে কোড ভাগ করে রাখা।

# 10. Generators (জেনারেটরস)

        _ yield ব্যবহার করে জেনারেটর ফাংশন থেকে ভ্যালু ফেরত পাওয়া।

# 11. Iterators (ইটারেটরস)

        _ Symbol.iterator ব্যবহার করে array বা object ট্রাভার্স করা।

# 12. Map

        _ Map ব্যবহার করে key/value পেয়ার সংরক্ষণ করা এবং সহজে অ্যাক্সেস করা।

# 13. Set

        _ Set ব্যবহার করে unqiue values সংরক্ষণ করা।

# 14. Object Destructuring (অবজেক্ট ডেস্ট্রাকচারিং)

      _ অবজেক্টের বিভিন্ন প্রপার্টি একসাথে বের করা।