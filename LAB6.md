ЗВІТ до лабораторної роботи №6

Тема: “Команди Linux для архівування та стиснення даних. Робота з текстом”

Мета роботи: 
Отримання практичних навиків роботи з командною оболонкою Bash.
Знайомство з базовими командами для архівування та стиснення даних.
Знайомство з базовими діями при роботі з текстом у терміналі.

Словник англійських термінів (English Terms Dictionary)
Compression: A method of reducing the size of a file on disk using algorithms and mathematical calculations.   
Archival (Archive): A file format that creates a convenient way to distribute, store, back up, and manipulate groups of related files (historically tape archives, commonly .tar).   
Lossless Compression: A compression method that creates a file smaller than the original that can be used to reconstruct the original file without losing data.   
Lossy Compression: A compression method that permanently discards unimportant or redundant data from the original file (e.g., MP3, JPEG).   
Standard Output (stdout): The default destination where a command writes its output data stream.
Standard Error (stderr): The default channel where a command writes error messages or diagnostics.
Pipeline (Pipe): A mechanism (|) that connects the standard output of one command directly to the standard input of another.
Redirection: Directing data streams from or to files instead of standard input/output devices.

1.Завдання для попередньої підготовки:

Питання 1: Призначення та параметри команд tar, xz, zip, bzip, gziptar: 
Призначена для об'єднання кількох файлів та каталогів в один архівний файл зі збереженням структури каталогів, прав доступу та метаданих.   Основні параметри: -c (створення архіву), -x (витягнення архіву), -t (перегляд вмісту), -f (вказівка файлу), -v (детальний вивід), -z (стиснення gzip), -j (стиснення bzip2), -J (стиснення xz).gzip: Класичний інструмент стиснення даних у Linux на основі алгоритму DEFLATE.   Основні параметри: -d (декомпресія), -l (виведення статистики), -c (виведення в стандартний потік), -1…-9 (рівні стиснення від швидкого до максимального).bzip2: Інструмент стиснення на основі алгоритму Барроуза-Вілера (Burrows-Wheeler), що забезпечує краще стиснення порівняно з gzip за рахунок більшого часу та ресурсів пам'яті.   Основні параметри: -d (декомпресія), -s (зниження вимог до пам'яті).xz: Сучасний інструмент стиснення на основі алгоритму LZMA2, що забезпечує найвищий коефіцієнт стиснення (найменший розмір файлу), але потребує найбільше часу та пам'яті.   Основні параметри: -d (декомпресія), -l (статистика), -e (екстремальний режим стиснення), -0…-9 (ступінь стиснення).zip: Популярна програма для архівування та стиснення файлів у форматах, сумісних з різними ОС (особливо Windows), яка об'єднує функції архівування та стиснення в одному файлі з розширенням .zip.

Питання 2: 
Приклади реалізації архівування та стискання даних різними командамиСтворення tar-архіву, стисненого за допомогою gzip:tar czvf archive.tar.gz directory1   Створення архіву, стисненого за допомогою bzip2:tar cjvf archive.tar.bz2 directory2   Створення архіву, стисненого за допомогою xz:tar cJvf archive.tar.xz directory3   

Питання 3: 
Призначення та параметри команд cat, less, more, head, tailcat: Виводить вміст файлів на стандартний пристрій виведення (або об'єднує кілька файлів).less: Посторінковий перегляд вмісту текстових файлів із можливістю прокручування назад та вперед.more: Посторінковий перегляд вмісту текстових файлів (лише прокручування вперед).head: Виводить перші рядки файлу (за замовчуванням — перші 10).tail: Виводить останні рядки файлу (за замовчуванням — останні 10).

Питання 4:
Принципи роботи командної оболонки з каналами, потоками та фільтрамиКомандна оболонка Bash використовує стандартні потоки: стандартне введені (stdin, дескриптор 0), стандартне виведення (stdout, дескриптор 1) та стандартні помилки (stderr, дескриптор 2). За допомогою каналів (|) вихід одного процесу передається на вхід іншого. Фільтри — це команди, які зчитують дані з stdin, обробляють їх та передають у stdout (наприклад, grep, sort, wc).

Питання 5:
Призначення команди grepКоманда grep призначена для пошуку рядків, що відповідають заданому шаблону (регулярному виразу) у текстових файлах або у вхідному потоці даних.

2.Хід роботи

3.Відповіді на запитання

4.Conclusions
