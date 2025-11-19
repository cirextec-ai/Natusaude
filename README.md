# NatuSaude

# 📘 Documentação do Projeto NatuSaude

## 📌 Descrição breve do sistema
O **NatuSaude** é um protótipo de aplicativo móvel que disponibiliza um banco de dados sobre produtos naturais e fitoterápicos oriundos da flora do Estado do Amazonas. É um protótipo de pesquisa para usuários que buscam informações confiáveis sobre produtos naturais e medicinais, auxiliando em práticas de complementação saudável e tratamentos terapêuticos naturais.
O sistema busca conectar consumidores e pequenos produtores, promovendo o uso consciente dos fitoterápicos, a valorização do conhecimento tradicional e a preservação da biodiversidade amazônica.  

## 🏗️ Arquitetura resumida
O aplicativo foi desenvolvido na plataforma **Android Studio**, utilizando a linguagem **Kotlin** e a biblioteca **Jetpack Compose** para construção das interfaces gráficas.  
A arquitetura adotada é **MVVM (Model-View-ViewModel) **, garantindo separação de responsabilidades e facilidade de manutenção.  
O armazenamento e consulta de dados são feitos no **Firebase Realtime Database**.

- ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white) **Kotlin** → Linguagem principal para o desenvolvimento Android.  
- ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) **Android Studio + Jetpack Compose** → Criação da interface do usuário.  
- ![MVVM](https://img.shields.io/badge/MVVM-Architecture-blueviolet?style=flat-square) **Arquitetura MVVM** → Organização entre **Model**, **View** e **ViewModel**.  

### Estrutura Simplificada
- **UI (Jetpack Compose):** telas e componentes de interação com o usuário.  
- **ViewModel:** camada responsável pela lógica de apresentação e comunicação com os repositórios.  
- **Repository:** abstração do acesso aos dados e integração com o Firebase.  
- **Model:** entidades de domínio, como produtos, plantas e usuários.  
- **Firebase Realtime Database:** banco de dados em nuvem para persistência das informações.  

## 🛠️ Tecnologias Utilizadas  

- ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?logo=kotlin&logoColor=white) **Kotlin** → Linguagem principal para o desenvolvimento Android.  
- ![Android](https://img.shields.io/badge/Android-3DDC84?logo=android&logoColor=white) **Android Studio + Jetpack Compose** → Criação da interface do usuário.  
- ![MVVM](https://img.shields.io/badge/MVVM-Architecture-blueviolet?style=flat-square) **Arquitetura MVVM** → Organização entre **Model**, **View** e **ViewModel**.  
- 🔥 **Firebase Realtime Database** → Armazenamento e sincronização de dados em tempo real.  

## 📱 Funcionalidades do Protótipo  
- Visualização de **categorias de fitoterápicos**.  
- Lista de produtos com **nome, descrição, fabricante e loja**.  
- **Guias educativos** sobre uso correto.  
- Tela de **avaliação da usabilidade** (escala de 1 a 5).  
- **Sincronização em tempo real** dos dados (mesmo offline).

▶️ Como Executar o Sistema (Rodar Localmente)

Para rodar o aplicativo NatuSaude localmente em ambiente de desenvolvimento, siga os passos abaixo:

✅ Pré-requisitos

Antes de começar, certifique-se de ter os seguintes softwares instalados:

Android Studio (Bumblebee ou superior)

Java Development Kit (JDK 11 ou superior)

Kotlin (incluso no Android Studio)

Emulador Android configurado ou dispositivo físico com modo de desenvolvedor habilitado

Conexão com a internet para acesso ao Firebase

📦 Dependências Utilizadas

Certifique-se de que o build.gradle contém (ou adicione) as dependências principais:

// Jetpack Compose
implementation "androidx.compose.ui:ui:1.5.0"
implementation "androidx.compose.material:material:1.5.0"
implementation "androidx.compose.ui:ui-tooling-preview:1.5.0"

// Lifecycle + ViewModel (MVVM)
implementation "androidx.lifecycle:lifecycle-runtime-ktx:2.6.1"
implementation "androidx.lifecycle:lifecycle-viewmodel-compose:2.6.1"

// Firebase Realtime Database
implementation 'com.google.firebase:firebase-database-ktx:20.3.0'
implementation 'com.google.firebase:firebase-common-ktx:20.4.1'

// Firebase (Core)
implementation platform('com.google.firebase:firebase-bom:32.2.2')
implementation 'com.google.firebase:firebase-analytics-ktx'

// Outras (opcional)
implementation "androidx.navigation:navigation-compose:2.7.3"


No final do build.gradle (app), certifique-se de incluir:

apply plugin: 'com.google.gms.google-services'


No build.gradle (project):

classpath 'com.google.gms:google-services:4.3.15'

🛠️ Passo a Passo para Execução

Clone o Repositório (se aplicável)

git clone https://github.com/seu-usuario/natusaude.git
cd natusaude


Abra o projeto no Android Studio

Vá em File > Open, e selecione a pasta do projeto.

Configure o Firebase

Acesse o Firebase Console
, crie um projeto com o nome "Natusaude".

Baixe o arquivo google-services.json e adicione à pasta app/ do projeto.

No Firebase, ative o Realtime Database e configure as permissões (exemplo para teste):

{
  "rules": {
    ".read": true,
    ".write": true
  }
}


Sincronize o projeto com o Gradle

Clique em "Sync Now" quando solicitado ou vá em File > Sync Project with Gradle Files.

Compile e execute o projeto

Escolha um emulador ou conecte um dispositivo físico.

Clique em Run > Run 'app' ou pressione Shift + F10.

🧪 Testando o Protótipo

Após iniciar o app, você poderá:

Navegar pelas categorias de fitoterápicos

Ver detalhes dos produtos naturais

Acessar guias educativos

Avaliar a usabilidade na tela de avaliação

⚠️ Observações Importantes

O app está preparado para funcionar offline, sincronizando dados assim que houver conexão.

Esta é uma versão protótipo, apenas para fins educacionais e demonstrativos.

Em ambiente de produção, as regras de segurança do Firebase devem ser ajustadas adequadamente.


## 🚀 Status do Projeto  
✅ Protótipo inicial desenvolvido  
🔄 Em fase de testes de usabilidade  
📌 Próximos passos: expansão da base de dados, integração de geolocalização e certificação de produtores.  

## 👨‍💻 Autor:  Sergio Ademir 
