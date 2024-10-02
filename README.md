**Как запустить убунту с юпитером?**

1) git clone https://github.com/IMikhaylov2710/judocker
2) cd judocker 
3) docker build -t judocker:latest .
4)  *Если без вывода в терминал (detached):* \n
        run --name judocker -d -v dockerData:/usr/src/app/data -p 8888:8888 judocker \n
    *Если с выводом в терминал:* \n
        run --name judocker -v dockerData:/usr/src/app/data -p 8888:8888 judocker \n
5) чтобы увидеть токен - docker logs judocker

NB создается volume dockerData, папка ~/data ее повторяет