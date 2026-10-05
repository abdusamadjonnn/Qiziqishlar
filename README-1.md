# Qiziqishlarim

O'quvchilar o'z qiziqishlari bo'yicha do'st topadigan va AI Ustoz bilan o'rganadigan Flask sayti.

## Lokal ishga tushirish
```
pip install -r requirements.txt
python app.py
```
Sayt: http://127.0.0.1:5000

## Muhit o'zgaruvchilari
| Nomi | Vazifasi |
|---|---|
| `SECRET_KEY` | Sessiya uchun maxfiy kalit (uzun tasodifiy matn) |
| `ADMIN_PASSWORD` | Admin paroli (login: `admin`) |
| `OPENAI_API_KEY` | AI Ustoz uchun OpenAI kaliti |
| `DB_PATH` | (ixtiyoriy) SQLite fayl manzili |

## Internetga chiqarish (Render.com)
1. Kodni GitHub'ga yuklang.
2. render.com → New → Web Service → GitHub repozitoriyni tanlang.
3. Build: `pip install -r requirements.txt`, Start: `gunicorn app:app`.
4. Environment bo'limida yuqoridagi o'zgaruvchilarni kiriting.
