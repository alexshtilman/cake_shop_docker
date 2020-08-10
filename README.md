# docker basic comands
1. docker
   - version  версия докера
   - ps список запущенных контейнеров ( -a все включая остановленные)
   - images - список доступных образов
   - run
     - -p external:internal
     - -d запуск в фоне
     - --name <container_name>
     - -e env_name=env_val
     - --memory=<memory>
     - --cpu<.%number>
     - network=<network_name>
     - -i итерактивный режим для ввода данных из консоли
     - -it то же что и -i но с подключением к терминалу
     - -v <external_path>:<internal_path> подключение директорий
   - attach <container_id> подключится к выводу контейнера
   - stop <container_name>
   - rm <container_name>
   - pull <image_name:tag>
   - rmi <image_name:tag>
   - inspect <cont_name>
   - networks
     - inspect
     - ls
     - create
       - d
       - subnet
       - gateway
       - <network_name>
  - exec <container_name> command
  - logs <container_id> показывает логи
  
# DockerFile basic
   - build -t cont_name . - собирает докер контейенр по DockerFile
   - FROM <image_name:tag>
   - RUN <comand>
   - COPY <FROM> <TO>
   - ENTRYPOIN - первое что вызывается
   - CMD ["comand_1","comand_2"] 
