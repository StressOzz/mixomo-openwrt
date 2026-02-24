ССЫЛКИ:

- https://github.com/Internet-Helper/mixomo-openwrt
- https://github.com/Internet-Helper/mixomo-openwrt/blob/main/files/Советы.md
- https://github.com/Internet-Helper/mixomo-openwrt/blob/main/files/MagiTrickle/MagiTrickle.md

---

# Генерируем WARP

Генерируем **WARP** в TГ боте - https://t.me/warp_generator_bot

<img width="477" height="121" alt="Image" src="https://github.com/user-attachments/assets/f5385211-4ae6-4132-97a5-864ee6daa4b6" />

- Затем на `Подтвердить` (можно выбрать другую локацию для экспериментов)

<img width="461" height="1293" alt="Image" src="https://github.com/user-attachments/assets/c6f512ff-d4e9-4668-821b-c8a17bf58d92" />

- Скачайте `WARP*.conf`
<img width="300" height="497" alt="Image" src="https://github.com/user-attachments/assets/a0a6fa0b-3992-4572-9fe5-5b7fab52419c" />

---

# Установка и удаление Mixomo

- для установки в **SSH** запустите скрипт:
```
sh <(wget -O - https://raw.githubusercontent.com/StressOzz/mixomo-openwrt/refs/heads/main/mixomo_openwrt_install.sh)
```

- для удлаения в **SSH** запустите скрипт:
```
sh <(wget -O - https://raw.githubusercontent.com/StressOzz/mixomo-openwrt/refs/heads/main/mixomo_openwrt_delete.sh)
```
---

- Выберите 1
<img width="473" height="139" alt="Image" src="https://github.com/user-attachments/assets/9a803327-03cb-433f-bac2-31d9958d691b" />

---

# Генерируем конфигурацию

- Зайдите на сайт https://spatiumstas.github.io/web4core/ 

<img width="411" height="693" alt="Image" src="https://github.com/user-attachments/assets/2507d9a9-b4e7-4a89-8a62-958a0cfcae23" />

- Нажмите на <img width="29" height="85" alt="Image" src="https://github.com/user-attachments/assets/685c9527-4c5d-4664-af88-58edaceb7b44" />

- Нажмите на <img width="100" height="91" alt="Image" src="https://github.com/user-attachments/assets/f583ff2a-7b49-4726-baea-3f4dd03a5339" />

- Выберите файл `WARP*.conf`
- Нажмите <img width="90" height="101" alt="Image" src="https://github.com/user-attachments/assets/ed1f3143-1a2e-460d-9e27-cbf8d69b3ae4" />

- Нажмите на  <img width="41" height="150" alt="Image" src="https://github.com/user-attachments/assets/12660858-7a96-4fa3-b0f3-c3bc6bad6a3c" /> это скопирует результат

---

# Настраиваем Mihomo

- Зайдите на роутер в **LuCI**
- Вкладка `Services` → `Mihomo`
- Удалите всё из Конфигурация
- Вставьте скопированный результат
- Внизу нажмите <img width="103" height="69" alt="Image" src="https://github.com/user-attachments/assets/1c620792-a0bd-49d7-8030-ac1ad68442c3" />
- Нажмите <img width="187" height="73" alt="Image" src="https://github.com/user-attachments/assets/cc11862f-ac70-4958-9186-5bed1569705f" />
- Должно появится, что-то типа этого

<img width="797" height="333" alt="Image" src="https://github.com/user-attachments/assets/c5e736d4-c4fa-473e-930d-5cfd98d5d33e" />

- Нажмите на `Запустить` <img width="280" height="73" alt="Image" src="https://github.com/user-attachments/assets/0bc2d735-c50c-4cf6-ac9e-8703b184d3da" />

---

# Сохраняем список доменов

- Переходим по ссылке https://github.com/Internet-Helper/mixomo-openwrt/blob/main/files/MagiTrickle/config_from_internet_helper.mtrickle
- Скачиваем файл `config_from_internet_helper.mtrickle`<img width="197" height="155" alt="Image" src="https://github.com/user-attachments/assets/e07b23d3-f7cb-4fb8-a272-f46199cdd990" />

---

# Настраиваем Magitrickle

- Зайдите на роутер в **LuCI**, вкладка `Services` → `Magitrickle`
- Или зайдите в браузере http://192.168.1.1:8080/
- Удалите `Example` <img width="371" height="401" alt="Image" src="https://github.com/user-attachments/assets/0f1c5f77-c72e-4790-8a22-d9277cfce934" />
- Нажмите `Сохранить изменения` <img width="45" height="111" alt="Image" src="https://github.com/user-attachments/assets/510dce31-20aa-44a1-a92d-6ed2c18fc5e0" />

- Нажмите на Импортировать конфиг <img width="147" height="173" alt="Image" src="https://github.com/user-attachments/assets/70f92a9e-85cb-4fe8-b5ed-b2cb6c6c9a3e" />
- Выбираете `config_from_internet_helper.mtrickle`
- Выбираете `Все` и нажмите `Импортировать` 

<img width="327" height="1105" alt="Image" src="https://github.com/user-attachments/assets/3f6e50dc-5f97-4f6c-abbb-2e7369398324" />

- Нажмите `Сохранить изменения` <img width="45" height="111" alt="Image" src="https://github.com/user-attachments/assets/510dce31-20aa-44a1-a92d-6ed2c18fc5e0" />

---

# Настройки Групп

- Нажмите `Свернуть группу`

<img width="405" height="1441" alt="Image" src="https://github.com/user-attachments/assets/3e839dbb-0b14-4546-bffb-d84acbdb4123" />

- Выберете, то что хотите пустить через `WARP`

---

## После этого должно всё работать...

- Если не работает, выполните `Остановить` и `Запустить` **Mihomo**

---

Можете генерировать разные WARP и пробовать, т.к. в По умолчанию не будет работать `GeoBlock` и ещё всякое...

Для смены WARP:
- Генерируем WARP
- Генерируем конфигурацию
- Настраиваем Mihomo (останавливаем, удаляем, вставляем, сохраняем и запускаем)

---

В общем инструмент вроде не плохой...
Можно по экспериментировать...

---

Совместно с Zapret работает...
Можно использовать как отдельный инструмент, так и в помощь Zapret...

---

## Я не автор и не разработчик !
## Я просто написал эту инструкцию !
## Вопросы по работе данного пакета - не ко мне ! )))
