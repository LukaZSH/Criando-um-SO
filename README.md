# Criando-um-mini-SO
Passo a passo da criação de um Sistema Operacional.
O SO foi feito seguindo o passo a passo do canal [KiddieOS Tutorial](https://www.youtube.com/watch?v=Jws7BHrts6g&list=PLsoiO2Be-2z8BfsSkspJfDiuKeC9-LSca&index=2) !!!

Neste repositório será documentado todo o passo a passo da criação de um SO simples. As ferramentas que serão utlizadas para a criação são:
- Nasm(Netwide Assembler): O Nasm é um software focado para criar projetos em arquiteturas de CPUs x86, utilizando a linguagem de baixo nível Assembly.
- Rufus: Software amplamente utilizado para carregar imagens/.iso de SO em um pendrive para torná-lo bootável.
- Fergo Raw Image Maker: Este software cria um arquivo de imagem de dados brutos para usar em pendrives, HDs, etc. Onde pode ser definido o cilindro, a trilha e o setor a serem usados ​​e adiciona qualquer arquivo que desejar.

<h2>Atualização sobre o Fergo RawImage Maker</h2>
Após ter feito o Download do arquivo "MSCOMCTL.OCX", movi o arquivo para a pasta C:\Windows\SysWOW64 e executei 2 comandos no CMD como administrador na pasta da DLL, "regsvr32 mscomctl.ocx" e "regsvr32 C:\Windows\SysWOW64\comdlg32.ocx", após ter feito esse passo a passo, o Fergo RawImage Maker executou normalmente!!

<h2>Como testar o SO</h2>

- Utilize o Nasm para converter os arquivos `.asm` para gerar arquivos os arquivos `.bin`
- Execute o arquivo Assembler.bat para gerar os arquivos `.bin`
- Para compilar os arquivos `.bin`, abra o FergoRaw.exe e adicione os 3 arquivos binários gerados pelo Nasm, na mesma ordem da imagem abaixo:


![FergoRaw](https://github.com/LukaZSH/Criando-um-SO/assets/49702498/2ef0bb6d-3707-49f0-b1c5-136f683e2ab9)

- Após gerar o arquivo `.img`, execute o Rufus para montar a imagem do SO em um pendrive
- Em seguida, basta testar numa máquina virtual ou em um computador físico, alterando a ordem de boot na BIOS

<h2>Implementações feitas até o momento no SO</h2>

- Janela Principal
- Interface gráfica simples
- Bibliotecas de leitura de disco; monitor; e window memory (elas estão localizadas no diretório `/Hardware`) 


**LukaOS**

![LukaOS](https://github.com/LukaZSH/Criando-um-SO/assets/49702498/f8218770-077d-4a43-9d13-139b7fb8bdc0)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
**Janela**


![Janela LukaOS](https://github.com/LukaZSH/Criando-um-SO/assets/49702498/cce1da74-9bcd-4001-8324-b5529e7e1e2f)

-----------------------------------------------------------------------------------------------------------------------------------------------------------------------
 
<h2>Observações</h2>

Utilizei o `VirtualBox` para testar o SO, o armazenamento dessa VM foi alterado para utilizar um "HD externo" para ser o HD e dar boot no sistema, no caso, utilizei um pendrive como "HD externo".




