from datetime import datetime

# Foydalanuvchidan tug'ilgan kunni kiritishni so'rash (format: YYYY-MM-DD)
birth_input = input("Tug'ilgan kuningizni kiriting (YYYY-MM-DD): ")
  birth_date = datetime.strptime(birth_input, "%Y-%m-%d")

today = datetime.now()

# Joriy yil uchun tug'ilgan kun sanasini yasash
next_birthday = birth_date.replace(year=today.year)

# Agar bu yilgi tug'ilgan kun o'tib ketgan bo'lsa, keyingi yilgisini olamiz
if next_birthday < today:
  next_birthday = next_birthday.replace(year=today.year + 1)

# Qolgan vaqtni (kunlarda) hisoblash
time_difference = next_birthday - today

print(
    f"Keyingi tug'ilgan kuningizgacha {time_difference.days} kun qoldi."
)

