# ReviewPython
Данный скрипт работает в 4 режимах : 1) encode 2) decode 3) read 4) hack
1) Encode: Требует входного файла / ссылки(--input_file, --input_url) и выходного файла(--output_file), если нет входных данных, либо выходных - бросается исключение.
Указать можно параметры: --cipher - шифры цезаря, виженера, вернама (caesar, vigenere, vernam). Для шивров цезаря и виженера требуются ключи --key(число / строка), для вернама не указывается ключ, но укзаывается файл --random_file , в который будет записан текст шифратор. Так же указывается язык --language(eng, rus) по умолчанию язык английский. 
2) Decode: Обратная операция к Encode, такие же аргументы
3) Read: требуется указать --output_file и --input_file/--input_url. В этом режими скрипт считываем текст и запоимнает вероятности и слова из текста.
4) Hack: Взлом. Указать нужно --input_file --output_file, --AnalyzedDataFile - последний содержим данные о частотах букв и словах в нормальном тексте. Взлом определяет язык текста и взламывает его по цезарю, потом по виженеру(Индексы совпадений). Выбиарется лучший из исходов.