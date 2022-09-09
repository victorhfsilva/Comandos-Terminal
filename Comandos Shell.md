# Comandos Shell

## Diretórios
Lista diretórios
```
ls
```
Muda de diretório
```
cd <nome_dir>
```
Retroceder diretório
```
cd ..
```
Criar um diretório
```
mkdir <nome_dir>
```
Remover um Diretório
```
rm -rf <nome_dir>
```
Imprime o nome do diretório atual
```
pwd
```

## Arquivos
Imprime string em um arquivo
```
echo Hello World > hello_world.txt
```
Cria um arquivo vazio
```
touch <nome_arquivo>
```

Deletar um arquivo
```
rm <nome_arquivo>
```
Move um arquivo
```
mv <nome_arquivo> <pasta>
```
Renomeia um arquivo
```
mv <nome_arquivo> <novo_nome>
```

Imprime o conteúdo de um arquivo
```
more <nome_arquivo>
```
ou
```
cat <nome_arquivo>
```
Mostra árvore de arquivos da pasta atual
```
find
```
Mostra árvore de arquivos de uma pasta em específico
```
find <nome_pasta>
```
## Tela
Limpar a Tela (Ctrl+L)
```
clear
```
Imprime string na tela
```
echo <string>
```
## Instalação
Instala pacote deb
```
dpkg -i <pacote.deb>
```
Instala pacote rpm
```
rpm -Uvh <pacote.rpm>
```

## Pesquisa

Pesquisa por padrão em arquivos
```
grep <padrão> <nome_arquivos>
```
Pesquisa por padrão em diretório
```
grep -r <padrão> <nome_diretório>
```
Pesquisa por padrão no output de um comando
```
<comando> | grep <padrão>
```
## Compressão
Comprime os arquivos em um arquivo tar
```
tar cf <arquivo.tar> <nome_arquivos>
```
Extrai um arquivo tar
```
tar xf <arquivo.tar>
```
Comprime os arquivos em um arquivo tar.gz
```
tar czf <arquivo.tar.gz> <nome_arquivos>
```
Extrai um arquivo tar.gz
```
tar xzf <arquivo.tar.gz>
```
Comprime os arquivos em um arquivo tar.bz2
```
tar cjf <arquivo.tar.bz2> <nome_arquivos>
```
Extrai um arquivo tar.bz2
```
tar xjf <arquivo.tar.bz2>
```
Comprime os arquivos em um arquivo gz
```
gzip <nome_arquivo>
```
Extrai um arquivo gz
```
gzip -d <arquivo.gz>
```

## Processos
Lista todos os processos ativos
```
ps
```
Encerra processo com um específico PID
```
kill <PID>
```
Encerra todos os processos com um nome em específico
```
killall <nome_processo>
```
## Permissões
Muda as permissões de um arquivo (4 = read, 2 = write, 1 = execute; o = owner, g = group, w = world)
```
chmod <ogw> <nome_arquivo>
```
## Redes
Testa a conectividade de equipamentos
```
ping <endereço_IP>
```
Traça a Rota até determinado endereço IP
```
traceroute <endereço_IP>
```
Obtêm informações sobre registro DNS de determinado domínio
```
nslookup <endereço_DNS>
```
## Sistema
Mostra informações do Kernel
```
uname -a
```
Mostra utilização do disco
```
df
```
Mostra utilização da memória e SWAP
```
free
```
Mostra informações da distribuição do Linux
```
lsb_release -a
```
## Criptografia
### Hash
Obtém um Hash do tipo SHA1
```
openssl sha1 <nome_arquivo>
```


