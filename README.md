# Toxin
Project for Toxin hotel
Описание задания
Макет страниц по поиску номеров в отеле находится по ССЫЛКЕ . 

В макете две вкладки. На первой вкладке представлен UI Kit, а на второй вкладке сами страницы по поиску номеров отеля. Переключение между вкладками находится в левом верхнем углу, рядом со значком ладошки.

Прошлая версия задания: ранее требовалось сверстать макет резюме и макет UI Kit, сейчас эти макеты заменены одним проектом, описанным выше. Тем, кто уже начал делать прошлую версию, можно продолжать работать по ней.
---
Рекомендуем познакомиться со стандартами разработки (bestpractices) перед началом практического задания. По данным стандартам, на 5м задании, будет проводится код-ревью ваших проектов. Имеет смысл делать сразу по этим стандартам, чтобы ревью прошло быстрее. Ссылка на стандарты продублирована сюда из 5го задания.
---

Требования к верстке:
* Вся вёрстка должна быть выложена на Github в ваш публичный репозиторий, результатом задачи будет как раз этот репозиторий. Под каждый проект создаём новый репозиторий. Присылать ссылку на него необязательно, это можно будет сделать только в пятом задании в личные сообщения организатору.
* Для второго задания выделить отдельный репозиторий (мы потом отдельные issues можем туда делать). Макет опубликовать через Github Pages: https://youtu.be/9h1UiqBuxO0, чтобы мы могли быстро проверить конечный результат.
* Ссылку на Github Pages добавить в Readme проекта, чтобы мы при проверке могли быстро перейти к самой вёрстке.
* С начала работы коммиты в репозиторий делать как можно чаще, минимум раз в день, когда было что-то сделано, а лучше чаще (для каждого нового блока). Не надо копить многодневную работу и сваливать это одним коммитом, для таких вещей лучше использовать ветки. Не бойтесь незаконченные изменения коммитить, в этом нет ничего страшного.
* Все коммиты должны иметь осмысленные названия.
* Ориентироваться на последние версии Chrome и Firefox. На Safari и старые IE можно не обращать внимания для этих заданий
* Все отступы и размеры элементов должны быть соблюдены, для этого во время работы используйте расширение
* Все шрифты должны быть подключены и сгенерированы в форматах .ttf, .woff, .svg, в сервисе Font2Web
* Количество картинок должно быть минимальным: если элемент состоит из текста, он должен быть текстовым, если элемент — это просто круг, сделать его чистым css, без картинок
* Все страницы должны быть по максимуму responsive (здесь примеры чем responsive отличается от adaptive и liquid). Можно максимальной ширину сделать 1920, а минимальной 320, а между этими значениями подстраиваться под ширину страницы.
* Ставить в приоритет использование современных способов создания сеток, таких как flexbox и grid.
* Не использовать фреймворки для создания раскладки страницы, такие как, например, bootstrap. Это, с одной стороны, важно для нашего понимания того, что вы владеете техниками создания раскладки страницы, а с другой, будет полезно вам, так как поможет углубить ваши знания в html и css, и, также, научит решать боевые задачи связанные с созданием раскладки.
* Компонентность. В стандартах будет требоваться использование БЭМ, так что предлагаем сразу его использовать. Необходимо настроить Parcel или Webpack и шаблоны, чтобы каждый БЭМ-овский блок находился в отдельной папке (там будет шаблон самого блока и все его стили, скрипты и картинки.
     Затем в index.pug вы будете просто подключать самые верхние блоки, а они уже будут внутри себя импортировать вложенные блоки, где надо.
     Каждый отдельный элемент лучше делать отдельным БЭМ-блоком. Мы сделали небольшой туториал по компонентной архитектуре, где вы можете понять основные принципы.
* Использовать в макетах препроцессоры по максимуму. Вам в любом случае надо будет это сделать для соблюдения предыдущего требования про компонентность, импорты и вставки компонентов друг в друга вы на сыром HTML не сделаете.  Подключайте Parcel (или Webpack), он же нужен будет для 4-го задания, и через него настройте сборку Pug (замену HTML) и SCSS (замена CSS). Конкретно эти технологии просто рекомендации, можете использовать другие препроцессоры, главное, чтобы они позволяли вам сделать вкладываемые компоненты с чёткими контрактами.
* Небольшие расхождения в PerfectPixel допускаются в местах, где есть неточности в макете (пример: разная ширина у одинаковых блоков).
* Макет был подобран так, чтобы вы явно почувствовали типичную проблему верстки — когда есть несколько (от 3-х до 100) страниц верстки, в которых используются часто похожие (совсем похожие или с небольшими отличиями) блоки.
* UI-Kit — это единый макет дизайна и единая страница верстки, с которой берут типовые блоки и используют в конечных страницах
* На страницах UI-Kit responsive не требуется.
* В этом задании вам нужно сверстать все элементы из макета, разбив на компоненты. То есть прямо по макету накидать на одной странице все компоненты.
* Сделать отдельно сами страницы проекта по поиску номеров в отеле, где эти блоки будут использоваться. Обратите внимание, что некоторые блоки будут в немного измененных модификациях (в разных местах будут разный цвет, разные масштабы или еще что-то подобное).
* Так же такие вещи, как бегунки, календари и дропдауны должны быть сделаны через JS. можете подключать какие угодно jQuery-плагины для этого (вообще ради этого макет и подбирался, чтобы был опыт экспериментов с подключением jQuery и его плагинов)
* Проект можно сразу реализовывать с учетом наших СТАНДАРТОВ разработки. Именно на соответствие этим стандартам будет проводиться ревью проекта. Ссылка на стандарты (best practices).

Если есть вопросы по разработке, спрашивайте в чате задания, в Figma задавать вопросы нет смысла, потому что комменты в первую очередь видит дизайнер, а ответов у него нет.

Задание вам даст
* Понимание, как верстать большие макеты с большим количеством одинаковых элементов.
* Навыки проектировать компонентную архитектуру, где каждый блок можно переиспользовать.
* Работу с препроцессорами Pug и SCSS.
* Базовые знания БЭМ.
* Навыки отзывчивой вёрстки.
* Самые базовые навыки работы с JavaScript.
* Базовые знания систем сборок Parcel или WebPack по выбору.
* Умение подключать и настраивать шрифты так, чтобы они корректно отображались в разных браузерах.
* Умение искать, подключать и настраивать JavaScript-библиотеки и jQuery-плагины в частности.
* Навыки работы с макетами в Figma
