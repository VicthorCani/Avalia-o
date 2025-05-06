1. Como criar um emulador no Android Studio

-> Abra o Android Studio.
-> Vá em Tools > Device Manager.
-> Clique em Create Device.
-> Escolha o tipo de dispositivo (por exemplo: Pixel 5) e clique em Next.
-> Escolha uma imagem do sistema Android (recomendo uma versão recente, como "API 30" ou superior). Clique em Download se ainda não tiver.
-> Depois de baixar, clique em Next.
-> Dê um nome ao emulador e ajuste as configurações, se quiser.
-> Clique em Finish.
-> Agora você verá seu emulador listado. Clique no ícone de Play (▶) para iniciá-lo.

2. Como habilitar o SDK

-> No Android Studio, vá em File > Settings (ou Android Studio > Preferences no macOS).
-> Vá para Appearance & Behavior > System Settings > Android SDK.
-> Na aba SDK Platforms, certifique-se de que uma versão do Android (ex: Android 11, API 30) está marcada.
-> Na aba SDK Tools, marque:
-> Android SDK Build-Tools
-> Android Emulator
-> Android SDK Platform-Tools
-> Intel x86 Emulator Accelerator (HAXM) – se estiver usando Intel
-> Clique em Apply e depois em OK.

3. Como configurar o ANDROID_HOME e JAVA_HOME nas variáveis de ambiente da sua conta?

Acesse o menu Iniciar, pesquise por Variáveis de Ambiente e clique em "Editar variáveis de ambiente do sistema".
Na janela que abrir, clique em "Variáveis de Ambiente...".
Em Variáveis de usuário, clique em "Nova..." e preencha da seguinte forma:
Nome da variável: ANDROID_HOME
Valor da variável: C:\Users\SeuUsuario\AppData\Local\Android\Sdk
(substitua "SeuUsuario" pelo seu nome de usuário do Windows)
Clique novamente em "Nova..." e adicione:
Nome da variável: JAVA_HOME
Valor da variável: C:\Program Files\Android\Android Studio\jbr
Ainda em Variáveis de Ambiente, selecione a variável Path e clique em Editar. Depois, adicione as seguintes entradas:

%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\emulator
%JAVA_HOME%\bin

Clique em OK em todas as janelas para salvar as alterações.

4. Como fazer para abrir o projeto no emulador?

Com o projeto aberto no Android Studio, vá até a parte superior da tela e veja o menu de dispositivos.
Certifique-se de que seu emulador (ex: Pixel 5 API 30) esteja selecionado.
Clique no ícone Run ou use o atalho Shift + F10.
O Android Studio irá compilar e abrir seu projeto automaticamente no emulador.
