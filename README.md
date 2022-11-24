# CMOV_robot
Aplicação para testar o funcionamento do robô poppy (humanoid ou torso). Esta aplicação foi feita em python, por Leonardo Massuhiro Sato && Lucas Coimbra da Silva.
## Sobre
Esta aplicação tem como objetivo expressar os movimentos captados no aplicativo de captura de movimento, sendo reproduzidos por um robô poppy humanoid ou poppy torso.
## Recomendações e avisos
1. Utilize sempre a mesma entrada ao conectar os motores, ou robô
2. Lembre de conectar a fonte de alimentação no usb2ax
## Instruções para utilizar os testes .py
1. Clone o repositório
2. Descompacte o arquivo .zip "python-20221124T002403Z-001.zip"
3. Abra a pasta "python"
4. Abra o prompt de comando (cmd)
5. Execute a linha de comando "python setup.py install"
### Após isso, há duas opções:
1. Utilizar o software de teste Dynamixel Wizard 2.0
2. Utilizar a tabela de valores do modelo do motor servo específico
### Na primeira opção deve-se:
1. Instalar software no site [Dynamixel Wizard 2.0](https://emanual.robotis.com/docs/en/software/dynamixel/dynamixel_wizard2/)
2. Abra o software como administrador (para evitar erros)
3. Abra as configurações
4. Clique no botão scan </br>
![image](https://user-images.githubusercontent.com/73305733/203671572-69b0f8fe-dfa7-4cb0-ac9b-e3ecbdd97428.png)
5. Espere até o fim do escaneamento
6. Anote os valores de bauldrate, protocolo e entrada
7. Mude nas configurações o alvo de escaneamento para os valores específicos anotados (isso agiliza o processo de escaneamento futuro)
8. Anote as informações gerais do motor
9. Substitua no programa teste .py que se deseja rodar
### Na segunda opção:
1. Procure o modelo do motor desejado
2. Pesquise as informações necessárias (bauldrate, address, etc)
3. Substitua essas informações no programa .py </br>
Obs: Pode haver falta de informação na pesquisa, nesse caso é recomendado o uso da primeira opção
### Após a substituição das informações necessárias:
1. Clique duas vezes no arquivo que se deseje rodar ou execute o código para testar </br>
Obs: O código está incompleto e disfuncional
## Instruções para rodar o código da simulação V-Rep
1. Instale o simulador V-Rep [aqui](https://v-rep-pro-edu.software.informer.com/download/) 
2. Abra o cmd e coloque os seguintes comandos
- pip install pypot
- pip install poppy-humanoid
- pip install poppy-torso
- "*caminho do python*" -m pip install ipykernel -U --user --force-reinstall
3. Abra o Visual Studio Code
4. Instale as extensões:
- Python
- Jupyter
5. Abra o V-Rep
5. Abra a pasta com os códigos
6. Verifique a versão do python que está sendo utilizada
7. Caso esteja 3.9, mude para a 3.10
8. Execute a célula dos pacotes, apertando no botão executar célula </br>
![image](https://user-images.githubusercontent.com/73305733/203684823-85be3563-8c46-4c2a-8672-e02f90c2a4ca.png)
9. Execute a célula de instanciação do poppy
10. Clique em Ok no V-Rep
11. Execute a célula de tchau
### Personalização
O console de Jupyter permite que diversas personalizações sejam feitas, como por exemplo, é possível executar o programa em partes específicas de maneira desordenada, ou seja, o usuário pode executar uma célula no final do código em primeiro lugar. Além disso, essa ferramenta monstra de maneira nítida todos os erros do programa, permitindo solucionar o erro de maneira mais eficiente. Portanto, seja criativo e invente novas células de teste e se divirta com o robô poppy!!! A célula de tchau é somente o topo do iceberg desse mar de infinidades de movimentos.
