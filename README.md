# Тестовое задание для стажера на позицию "Программист на языке JS"

## [Текст задания](https://github.com/AVor0n/infoTech/blob/master/docs/task.md)

## [Результат](https://avor0n.github.io/infoTecs/)

## Заметки к выполнению

В задании не заданы целевые версии браузеров, так что я не оглядывался на совместимость и свободно использовал нововведения JS, например приватные поля и методы для инкапсуляции логики классов.

Работоспособность проверена в _Chrome_, _FireFox_ и _Opera_ последних версий.

Сменил расширение файла с исходными данными с `.json` на `.js`, чтобы добавить поддержку FireFox, так как в нем пока что не доступен `assert {type: 'json'}`. Если же файл с исходными данными нельзя было редактировать, то достаточно поменять 6 и 7 строчки в файле `initTable.js`, чтоб переключится на исходный json-файл.

Т.к. исходные данные на английском, интерфейс сделал также на английском, включая сортировку. Т.е. при сортировке по возрастанию сначала идёт латиница, затем кириллица. Регистр не учитывается.

Исходя из задания не ясно как сортировать поля eyeColor. По названию цвета или по hex-значению. Реализовал сортировку по названию цвета как более интересный вариант. При выборе цвета, его hex-код конвертируется в один из 147 предопределенных html цветов и уже название данного цвета записывается в таблицу.

Если к таблице была применена сортировка, то при изменении значения из этого столбца, оно останется на месте, даже если это нарушает порядок сортировки. Можно было конечно автоматически пересортировывать таблицу при внесении изменений, но показалось неудобным что после редактирования, строки будут улетать в неизвестность ведомые автосортировкой. Так что это 'не баг, а фича'

По условию задания обязательны комментарии, так что присутствует множество комментариев в стиле JSDoc.
Возможно даже слишком много 🙂
