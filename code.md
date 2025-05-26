import os

# Предупреждение
confirm = input("Вы уверены? (y/n): ")
if confirm.lower() == 'y':
    os.system("shutdown /r /t 1")  # /t 1 — задержка 1 секунда
else:
    print("Отменено.")
