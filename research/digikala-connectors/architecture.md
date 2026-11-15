# معماری پیشنهادی اتصال

1. آداپتر Sepehr در محیط ایزوله با فقط egress به دامنه‌های اعلام‌شده، بدون توکن و بدون ابزار نوشتن.
2. provenance شامل source_url، retrieved_at، tool، response_hash، raw_status و schema_version.
3. سقف نرخ محافظه‌کارانه، صف کوچک، timeout، retry محدود و قطع fail-closed برای 403/429/5xx.
4. نرمال‌سازی قیمت با حفظ واحد (ریال upstream / تومان نمایش) و ثبت تبدیل.
5. جداسازی داده خام از ادعاهای ممیزی؛ انتشار فقط رکوردهای مجاز و بدون PII.
6. mmdju فقط منبع آزمایشی موقت، نه وابستگی تولیدی؛ dataset فقط corpus تاریخی با attribution.
