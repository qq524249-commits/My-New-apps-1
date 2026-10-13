তেঘরিয়া আল-কারীম ইসলামী যুব সংগঠন — PWA Starter

ফাইলসমূহ:
- index.html: অ্যাপের স্ক্রিন ও demo form
- manifest.json: PWA/app metadata
- service-worker.js: basic offline caching
- icons/: Android app icons

মোবাইল থেকে APK তৈরির মোটামুটি ধাপ:
1. ZIP extract করুন।
2. সব ফাইল একসঙ্গে একটি public HTTPS static hosting-এ publish করুন। উদাহরণ: GitHub Pages বা অন্য static hosting।
3. প্রকাশিত সাইট URL Chrome-এ খুলে পরীক্ষা করুন; manifest.json এবং icons লোড হচ্ছে কি না দেখুন।
4. https://www.pwabuilder.com/ খুলে আপনার live HTTPS URL দিন।
5. Package for stores → Android → Generate Package নির্বাচন করুন।
6. নাম: তেঘরিয়া আল-কারীম ইসলামী যুব সংগঠন; short name: আল-কারীম যুব; package ID উদাহরণ: org.teghoria.alkarimyouth (নিজস্ব unique ID নিশ্চিত করুন)।
7. Testing-এর জন্য APK থাকলে ডাউনলোড করে ফাইলটি খুলুন। যদি শুধু AAB আসে, APK অপশন/Other Android package নির্বাচন আছে কি না দেখুন।

গুরুত্বপূর্ণ:
- এই starter-এ আবেদন localStorage-এ থাকে, অনলাইন ডেটাবেস নয়।
- এটি কেবল প্রাথমিক demo, নিরাপদ সদস্য ব্যবস্থাপনার জন্য প্রস্তুত নয়।
- বাস্তব সদস্যের তথ্য রাখার আগে Firebase/backend, authentication, server-side authorization, privacy policy, backups ও security testing যোগ করতে হবে।
- PWA packaging-এ live HTTPS URL আবশ্যক; স্থানীয় index.html ফাইলের পথ সরাসরি PWABuilder-এ দেওয়া যাবে না।
