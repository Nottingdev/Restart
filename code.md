import os
import time
import subprocess

for i in range(100):
    # Завершить процесс explorer.exe
    os.system("taskkill /f /im explorer.exe")
    time.sleep(1)  # Подождать, чтобы процесс завершился

    # Запустить explorer.exe снова
    subprocess.Popen("explorer.exe")
    time.sleep(1)  # Подождать, чтобы explorer загрузился

    print(f"Перезапуск проводника: {i + 1}/100")
print("Готово!")
