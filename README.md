# پرسش اول

همانطور که گفته شده برای سادگی آزمایش لازم نیست در لیست تراکنش ها منفی نشدن را در هر لحظه بررسی کنیم اما در نهایت نباید به ازای یک لیست تراکنش موجودی حساب منفی شود. این در حالی است که در سناریو هایی که برای تست در نظر گرفته شده، در هیچ موردی برداشت بیشتر از واریز نبوده و لذا این حالت بررسی نمیشده. از آنجایی که کلیت عملکرد برنامه درست است و حتی یک تست شامل هر دوی واریز و برداشت نوشته شده، احتمالا حواس برنامه نویس از وجود این خطا پرت شده است.

# پرسش دوم

ابتدا تستی به نام

testCalculateBalanceThrowsErrorWhenNegative

اضافه کردیم که در صورت منفی شدن موجودی خطایی را برگرداند. طبیعتا قبل از اعمال تغییر در کد این تست به این صورت فیل میشد:

edu.sharif.selab.AccountBalanceCalculatorTest.testCalculateBalanceThrowsErrorWhenNegative -- Time elapsed: 0.007 s <<< FAILURE!
org.opentest4j.AssertionFailedError: Balance cannot be negative ==> Expected java.lang.IllegalArgumentException to be thrown, but nothing was thrown.

سپس با اعمال تغییر در متد مربوطه، این تست نیز با موفقیت پاس شد.

Tests run: 7, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.051 s -- in edu.sharif.selab.AccountBalanceCalculatorTest
