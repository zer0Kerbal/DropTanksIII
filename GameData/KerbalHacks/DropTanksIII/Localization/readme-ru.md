---
permalink: /readme-ru.html
title: Иструкция по переводу и локализации
---
<!-- readme-ru.md v1.0.1.0
Localization project
created: 04 Jun 2023
updated: 04 Jun 2023

THIS FILE:
    CC BY-ND-4.0
    by [zer0Kerbal](https://gitbug.com/zer0Kerbal)
    Переведено/translated by [evanisrael](https://github.com/evanisrael)
-->

# Перевод на ваш язык

![Языки поддерживаемые в KSP 1.3: Английский, Испанский, Китайский, Русский, Японский](https://i.imgur.com/DbCCJWK.png)

В версии KSP 1.3 появилась локализация, которая позволяет переводить текст в игре на другие языки. Блягодаря этому большее число людей сможет наслаждаться игрой на предпочитаемом ими языке и сообщество игроков будет только расширяться. Однако, для модов этот процесс не автоматизирован; по умолчанию, мод будет на английском языке, независимо от языка основного клиента игры. Чтобы и основной клиент и моды были доступны на одном языке, при этом отличном от английского, создателю мода нужно проделать дополнительную работу.

К сожалению, я говорю только на английском, и я разрабатываю и поддерживаю этот мод бесплатно. ПОэтому я не могу заниматься переводами самостоятельно и не имею возможности заплатить  переводчикам за профессиональный перевод. Лучшее что я могу сделать самостоятельно - это использовать Google Переводчик, который не очень хорошо справляется с краткими и идиоматическими фразами, необходимыми в пользовательском интерфейсе мода KSP. Вместо этого, я мне придется полагаться на ваш, многоязычного члена сообщества KSP, профессионализм, чтобы вы показали мне как выглядят по настоящему хорошие переводы. Если вы хотите помочь в этом деле, пожалуйста, подробно изучите этот файл до конца, чтобы узнать, как устроены языковые файлы мода и как подготовить переводы для использования другими игроками.

Примечание: Несмотря на то что вы редактируете файлы проекта, не бойтесь ошибиться. GitHub сохранит ваши изменения отдельно от основных файлов до тех пор, пока я не проверю их и не подтвержу, что все в норме. Я даже смогу, в случае чего, задавать вам вопросы или просить внести изменения, прежде чем ваша работа будет добавлена в основной код.

## Языки

* Поддерживаемые Kerbal Space Program на момент версии 1.12.x
  * ![Английский][EN] Английский <en-us.cfg>
  * ![Бразильский][BR] Бразильский <pt-br.cfg>
  * ![Китайский][CN] Упрощенный китайский (中文) <zh-cn.cfg>
  * ![Немецкий][DE] Немецкий (Deutsch) <de.cfg>
  * ![Испанский][ES] Испанский (Español) <es-es.cfg>
  * ![Французский][FR] Французский (Français)<fr-fr.cfg>
  * ![Итальянский][IT] Итальянский (Italiano) <it-it.cfg>
  * ![Японский][JA] Японский (日本語) <ja.cfg>
* Included as well
  * ![Корейский][KO] Корейский (한국어) <ko.cfg>
  * ![Мексиканский испанский][MX] Мексиканский испанский (Español Mexicano) <es-mx.cfg>
  * ![Голландский][NL] Голландский <nl-nl.cfg>
  * ![Норвежский][NO] Норвежский (Norsk) <no-no.cfg>
  * ![Польский][PO] Польский (Polski) <pl.cfg>
  * ![Русский][RU] Русский (Русский) <ru.cfg>
  * ![Шведский][SW] Шведский (Svenska) <sw-sw.cfg>
  * ![Тайваньский][TW] Тайваньский (国语) <zh-tw.cfg>

## Создание или редактирование перевода

Рекомендуется вносить изменения сначала локально на вашем устройстве, чтобы вы могли их протестировать перед отправкой. Особенно если вы создаете новый перевод с нуля.

1. Установите последнюю версию xxx мода, если еще этого не сделали.
2. Откройте папку <KSP_ROOT>/GameData/xxxMod/Localization на вашем локальном диске.
3. Найдите файл с названием *lang*.cfg, где *lang* - это название языка в KSP; начиная с KSP 1.3, в него входят:

* en-us (английский)
* es-es (испанский)
* ja (японский)
* ru (русский)
* zh-cn (китайский)

Дальнейшие действия зависят от того, существует ли файл:

### Если файл существует

Чтобы внести улучшения в существующий перевод, выполните следующие действия:

4. Откройте файл вашего языка в выбранном вами текстовом редакторе.
5. Внесите изменения которые хотели бы видеть в игре (подробнее в разделе [Формат файла](#file-format) ниже)
6. Сохраните ваши изменения
7. Не забудьте [их протестировать](#testing)!

### Если файл не существует

Чтобы создать свой собственный перевод с нуля, выполните следующие действия:

4. Сделайте копию файла `en-us.cfg` в папке `Localization`.
5. Переименуйте файл в соответствии со списком языков выше.
6. Откройте файл вашего языка в выбранном вами текстовом редакторе.
7. Замените третью строку с `en-us` на название вашего языка (подробнее в разделе [Языки](#Languages))
8. Переведите каждую строку с английского на ваш язык (подробнее в разделе [Формат файла](#file-format) ниже)
9. Сохраните внесенные изменения
10. Не забудьте [их протестировать](#testing)!

### Формат файла

Центральная часть файла `cfg` содержит строки, которые нужно перевести. Формат записи выглядит так: `имя = перевод`, где имя - это особая строка, определенная модом. Например:

    #launchSubtitle = Transfers from <<1>>\n(Launch ~<<2>>)

**Не нужно** изменять часть слева от знака равенства ("=")! Эта часть должна быть одинаковой во всех файлах с переводами.

Часть справа от знака равенства - это строка, которая будет использоваться в игре. Большая часть текста будет отображаться как есть, но он может содержать несколько особых строк, как показано в [демонстрационном грамматическом модуле Lingoona](http://lingoona.com/cgi-bin/grammar#l=en&oh=1):

| Строка  | Назначение                                                                                                                 |
| ------- | -------------------------------------------------------------------------------------------------------------------------- |
| \n      | Перенос строки; старайтесь сохранить их исходя из исходных строк, чтобы убедиться, что все строки поместятся               |
| <<1>>   | Первый подставляемый токен в строке, который будет заменен на число, название планеты и т.д., в зависимости от строки      |
| <<2>>   | Второй токен и так далее                                                                                                   |
| <<A:1>> | Первый токен, но замененный правильным значением                                                                           |

Например, вот так может выглядеть перевод строки, указанной выше, на испанский, выполненный через Google Переводчик:

    #launchSubtitle = Transferencias desde <<1>>\n(Lanzamiento ~<<2>>)

### Тестирование

Очень важно убедиться что ваши изменения работают корректно. Если вы используете Steam:

1. [Выберите язык для использования в Steam](https://www.youtube.com/watch?v=iBwYCvQxfeI)
2. Дождитесь полной загрузки языкового пакета
3. Запустите KSP
4. Активируйте xxxMod в игре и убедитесь что ваши изменения работают так, как вы задумывали

Если вы не пользуетесь Steam, я не знаю какие шаги необходимо предпринять для смены языка. Свяжитесь со SQUAD если не сможете разобраться самостоятельно.

## Публикация перевода в общий доступ

После того как вы подготовили `cfg` файл для вашего языка и убедились что все работает как нужно, если вы хотите предоставить его для переиспользования под xxxModd's лицензией - следуйте следующим шагам чтобы загрузить перевод в основной репозиторий:

1. Войдите в свою учетную запись [GitHub](https://github.com); Вам нужно будет зарегистрировать новый аккаунт если вы заходите туда впервые.
2. Перейдите в папку Localization внутри xxxMod 
3. Найдите файл над которым вы работали

Дальнейшие действия зависят от того, существует ли файл:

### Если файл существует

4. Нажмите на название файла чтобы посмотреть его
5. Нажмите на [иконку карандаша](https://help.github.com/assets/images/help/repository/edit-file-edit-button.png) для внесения изменений
6. Замените текст на отредактированный вами локально
7. **Важно**: Внизу страницы, под кнопкой Propose file change, напишите краткое описание своий изменений на английском языке, что именно изменено и почему вы считаете эти правки необходимыми. Это поможет мне понять что правки действительно следует внести. Помните, что я не говорю на языке текста в `cfg` файле, поэтому мне нужно чтобы вы объяснили мне почему ваш вариант лучший!
6. Нажмите на кнопку `Propose file change` внизу страницы, когда вы закончите

### Если файл не существует

4. Нажмите на кнопку [Create new file](https://help.github.com/assets/images/help/repository/create_new_file.png) для создания нового файла
5. Введите корректное название файла в поле сверху
6. Вставьте отредактированный вами локально текст в большое поле посередине страницы
8. Нажмите на кнопку `Propose file change` внизу страницы, когда вы закончите

### Ревью

Как только вы внесете изменения, GitHub пришлет мне уведомление о том, что появился новый пул реквест. Я обязательно взгляну на него в течении суток или двух и попробую определить валидность правок следующими методами:

* Убеждаясь что название файла и третья строка в нем совпадают с кодом выбранного языка
* Просмотрев все измененные строки в игре
* Проверив перевод через Google Переводчик
* Спросив нескольких знакомых экспертов
* Запросив помощь на форуме KSP

Если у меня будут какие-нибдь вопросы касательно конкретных изменений которые вы внесли, я добавлю их в пул реквест, вам должно будет придти уведомление об этом. Пожалуйста, постарайтесь отвечать на эти вопросы как можно оперативнее, насколько вам позволяет ваше время. Ваш пул реквест может быть закрыт без утверждения и добавления ваших правок в основной репозиторий если от вас слишком долго не будет ответа.

Как только я буду полностью удовлетворен решениями всех возникших вопросов, ваши правки будут добавлены в основной репозиторий и будут включены в следующий релиз. Также, я добавлю ваш никнейм на Github в секцию Acknowledgements в файле README.

[EN]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/EN.png "English"  
[BR]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/BR.png "Português Brasil"
[CN]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/CH.png "中文"  
[DE]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/DE.png "Deutsch"  
[ES]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/ES.png "Español"  
[FR]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/FR.png "Français"  
[IT]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/IT.png "Italiano"  
[JA]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/JA.png "日本語"  
[KO]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/KO.png "한국어"  
[MX]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/MX.png "Mexicano Español"  
[NL]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/NL.png "Dutch"  
[NO]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/NO.png "Norsk"
[PO]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/PO.png "Polski"  
[RU]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/RU.png "Русский"  
[SW]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/SW.png "Svenska"  
[TW]: https://raw.githubusercontent.com/zer0Kerbal/zer0Kerbal/zed'K/img/TW.png "国语"