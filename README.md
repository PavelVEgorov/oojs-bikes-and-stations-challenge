## OOJS:  Велосипеды и станции

В некоторых городах велосипеды можно арендовать на короткое время. [Станции велопроката](https://www.google.com/search?q=bike+rental+stations&espv=2&biw=1366&bih=647&tbm=isch&tbo=u&source=univ&sa=X&ved=0ahUKEwjhuaOwsf3LAhUFOiYKHQOZCkwQsAQIGw) расположены в разных частях города. Люди могут арендовать велосипед на одной из станций, поехать на нем туда, куда им нужно, и вернуть велосипед на другой станции. Тебе нужно будет разработать объекты на JavaScript для моделирования велосипедов и станций.


### Release 0. Разработка на основе предложенных технических характеристик

У велосипеда должен быть индетификационный номер, цвет и год выпуска. (Cоответственно, поля класса должны иметь имена: id, color, modelYear. Такой нейминг необходим для прохождения unit тестов.)

Станция должна иметь название, местоположение, год открытия и велосипеды, которые в данный момент находятся на станции.
(поля класса: name, location, openingYear, bikes)

Также тебе надо будет написать несколько методов класса:
- Нужно иметь возможность вывести самый новый велосипед на станции
- Проверить, есть ли на станции велосипеды
- Станция должна позволять взять велосипеды в прокат (выдать один велосипед) и сдать велосипеды обратно на станцию (как один, так и несколько). Подумай, что будет в этот момент происходить с массивом велосипедов на станции.

Предложенные тесты описывают как велосипеды, так и станции. Чтобы запустить тесты, открой в браузере файл `SpecRunner.html`.  Напиши код, позволяющий пройти тесты. Используй функции конструктора, чтобы назначить уникальные свойства каждому экземпляру велосипеда или станции. 

Заверши модель велосипеда, прежде чем приступать к модели станции.

### Release 1. Вместимость станции
В своем нынешнем виде наши станции продолжат принимать велосипеды независимо от того, сколько велосипедов в них уже стоит. Сделай свою модель более точной, наделив каждую станцию характеристикой вместимости. Например, на одной станции могут стоять 30 велосипедов, а на другой – 10. Поставить велосипед на станцию можно будет, только если она ещё не заполнена. Рассмотри пограничный случай: что произойдет, если группа попытается вернуть одновременно пять велосипедов, но на станции будут места только для двух?

Напиши тесты, которые будут описывать это новое поведение.

### Release 2. Велосипеды с поломками
Твои модели велосипедов всегда находятся в прекрасном рабочем состоянии. В реальности у велосипедов могут быть поломки: спущенные шины, порванные цепи и т.д. Дополни модель велосипеда так, чтобы велосипед мог иметь множественные поломки. Пользователь должен иметь возможность добавить поломки к велосипеду, а затем починить его. Велосипед также должен сообщать, сломан он или нет.

Далее нужно доработать объекты станций таким образом, чтобы они могли учитывать сломанные велосипеды. Например, станция не должна выдавать сломанные велосипеды. Она должна уметь сообщать, какое количество велосипедов, стоящих на ней, сломано. Как ещё сломанные велосипеды могут повлиять на станцию?

Напиши тесты, которые будут описывать это новое поведение.


Ты должен(на) чувствовать себя всё более и более уверенно при работе с функциями и классами. Обратись к преподавателю, если тебе сложно понять эти инструкции с теоретической точки зрения или если у тебя не получается использовать их при написании кода.

[изображение станции]: https://www.google.com/search?q=bike+rental+stations&espv=2&biw=1366&bih=647&tbm=isch&tbo=u&source=univ&sa=X&ved=0ahUKEwjhuaOwsf3LAhUFOiYKHQOZCkwQsAQIGw
[Error]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Error

