Тип | Описание | Объявление типа | Пример типа
------------ | ------------------- | --------------- | -------------
Список | Последовательность переменной длины, состоящая из элементов одного типа. | `List<Type>` | `List<Int32>`
Словарь | Набор пар ключ-значение с указанными типами для ключа и значения. | `Dict<KeyType, ValueType>` | `Dict<String, Int32>`
Кортеж | Набор безымянных элементов фиксированной длины с указанными типами всех элементов. | `Tuple<Type1, ..., TypeN>` | `Tuple<Int32, Double>`
Структура | Набор именованных полей с указанными типами значений, фиксированный на момент начала запроса и не зависящий от данных. | `Struct<Name1:Type1, ..., NameN:TypeN>` | `Struct<Name:String, Age:Int32>`
Поток | Однопроходной итератор по значениям одного типа. Не является сериализуемым. | `Stream<Type>` | `Stream<Int32>`
Вариант над кортежем | Кортеж, про который известно, что заполнен ровно один элемент. | `Variant<Type1, Type2>` | `Variant<Int32, String>`
Вариант над структурой | Структура, про которую известно, что заполнен ровно один элемент. | `Variant<Name1:Type1, Name2:Type2>` | `Variant<value:Int32, error:String>`