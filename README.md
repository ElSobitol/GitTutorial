# Туториал по работе с Git

1. Создаем аккаунт в Github.com
2. Создаем локальный репозиторий командой:
```
git init
```
3. Пробуем подружить локальный и удаленный репозитории Github, при создании нового репозитория с помощью команды: 
```
git remoute add origin <https:/  >
```
4. Отправляем:
```
git push
```
локальный репозиторий в удаленный на Github 
5. При изменении удаленного репозитория выкачиваем в локальный актуальное состояние с помощью команды: 
```
git push
```
## Для работы с чужим репозиторием:

1. Делаем: 
```
fork
```
интересующего нас файла.
2. Создаем: 
```
git clone
```
для нашей версии данного репозитория.
3. Создаем новую ветку:
```
git checkout -b < >
```.
4. Производим все изменения в одной ветке.
5. Отправляем эти изменения в наш аккаунт: 
```
git push
```


6. В окне на Github появляется возможность отправить: 


```
pull request
```.