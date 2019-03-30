# myapp

A new Flutter project.

## Getting Started

This project is a starting point for a Flutter application.

A few resources to get you started if this is your first Flutter project:

- [Lab: Write your first Flutter app](https://flutter.io/docs/get-started/codelab)
- [Cookbook: Useful Flutter samples](https://flutter.io/docs/cookbook)

For help getting started with Flutter, view our 
[online documentation](https://flutter.io/docs), which offers tutorials, 
samples, guidance on mobile development, and a full API reference.


## Configurando o Framework em ambiente LINUX

**Clone o repositório do git oficial do flutter**

` git clone -b beta https://github.com/flutter/flutter.git`

**insira o flutter como variável de ambiente, pegue o caminho <workspace>/flutter/bin, no meu caso coloquei no /etc/profile **

`echo export PATH="$PATH:/home/projects/flutter/flutter/bin" >> /etc/profile`

**atualize as alterações** 
`source /etc/profile`

## Criando um projeto ...

**Após ter feito os passos anteriores, basta criar ou acessar algum workspace de sua preferencia e criar o projeto**

`flutter create <nomeProjeto>`

**Verifique se está tudo OK antes de compilar executando o seguinte comando**

`flutter doctor -v`

***

### **Alguns problemas que tive ...**

**SEM SDK INSTALADA** - Instale a sdk caso não tenha

`apt-get install android-sdk`
 
**SDK 23 E FLUTTER TRABALHA COM 28** - baixe o tools atualizado direto da google 

`https://developer.android.com/studio/index.html#downloads`

substitua em  `/usr/lib/android-sdk/tools` pelo que foi baixado e execute 

`/usr/lib/android-sdk/tools/bin/sdkmanager "platforms;android-28" "build-tools;28.0.3"`
   
**ACEITAR LICENÇAS DA SDK**  - para aceitar as licenças 

`yes | /usr/lib/android-sdk/tools/bin/sdkmanager --licenses`

***
## OK ... BORA TESTAR!

agora basta conectar seu aparelho android no ubs e executar

`flutter run`
### se estiver tudo certo irá abrir um aplicativo DEMO .
