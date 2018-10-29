# Update-Passwork-ru-

**Инструкция по обновлению Пассворк**

**Репозиторий**  
Репозиторий находится по адресу:   
_http://passwork.download/_  
Проект:   
_http:// passwork.download/passwork/passwork_  
Логин и пароль предоставляются высылаются по почте.  
  
**Обновление**  
1. Сделайте копию папки с файлами Пассворка.   
В случае каких - либо проблем вы можете все откатить к вашей версии.   
Файлы располагаются в директории:  
Для Windows: _С: \inetpub\wwwroot\_  
Для Linux: _/var/www/_  
  
2. Скачайте Пассворк из репозитория  
  
Через Git (рекомендуемый способ)  
Если Passwork был установлен на ваш компьютер при помощи команды   
_git clone http:// passwork.download/passwork/passwork.git_ тогда,  
- зайдите в папку с репозиторием  
- откройте командную строку в папке Passwork  
- введите команду для извлечения репозитория:  
_git pull http:// passwork.download/passwork/passwork.git_   
  
Для методов b и c мы рекомендуем просто переименовать папку с Пассворком, а вместо нее создать новую, пустую.  
  
a. Через Git   
— убедитесь, что у вас установлен git   
— склонируйте репозиторий следующей консольной командой:    
_ git clone http:// passwork.download/passwork/passwork.git _   
— скопируйте файлы из репозитория в директорию Passwork  
  
b. Через скачивание ZIP архива   
— Авторизуйте через браузер в репозитории:   
_ http://passwork.download/ _  
— Перейдите в проект:   
_ http:// passwork.download/passwork/passwork _  
— Нажмите на кнопку «Скачать как архив»   
Автоматически будет скачена последняя стабильная версия проекта.    
  
3. Скопируйте из вашей старой версии Пассворка в новую следующие файлы:   
a.  
_ /app/keys/→/app/keys/ _  
(скопируйте все файлы)  
b.  
_ /app/config/reginfo.php→/app/keys/ _  
Таким образом, в папке /app/keys/ у вас будут файлы с лицензиями (.lic) и один файл reginfo.php  
  
4. В новой версии Пассворка по умолчанию нет конфигурационного файла.   
Вместо этого в репозитории находится пример конфигурационная файла.   
Найдите файл _/app/config/config.example.ini_ и сделайте его копию в _ /app/config/config.ini _  
(не рекомендуется удалять файл-пример config.example.ini)  
  
5. Сравните ваш новый файл конфигурации со старым, чтобы перенести все настройки:   
В вашей старой версии Пассворка найдите файл   
_ /app/config/config.ini _  
и перенести настройки в аналогичный файла новой версии.   
(Убедитесь, что вы перенесли ключи шифрования, а так же имя базы данных).  
  
**Обновление завершено.**
