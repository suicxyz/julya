# Início da Jornada

## Configurando ambiente de desenvolvimento

Imagino que sua máquina seja Windows 10, e não um sistema Unix como a minha, então irei te ensinar a configurar o seu
ambiente de desenvolvimento para ficar o mais parecido possível com o meu.

## Instalando e configurando WSL & Ubuntu

### WSL - Windows Subsystem Linux

Abra o PowerShell (como **administrador**) e digite o seguinte comando para habilitar o WSL:

```
dism.exe /online /enable-feature /featurename:Microsoft-Windows-Subsystem-Linux /all /norestart
```

Para habilitar o recurso de máquina virtual, para instalar o Linux, digite o seguinte comando:

```
dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
```

Defina o WSL2 como versão padrão com o seguinte comando:

```
wsl --set-default-version 2
```

Pronto, seu WSL está configurado! Agora vamos configurar o Ubuntu.

### Ubuntu

Abra sua Microsoft Store e escolha sua distro Linux a ser instalada. Podendo ser Ubuntu, Debian (a que eu uso), Kali Linux
ou OpenSuse, mas eu recomendo instalar o Ubuntu. Instale sempre a versão com o maior número e contendo LTS no nome.

Após instalado, abra o Ubuntu, e na primeira execução, e somente na primeira, você irá criar sua conta UNIX, com nome de 
usuário e senha.

Por exemplo:

```
Enter new UNIX username: julya
Enter new UNIX password: ********
Retype new UNIX password: ********
passwd: password updated succesfully
Installation successful!
To ru a command as administrador (user "root", use "sudo <command>".
See "man sudo_root" for details.

julya@DESKTOP-8013ENL:~$
```

Recomendo fortemente escolher uma senha com oito ou mais digitos.

Pronto! Configuramos o WSL e o Ubuntu na sua máquina.

## Instalando e configurando o Windows Terminal

O Windows Terminal é o aplicativo de Terminal feito pela Microsoft, inclusive é o melhor para trabalhar com o WSL.

Abra sua Microsft Store e procure por Windows Terminal, instale o aplicativo na sua máquina e execute-o.

Abra as configurações apertando `shift + ,` (vírgula) e selecione o **Default Profile** ou **Perfil Padrão**, mude de
PowerShell para Ubuntu 22.04 ou algo parecido. Feche o Windows Terminal e abra-o novamente. Ele deverá iniciar no 
Ubuntu.

Pronto! Instalamos o Windows Terminal e o configuramos da maneira correta!

## Mão na massa!

A partir de agora você já tem tudo que precisa para colocar a mão na massa e iniciar os estudos. 
Happy hacking!

## Links úteis:

### Guia oficial da Microsoft:

https://learn.microsoft.com/pt-br/windows/wsl/install

### Ubuntu na Microsoft Store:

https://apps.microsoft.com/store/detail/ubuntu/9PDXGNCFSCZV

### Windows Terminal na Microsoft Store:

https://apps.microsoft.com/store/detail/windows-terminal/9N0DX20HK701

### Tutorial mais detalhado:

https://www.youtube.com/watch?v=hd6lxt5iVsg
