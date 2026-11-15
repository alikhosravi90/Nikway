# گزارش آزمون و خطا

| آزمون | نتیجه | رسید |
|---|---|---|
| sepehr source compile | PASS | compileall exit 0 |
| sepehr unit tests | NOT_RUN | pytest در محیط پایه نصب نبود |
| mmdju handshake/tools/search | PARTIAL PASS | نسخه 0.9.2، 19 ابزار، 3 نتیجه، قیمت و URL |
| mmdju full verification | PARTIAL/BLOCKED | فرایند پس از مسیرهای اولیه در timeout 20s پایان یافت |
| direct upstream GET | BLOCKED_404 | api.digikala.com/v1/search/?q=هدفون&size=1 HTTP 404 |
| dataset static sample | PASS_STATIC_SAMPLE | DATASET_REPORT، dataset_stats و CSV head |
