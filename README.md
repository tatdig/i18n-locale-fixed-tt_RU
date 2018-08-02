где? На центос это папка /usr/share/i18n/locales/

что? Имя файла выбрано уникальным для предотвращения перезаписи при обновлениях. Исправлены имена дней недели. "tt_RU@az"

как? Скопировать файл "tt_RU@az" в вышеуказанную папку. Выполнить из терминала: localedef -i tt_RU@az -f UTF-8 en_US@az.UTF-8 .
Моҗно использовать например в PHP: 
if(!setlocale(LC_TIME, 'tt_RU.utf8@az.UTF-8')) error_log("Locale not found in ".__FILE__." at ".__LINE__);
