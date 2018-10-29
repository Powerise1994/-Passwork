## Update-Passwork-ru-

### **Инструкция по обновлению Пассворк**

### **Репозиторий**  
Репозиторий находится по адресу:   
`http://passwork.download/`  
Проект:   
`http:// passwork.download/passwork/passwork`  
Логин и пароль предоставляются высылаются по почте.  
  
### **Обновление**  
1. Сделайте копию папки с файлами Пассворка.   
В случае каких - либо проблем вы можете все откатить к вашей версии.   
Файлы располагаются в директории:  
Для Windows: `С: \inetpub\wwwroot\`   
Для Linux: `/var/www/`   
  
2. Скачайте Пассворк из репозитория  
  
Через Git (рекомендуемый способ)  
Если Passwork был установлен на ваш компьютер при помощи команды   
`git clone http:// passwork.download/passwork/passwork.git` тогда,  
— зайдите в папку с репозиторием  
— откройте командную строку в папке Passwork  
— введите команду для извлечения репозитория:  
`git pull http:// passwork.download/passwork/passwork.git`   
  
Для методов b и c мы рекомендуем просто переименовать папку с Пассворком, а вместо нее создать новую, пустую.  
  
a. Через Git   
— убедитесь, что у вас установлен git   
— склонируйте репозиторий следующей консольной командой:    
`git clone http:// passwork.download/passwork/passwork.git`   
— скопируйте файлы из репозитория в директорию Passwork  
  
b. Через скачивание ZIP архива   
— Авторизуйте через браузер в репозитории:   
`http://passwork.download/`  
— Перейдите в проект:   
`http:// passwork.download/passwork/passwork`  
— Нажмите на кнопку «Скачать как архив»   
Автоматически будет скачена последняя стабильная версия проекта.    
  
3. Скопируйте из вашей старой версии Пассворка в новую следующие файлы:   
a.  
`/app/keys/→/app/keys/`  
(скопируйте все файлы)  
b.  
`/app/config/reginfo.php→/app/keys/`  
Таким образом, в папке /app/keys/ у вас будут файлы с лицензиями (.lic) и один файл reginfo.php  
  
4. В новой версии Пассворка по умолчанию нет конфигурационного файла.   
Вместо этого в репозитории находится пример конфигурационная файла.   
Найдите файл `/app/config/config.example.ini` и сделайте его копию в `/app/config/config.ini`  
(не рекомендуется удалять файл-пример config.example.ini)  
  
5. Сравните ваш новый файл конфигурации со старым, чтобы перенести все настройки:   
В вашей старой версии Пассворка найдите файл   
`/app/config/config.ini`  
и перенести настройки в аналогичный файла новой версии.   
(Убедитесь, что вы перенесли ключи шифрования, а так же имя базы данных).  
  
### **Обновление завершено.**
