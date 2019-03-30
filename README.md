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


## Configurando Flutter
- Clone o repositório do git -> git clone -b beta https://github.com/flutter/flutter.git

- insira o flutter como variavel de ambiente, pegue o caminho <workspace>/flutter/bin, no meu caso coloquei no /etc/profile 
    -> echo export PATH="$PATH:/home/projects/flutter/flutter/bin" >> /etc/profile

- autualize 
    -> source /etc/profile

## PRONTO, agora crie um projeto 
    -> flutter create MyProject

- verifique se está tudo OK antes de compilar 
    -> flutter doctor -v

- abaixo algumas soluções para problemas que tive :
    - [SEM SDK]    Instale a sdk caso não tenha [LINUX] 
        -> apt-get install android-sdk
   
    - [SDK ANTIGA] Caso não tenha o sdkmanager baixe em [LINUX]  
        -> https://developer.android.com/studio/index.html#downloads
   
    - [SDK ANTIGA & SDKMANAGER] substitua /usr/lib/android-sdk/tools pelo que foi baixado e execute para atualizar a sdk 
        -> /usr/lib/android-sdk/tools/bin/sdkmanager "platforms;android-28" "build-tools;28.0.3"
   
    - [LICENÇAS SDK] para aceitar as licensas 
        -> yes | /usr/lib/android-sdk/tools/bin/sdkmanager --licenses

  agora basta conectar seu aparelho android no ubs e executar
    -> flutter run

    se estiver tudo certo irá abrir um aplicativo DEMO .
