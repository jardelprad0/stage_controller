# stage_controller
Este arquivo fornece instruções sobre como executar o código no seu ambiente local.

## Pré-requisitos
- Linguagem de programação: [Python 3]
- Versão Ubuntu: [20.04]
- Versão do ROS: [Noetic]

## Comandos para executar o programa 
### Preparando ambiente do ROS
1. Em um terminal, navegue até o repositório catkin_ws:

```sheel
$ cd catkin_ws/
```
2. Inicialize e configure o ambiente:

```sheel
~/catkin_ws$ source devel/setup.bash 
```
3. Compile os pacotes baixados (execute esse comando somente quando baixar um novo pacote, não é necessário executá-lo toda vez que executar a simulação):
```sheel
~/catkin_ws$ catkin_make
```
### Tornando o arquivo executável
4. Navegue até a pasta /scripts, executando o seguinte comando:

```sheel
~/catkin_ws$ cd src/stage_controller/scripts/
```
5. Em seguida, execute o comando para tornar o arquivo stage_controller.py executável:

```sheel
~/src/stage_controller/scripts/$ chmod +x stage_controller.py
```
### Executando a simulação
6. Inicialize o ROS:

```sheel
~/catkin_ws$ roscore
```
7. Em outro terminal, sem fechar o primeiro, execute os comandos 1 e 2 para carregar o ambiente e, em seguida, execute o seguinte comando para abrir a janela de simulação:

```sheel
~/catkin_ws$ roslaunch stage_controller launcher.launch
```
Assim, a seguinte janela será aberta:



![Captura da tela Stage](https://github.com/jardelprad0/stage_controller/assets/61805544/6bb63beb-8d87-40d5-b465-5792dfd39e88)

8. Com isso feito, abra outro terminal e execute os comandos 1 e 2. Em seguida, execute o seguinte comando para fazer o robô se movimentar:

```sheel
~/catkin_ws$ rosrun stage_controller stage_controller.py
```

## Pronto! Seu robô está se movendo em direção ao 'target' definido no código :)


![giphy (2)](https://github.com/jardelprad0/stage_controller/assets/61805544/12fc5000-2f72-42f2-b40b-02eaf1cff4c1)



### Link do Vídeo  : https://youtu.be/XEvFqXbvWAI
