# AIR – Резидент Искусственного Интеллекта

*Полностью автономный AI-помощник для вашего терминала.*

---

## Установка (скопируйте и выполните эти команды)

1. Установите Ollama:

curl -fsSL https://ollama.com/install.sh | sh

2. Скачайте модель:

ollama pull qwen2.5:7b-q4_K_M

3. Клонируйте репозиторий AIR:

git clone https://github.com/snietOFF/AIR-Artificial-Intelligence-Resident.git
cd AIR-Artificial-Intelligence-Resident

4. Создайте виртуальное окружение и установите AIR:

python3 -m venv venv
source venv/bin/activate
pip install -e .

5. Запустите AIR:

air --model ollama/qwen2.5:7b-q4_K_M

После этой команды вы попадёте в интерактивный режим.

---

## Настройка по умолчанию

Создайте файл ~/.air.conf.yml со строками:

model: ollama/qwen2.5:7b-q4_K_M
check-update: false
show-model-warnings: false

Теперь команда air будет запускаться с этой моделью автоматически.

---

## Лицензия

Apache License 2.0. Свободное использование, изменение и распространение.
