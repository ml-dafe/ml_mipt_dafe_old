# Курс "Машинное обучение" на ФАЛТ МФТИ

### Quick start
Should Change directory for mount inside docker by `cd` and run: 


If you want stop it just use `docker ps` and `docker stop`
## Tools 

### <img src='https://github.com/VlasovKirill/ml_mipt_dafe_minor/blob/master/pic/anaconda.png' height="20px" width="20px" align="top"> Вариант 1
- Установить [Anaconda](https://www.anaconda.com/distribution/)
- Написать в командной строке: `jupyter notebook`
- Открыть в браузере [http://localhost:8888](http://localhost:8888)
- Использовать по назначению

### <img src='https://github.com/VlasovKirill/ml_mipt_dafe_minor/blob/master/pic/docker.png' height="20px" width="20px" align="top"> Вариант 2
- Устанавливаем Docker с [официального сайта](https://www.docker.com/products/docker-desktop)
- Перейдите в терминале в директорию, где хотите запускать юпитер ноутбуки и используйте команду
```
docker run -d -p 4545:4545 -v $PWD:/home/user vlasoff/ml jupyter notebook 
``` 
- Заходим через браузер на [http://localhost:4545](http://localhost:4545)
- Использовать по назначению (Для остановки напишите в терминале`docker ps` and `docker stop`)
- Образ включает в себя:
  - Python 3.7
  - Julia 1.3.1 

> :warning: Unsecure! 
> Close port 4545 on your local machine while container is running  
