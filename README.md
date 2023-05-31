# SI_2023_lab2_206011

# Миа Јанева 206011

1. Code
2. Control Flow Graph

![controlflowgraph](https://github.com/miajaneva/SI_2023_lab2_206011/assets/73714277/a897d113-cdde-4eae-b26d-73aafb60b283)

3. Цикломатска комплексност

Цикломатската комплексност на овој код се пресметува со следнава формула:

V(G) = E - N + 2 каде:

V(G) е цикломатска комплексност
E е бројот на рабовите
N е бројот на јазли


E = 33
N = 24
=> 33-24+2=11

Цикломатската комплексност на овој код е 11.




4. Тест случаи според критериумот Every branch

=>1. throw new RuntimeException, пример ако user==null или password==null или email==null 

=>2. password.contains(" "), пример user = new User("softversko", "softversko 123", "softversko@gmail.com")

=>3. ист username и password, пример user = new User("softversko", "softversko", "softversko@gmail.com")

=>4. password нема празно место, нема специјален карактер

=>5. password содржи специјален карактер, user==null



5. Multiple condition

=>1. TXX, ако едното е точно пример user==null, не се важни другите user = null

=>2. FFT, ако user=softversko, password=softversko123, email=null user = new User("softversko", "softversko123", null)

=>3. FFF, ако сите полиња се исполнети user = new User("softversko", "softversko123", "softversko@gmail.com")

=>4. FTX, пример user=softversko, password=null, email може било што user = new User("softversko", null, )

