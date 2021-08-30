### Importante: para rodar a rotina *api_ERA5.ipynb* é necessário ter o CDS API instalado

*PASSOS PARA INSTALAR O CDS API*

>**1. Cadastro**

Fazer o cadastro no site da [Climate Data Store](https://cds.climate.copernicus.eu/#!/home)

>**2. Adicionar a chave e instalar o pacote CDS API no Python**

Este [LINK](https://cds.climate.copernicus.eu/api-how-to#install-the-cds-api-key) mostra como adicionar a chave e como realizar a instalação do biblioteca CDS API no Python.

A instalação do pacote pode ser feito pelo gerenciador de pacotes PIP ou CONDA\
*ex: pip install cdsapi\
ou\
conda install cdsapi*

***Caso encontrem dificuldades em instalar o CDS API, o vídeo no link a seguir mostra o passo a passo detalhado.***
[VÍDEO](https://www.youtube.com/watch?v=NHbvfggMC10&ab_channel=CopernicusECMWF)

<hr style="border:1px solid lightblue"> </hr>

Os dados adquiridos do ERA5 são do [ERA5 hourly data on single levels from 1979 to present](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-single-levels?tab=overview). Para adquirir dados com níveis de pressão específicos [(ERA5 hourly data on pressure levels from 1979 to present)](https://cds.climate.copernicus.eu/cdsapp#!/dataset/reanalysis-era5-pressure-levels?tab=overview) é preciso inserir a variável e os níveis de pressão de interesse ``'pressure_level': ['825','850',....]`` e trocar a variável ``'reanalysis-era5-single-levels'`` pela ``'reanalysis-era5-pressure-levels'``

* *A rotina estar configurada para realizar aquisição dos dados horários (resolução temporal de 1h) do ERA5 para todos os dias e meses para o intervalo de tempo desejado. O arquivo de saída da rotina será um .nc com médias diárias.* 

* *A única alteração que deve ser feita pelo usuário é determinar os diretórios para os arquivos de saída.*

* *Os parâmetros **latitude, longitude e intervalo de tempo** serão pedidos pela própria rotina quando executada.*  


<hr style="border:1px solid lightblue"> </hr>

**Bibliotecas usadas**

* CDO
* numpy
* pandas
* xarray
* cdsapi
* os
* glob
