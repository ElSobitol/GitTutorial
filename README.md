# Туториал Git. Часть 2.

1. ## Как скопировать внешний репозиторий на свой ПК?
```
git clone <url-адрес репозитория> – клонирование внешнего репозитория на  локальный ПК

```
Чтобы склонировать внешний репозиторий на наш ПК необходимо воспользоваться комадой `git clone <url-адрес репозитория>`

2. ## Как выкачать (pull) актуальное состояние из удалённого репозитория?
```
git pull – получение изменений и слияние с локальной версией
```
 Эта команда позволяет скачать все из текущего репозитория и автоматически сделать merge с нашей версией

3. ## Как отправляем изменения с локального репозитория в удаленный? 
```
   git push – отправляет локальную версию репозитория на внешний
```
эта команда позволяет отправить нашу версию репозитория на внешний
репозиторий.

4. ## Как сделать pull request?

* Делаем fork репозитория

* Делаем clone СВОЕЙ версии репозитория

* Создаем новую ветку и в НЕЕ вносим свои изменения

* Фиксируем изменения (делаем коммиты)

* Отправляем свою версию в свой GitHub

* На сайте GitHub нажимаем кнопку pull request