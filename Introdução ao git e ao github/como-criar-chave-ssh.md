1-Entrebem seu github
Clique na sua imagem deois em settings
vá até SSH and GPG keys
new SSH key
Depois abra o git bash
digite no terminal do git bahs
ssh-keygen -t ed25519 -C seu email
digite uma senha para sua chave
vá até a pasta que foi gerada sua chave pelo git bash
cd /Users/Seu usuario do pc/.ssh/
cat id_ed25519.pub
copie sua chave 
volte ao github 
coloque um titulo de sua preferencia e cole a chave que você copiou no gitbash
depois é so gerar a chave o github irá pedir sua senha do github
e pronto sua chave foi gerada
agora é preciso inicializar os ssh agent
volte ao gitbash na pasta onde paramos "cd /Users/Seu usuario do pc/.ssh/"
E digite eval $(ssh-agent -s) 
ira gerar um numero Agent pid 
agora é preciso passar a chave privada para o agent
na mesma pasta .ssh digite ssh-add id_ed25519 aperte ENTER
Ele vai pedir a senha da sua chave, digite e aperte ENTER
E pronto sua chave foi adcionada
