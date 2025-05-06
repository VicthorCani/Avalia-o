1. Como criar um emulador no Android Studio

Abra o Android Studio.
Vá em Tools > Device Manager.
Clique em Create Device.
Escolha o tipo de dispositivo (por exemplo: Pixel 5) e clique em Next.
Escolha uma imagem do sistema Android (recomendo uma versão recente, como "API 30" ou superior). Clique em Download se ainda não tiver.
Depois de baixar, clique em Next.
Dê um nome ao emulador e ajuste as configurações, se quiser.
lique em Finish.
Agora você verá seu emulador listado. Clique no ícone de Play (▶) para iniciá-lo.

2. Como habilitar o SDK

Primeiro ir no Android Studio e ir em: More Options > SDK Manager > SDK Tools e instalar o NDK e Android SDK Command
 
Depois de instalado no seu projeto dentro da pasta android crie um arquivo chamado local.properties e coloque
sdk.dir=C:\\Users\\seuusuario\\AppData\\Local\\Android\\Sdk
 
Logo após abra o powershell e copie e cole:
cd "C:\Users\seuusuario\AppData\Local\Android\Sdk\cmdline-tools\latest\bin"
.\sdkmanager.bat --licenses

 E aceite todas as solicitações que irá aparecer!

3. Como configurar o ANDROID_HOME e JAVA_HOME nas variáveis de ambiente da sua conta?

Acesse o menu Iniciar, pesquise por Variáveis de Ambiente e clique em "Editar variáveis de ambiente do sistema na sua conta".
Na janela que abrir, clique em "Variáveis de Ambiente...".
Em Variáveis de usuário, clique em "Nova..." e preencha da seguinte forma:
Nome da variável: ANDROID_HOME
Valor da variável: C:\Users\SeuUsuario\AppData\Local\Android\Sdk (substitua "SeuUsuario" pelo seu nome de usuário do Windows)
Clique novamente em "Nova..." e adicione:
Nome da variável: JAVA_HOME
Valor da variável: C:\Program Files\Android\Android Studio\jbr
Ainda em Variáveis de Ambiente, selecione a variável Path e clique em Editar. Depois, adicione as seguintes entradas:

%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\emulator
%JAVA_HOME%\bin

Clique em OK em todas as janelas para salvar as alterações.

4. Como fazer para abrir o projeto no emulador?

Primeiro você abrirá o android studio;
Para abrir o projeto coloque o seguinte código: 'npm start' e 'depois npm run android'. Após esse código abrira no seu emulador.
