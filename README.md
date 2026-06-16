# Лабораторная работа 4

Выполнила: Гафурова Н.А

Группа: ЦИБ-251

**№ 6**


Условие:

# Сравнение хешей

Функция check_integrity(data_str, given_hash) возвращает True, если MD5 от data_str совпадает с given_hash.

Шаблон:
def check_integrity(data_str: str, given_hash: str) -> bool:
pass

Тесты:

 Input: admin|21232f297a57a5a743894a0e4a801fc3 -> Output: True

 Input: user|21232f297a57a5a743894a0e4a801fc3 -> Output: False

 # Описание работы
Функция check_integrity выполняет ровно три действия:
1) Преобразует строку data_str в байты (UTF-8).
2) Вычисляет её MD5-хэш и переводит в шестнадцатеричный вид через .hexdigest().
3) Сравнивает полученную строку с given_hash и возвращает True при совпадении, иначе False.
