# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?
#### Ответ: файл находится по пути group_vars/all/examp.yml
![image](https://user-images.githubusercontent.com/92969676/163532921-33c90c0c-74e9-400d-bb17-271f17bfb57a.png)

3. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?

#### Ответ: ansible-playbook site.yml -i inventory/test.yml

![image](https://user-images.githubusercontent.com/92969676/163540835-6dbe5c16-eb61-499b-ad61-629ceb6ba742.png)


4. Какой командой можно зашифровать файл?
#### Ответ: например, вот так ansible-vault encrypt group_vars/deb/examp.yml

![image](https://user-images.githubusercontent.com/92969676/163550197-62efc03e-1920-4d00-ab3f-03bfe4a30b2f.png)

![image](https://user-images.githubusercontent.com/92969676/163550303-b28a04bf-a9bd-44f7-9ea8-d4f39eca7ba5.png)


5. Какой командой можно расшифровать файл?
#### Ответ: например вот так: ansible-vault decrypt group_vars/deb/examp.yml

![image](https://user-images.githubusercontent.com/92969676/163550419-e6a878ff-dd88-49eb-b9fe-f699aeaa1180.png)

![image](https://user-images.githubusercontent.com/92969676/163550450-05d03a9f-64e1-4a25-bc4e-fa3273e721d8.png)

6. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
#### Ответ: можно. В случае, когда файлы у нас зашифрованы:

![image](https://user-images.githubusercontent.com/92969676/163552130-7685a9d1-0557-440c-83fa-2b185fae88b8.png)

![image](https://user-images.githubusercontent.com/92969676/163552184-fce8bb71-8daa-4077-a4fb-3699e647ef4f.png)

То при запуске playbook мы увидим в процессе play какие именно данные у нас содержатся в данном файле: 

![image](https://user-images.githubusercontent.com/92969676/163553056-fa8e4369-bafc-4715-95a4-533ac21838a0.png)

![image](https://user-images.githubusercontent.com/92969676/163553187-6c45c54f-04f9-4806-9d12-abd2fc71f74a.png)

При этом мы не расшифровывали файл на операционной системе, Ansible сделал это внутри себя и выдал уже дешифрованные данные, которые дальше использовал.

7. Как выглядит команда запуска `playbook`, если переменные зашифрованы?
#### Ответ: команда выглядит вот так: ansible-playbook site.yml -i inventory/prod.yml --ask-vault-pass

![image](https://user-images.githubusercontent.com/92969676/163551317-99993b02-4817-4669-8e2f-55c845b091a0.png)

8. Как называется модуль подключения к host на windows?
#### Ответ:

9. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
#### Ответ:

10. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
#### Ответ:
