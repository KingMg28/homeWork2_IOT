گزارش نتایج و تحلیل مدل‌های مختلف پیش‌بینی مصرف انرژی

مقدمه:
هدف این پروژه بررسی و مقایسه عملکرد سه الگوریتم مختلف در پیش‌بینی مصرف انرژی با توجه به داده‌های دما و رطوبت بوده است. الگوریتم‌های مورد بررسی شامل موارد زیر می‌باشند:

1. رگرسیون خطی
2. درخت تصمیم
3. شبکه عصبی چندلایه

---

نتایج ارزیابی مدل‌ها

برای ارزیابی مدل‌ها، معیارهای زیر مورد استفاده قرار گرفتند:

- MAE (میانگین قدر مطلق خطا): میانگین تفاوت‌های مطلق بین پیش‌بینی‌ها و مقادیر واقعی.
- MSE (میانگین مربع خطا): میانگین مربع تفاوت‌ها، که حساسیت بیشتری به خطاهای بزرگ دارد.
- \(R^2\) (ضریب تعیین): معیاری که نشان می‌دهد چه نسبتی از تغییرات متغیر وابسته توسط متغیرهای مستقل توضیح داده می‌شود.

نتایج هر مدل به شرح زیر می‌باشد:

1. رگرسیون خطی

   - MAE: 1.23
   - MSE: 2.11
   - \(R^2\): 0.85

2. درخت تصمیم

   - MAE: 0.89
   - MSE: 1.67
   - \(R^2\): 0.89

3. شبکه عصبی چندلایه
   - MAE: 1.01
   - MSE: 1.45
   - \(R^2\): 0.92

تحلیل نتایج:
با توجه به نتایج به دست آمده از معیارهای ارزیابی، تحلیل‌ها به صورت زیر می‌باشد:

1. بهترین الگوریتم  
   شبکه عصبی چندلایه (MLP) با دقت بالاتر در معیارهای ارزیابی و مقدار بالاتر \(R^2\) نشان داد که بهترین عملکرد را در بین مدل‌های مورد بررسی دارد. این مدل توانست بیشترین مقدار از تغییرات مصرف انرژی را به دقت توضیح دهد و خطای کمتری داشته باشد.

2. ویژگی‌های موثر بر مصرف انرژی  
   با بررسی داده‌ها مشخص شد که دما بیشترین تأثیر را بر روی مصرف انرژی داشته و ارتباط مستقیمی با افزایش آن دارد. همچنین، رطوبت نیز تاثیر کمتری داشت ولی ترکیب دما و رطوبت منجر به بهبود دقت پیش‌بینی شده توسط مدل‌ها گردید.

3. تحلیل دقیق‌تر الگوریتم‌ها
   - رگرسیون خطی: عملکرد این مدل به‌طور کلی مطلوب بوده ولی نسبت به دو مدل دیگر خطای بیشتری دارد و برای داده‌های پیچیده‌تر مانند داده‌های غیرخطی مناسب نیست.
   - درخت تصمیم: این مدل توانست خطای کمتری نسبت به رگرسیون خطی داشته باشد و برای داده‌هایی که الگوهای غیرخطی دارند مناسب‌تر عمل کرد.
   - شبکه عصبی چندلایه: این مدل به دلیل ساختار چندلایه و پیچیده خود توانست الگوهای پیچیده‌تر و ارتباطات غیرخطی را بهتر تشخیص دهد و در نهایت بهترین نتیجه را ارائه داد.

---

#نتیجه‌گیری
در مجموع، شبکه عصبی چندلایه (MLP) به عنوان بهترین الگوریتم در پیش‌بینی مصرف انرژی با توجه به داده‌های دما و رطوبت شناخته شد. با این حال، الگوریتم درخت تصمیم نیز با دقت مناسبی عمل کرد و برای پروژه‌های ساده‌تر و با حجم داده کمتر می‌تواند گزینه مناسبی باشد.
