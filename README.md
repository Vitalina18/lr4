# ipc-pipes

Программа xor создаёт два дочерних процесса, замещая в них стандартный вывод.
Один дочерний процесс выводит какие-либо данные для шифрации, а второй поставляет ключ.
Для получения данных, мы будем использовать программу cat, а для генерации ключа напишем программу gen.
В процессе работы, данные с обоих процессов будут поступать по каналам в xor и шифроваться (через побитовый оператор "^").