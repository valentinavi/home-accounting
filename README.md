
Используемые технологии:

final-form,
prop-types,
react,
react-dom,
react-final-form,
react-redux,
react-router-dom,
react-scripts,
reactstrap,
redux,
json-server (для запуска программы).

Описание

Это программа предназначена для ведения домашнего бюджета.  
Она считает доходы, расходы и накопления, которые разбиты 
по отдельным блокам. 

Для начала использования нужно ввести даты с какого по какое 
число будет вестись учет средств. После добавления даты, ее 
можно редактировать.

Далее можно добавлять пункты списка доходов, расходов и накоплений. 
На основе этих данных в блоке Сводная информация будет идти подсчет 
Текущего бюджета и Накоплений. В каждом блоке ведется подсчет 
итоговой суммы. 

Есть счетчик, который отображает сколько дней осталось до конца 
отчетного месяца. 

Пункты списка можно редактировать и удалять. 

В блоке накопления имеется прогресс бар, который считает накопленный процент.

Все данные хранятся в файле db.json.



Компоненты

Add-period – кнопка Добавить период.

Cards – здесь содержатся компоненты: Постоянные доходы, Не постоянные доходы, 
Расходы, Не постоянные расходы, Накопления.

Form-period — компонент формы предназначенный для добавления даты отчетного периода.

Form-bank — компонент формы, предназначенный для добавления накоплений в блок Накопления. 

Form-data — компонент формы предназначенный для добавления пунктов Доходов, 
Расходов и Накоплений.

Info — здесь выводится Сегодняшняя дата, Дата отчетного периода, Бюджет, 
Текущий бюджет и Накопления.

Page-period — компонент, который включает в себя компоненты Info,  
Regular-Income, Variable-Income, Optional-Expenses, Obligatory-Expenses, Piggy-Bank.

Progress-bar – вложен в компонент  Piggy-Bank и выводит  накопленный процент.

Timer – вложен в компонент Info и выводит количество дней до конца отчетного периода.