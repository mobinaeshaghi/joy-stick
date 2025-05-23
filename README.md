# joy-stick
گزارش کار آزمایش جوی استیک

نام و نام خانوادگی:مبینا اسحاقی

استاد:اقای دکتر عباسی

 عنوان آزمایش: خواندن جوی‌استیک با آردوینو 🎮
 

🎯 هدف آزمایش
در این آزمایش می‌خوایم با ماژول جوی‌استیک آنالوگ کار کنیم و یاد بگیریم چطور مقادیر محورهای X و Y و دکمه فشاری (SW) رو با استفاده از آردوینو بخونیم و توی Serial Monitor نشون بدیم. هدف اینه که نحوه‌ی کار با ورودی‌های آنالوگ و دیجیتال رو در قالب یه مثال واقعی یاد بگیریم. ✅

🔧 وسایل مورد نیاز:

•	آردوینو UNO

•	جوی‌استیک آنالوگ 🎮

•	کابل USB برای اتصال به کامپیوتر

•	سیم جامپر 🧵

•	بردبورد 🧱


📝 شرح آزمایش جوی‌استیک با آردوینو 🎮:

در این آزمایش قصد داریم عملکرد یک ماژول جوی‌استیک آنالوگ را با استفاده از برد آردوینو UNO بررسی کنیم. این ماژول شباهت زیادی به جوی‌استیک‌های قدیمی کنسول‌های بازی دارد و دارای دو محور حرکتی (X و Y) و یک دکمه‌ی فشاری (SW) است.

جوی‌استیک به صورت داخلی از دو پتانسیومتر (مقاومت متغیر) برای تعیین موقعیت محورهای X و Y استفاده می‌کند. با حرکت دادن اهرم به سمت چپ، راست، بالا یا پایین، مقدار مقاومت تغییر کرده و خروجی آن به صورت یک ولتاژ آنالوگ بین ۰ تا ۵ ولت در پایه‌های VRx و VRy ظاهر می‌شود.

ما این ولتاژهای آنالوگ را با استفاده از پایه‌های آنالوگ A0 و A1 آردوینو خوانده و مقادیر آن‌ها را در Serial Monitor نمایش می‌دهیم. هرچه اهرم بیشتر به یک سمت حرکت کند، مقدار خوانده‌شده از آن پایه به ۰ یا ۱۰۲۳ نزدیک‌تر می‌شود.

همچنین، یک دکمه‌ی داخلی در جوی‌استیک وجود دارد که هنگام فشار دادن اهرم به سمت پایین فعال می‌شود. این دکمه به پایه SW متصل شده و به عنوان ورودی دیجیتال با دستور digitalRead() بررسی می‌شود. برای ساده‌تر شدن مدار، از مقاومت pull-up داخلی آردوینو استفاده می‌کنیم. به همین دلیل در حالت عادی مقدار آن ۱ (HIGH) و هنگام فشار دادن، مقدار آن ۰ (LOW) خواهد بود.

این آزمایش به ما یاد می‌دهد چگونه داده‌های آنالوگ و دیجیتال را هم‌زمان از یک ماژول بخوانیم و در پروژه‌های تعاملی مانند ربات‌ها، بازی‌ها یا کنترلرها از آن استفاده کنیم.

