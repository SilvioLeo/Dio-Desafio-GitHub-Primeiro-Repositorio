1-Entrebem seu github
##
2-Clique na sua imagem depois em settings
##
3-Vá até SSH and GPG keys
##
4-new SSH key
##
5-Depois abra o git bash
##
6-Digite no terminal do git bahs
##
7-ssh-keygen -t ed25519 -C seu email
##
8-Digite uma senha para sua chave
##
9-Vá até a pasta que foi gerada sua chave pelo git bash
##
10-cd /Users/Seu usuario do pc/.ssh/
##
11-Digite cat id_ed25519.pub
##
12-Copie sua chave 
##
13-Volte ao github 
##
14-Coloque um titulo de sua preferencia e cole a chave que você copiou no gitbash
##
15-Depois é so gerar a chave o github irá pedir sua senha do github
##
16-E pronto sua chave foi gerada
##
17-Agora é preciso inicializar os ssh agent
##
18-Volte ao gitbash na pasta onde paramos "cd /Users/Seu usuario do pc/.ssh/"
##
19-E digite eval $(ssh-agent -s) 
##
20-Ira gerar um numero Agent pid 
##
21-Agora é preciso passar a chave privada para o agent
##
22-Na mesma pasta .ssh digite ssh-add id_ed25519 aperte ENTER
##
23-Ele vai pedir a senha da sua chave, digite e aperte ENTER
##
24-E pronto sua chave foi adicionada
