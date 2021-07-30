## Importante: para rodar a rotina *api_ERA5.ipynb* é necessário ter o CDS API instalado

*PASSOS PARA INSTALAR O CDS API*

>**1. Cadastro**

Fazer o cadastro no site da Climate Data Store https://cds.climate.copernicus.eu/#!/home

>**2. Adicionar a chave e instalando o pacote CDS API no Python**

No link https://cds.climate.copernicus.eu/api-how-to#install-the-cds-api-key mostra como adicionar a chave e como realizar a instalação do biblioteca CDS API no Python.

A instalação do pacote pode ser feito pelo gerenciador de pacotes PIP ou CONDA\
*ex: pip install cdsapi\
ou\
conda install cdsapi*

***Caso encontrem dificuldades em instalar o CDS API, o vídeo no link a seguir mostra o passo a passo detalhadamente.***
https://www.youtube.com/watch?v=NHbvfggMC10&ab_channel=CopernicusECMWF

<hr style="border:1px solid lightblue"> </hr>

* *A rotina estar configurada para realizar aquisição dos dados horários (a cada 1h) do ERA5, para todos os dias e meses do intervalo de tempo desejado.* 

* *A única alteração que deve ser feita pelo usuário é determinar os diretórios para os arquivos de saída.*

* *Os parâmetros **latitude, longitude e intervalo de tempo** serão pedidos pela própria rotina quando executada.*  
