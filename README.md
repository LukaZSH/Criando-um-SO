# Criando-um-SO
Passo a passo da criação de um Sistema Operacional.

Neste repositório será documentado todo o passo a passo da criação de um SO simples. As ferramentas que serão utlizadas para a criação são:
- Nasm(Netwide Assembler): O Nasm é um software focado para criar projetos em arquiteturas de CPUs x86, utilizando a linguagem de baixo nível Assembly.
- Rufus: Software amplamente utilizado para carregar imagens/.iso de SO em um pendrive para torná-lo bootável.
- Fergo Raw Image Maker: Este software cria um arquivo de imagem de dados brutos para usar em pendrives, HDs, etc. Onde pode ser definido o cilindro, a trilha e o setor a serem usados ​​e adiciona qualquer arquivo que desejar.

<h4> :x: Problemas atuais :x: </h4>
Nos sistemas Windows, especificamente no Windows 10 e 11, quando tenta executar o Fergo Raw, acontece um erro de dependência do Windows necessitando do arquivo "MSCOMCTL.OCX", porém mesmo baixando o arquivo manualmente e direcionando-o para uma pasta na raíz do Windows 10 e reiniciando o computador, o Fergo Raw continua dando erro de dependência.
Aparentemente, no Windows 7 o Fergo Raw executa normalmente sem erro de dependência, posteriormente irei testar em uma Máquina Virtual e dar proseguimento no projeto através do Windows 7 na VM.
