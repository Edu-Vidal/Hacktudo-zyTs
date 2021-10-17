# CNPJ-SQLITE
Script em python para carregar os arquivos de cnpj dos dados públicos da Receita Federal em formato sqlite.

## Dados públicos de cnpj no site da Receita:
A partir de 2021 os dados da Receita Federal estão disponíveis no link https://www.gov.br/receitafederal/pt-br/assuntos/orientacao-tributaria/cadastros/consultas/dados-publicos-cnpj (ou http://200.152.38.155/CNPJ/) em formato csv zipado. 

## Pré-requisitos:
Python 3.8;<br>
Bibliotecas pandas, dask e sqlalchemy.<br>

## Utilizando o script:
Baixe todos os arquivos zipados do site da Receita e salve na pasta "dados-publicos-zip".<br>
Crie uma pasta com o nome "dados-publicos".<br>

Para iniciar esse script, em um console DOS digite<br>
python dados_cnpj_para_sqlite.py<br>

A execução durou no meu notebook cerca de 2hs.

Ao final, será gerado um arquivo cnpj.db, no formato sqlite, que pode ser aberto no DB Browser for SQLITE (https://sqlitebrowser.org/).<br>

O arquivo cnpj.db poderá ser usado no projeto [dados-cnpj](https://github.com/rictom/rede-cnpj) que está localiazado no (diretório acima)[https://github.com/Edu-Vidal/Hacktudo-zyTs/tree/master/DadosReceitaFederal].<br>

## Arquivo sqlite já tratado:
Arquivo sqlite, referência 11/09/2021, está disponível no google drive, zipado em 4 pedaços:
https://drive.google.com/drive/folders/1Gkeq27aHv6UgT8m30fc4hZWMPqdhEHWr?usp=sharing <br>
Utilize o 7-zip para descompactar.<br>

## Histórico de versões

versão 0.1 (julho/2021)
- primeira versão

