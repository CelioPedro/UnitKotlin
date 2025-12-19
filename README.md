<table style="width: 100%;" border="0">
  <tr>
    <td align="left" style="width: 99%;">
      <h1>Android Developer - Kotlin</h1>
    </td>
    <td align="right" style="width: 1%;">
      <img src="src/main/resources/icons/mobiledev.webp" alt="DIO Logo" width="80px">
    </td>
  </tr>
</table>

Bem-vindo ao meu repositório de estudos! Aqui concentro os códigos, anotações e soluções dos desafios propostos no bootcamp de Desenvolvimento Android com Kotlin.

### O objetivo é documentar minha evolução, desde a lógica básica até a arquitetura avançada de apps.

<p align="center">
  <img src="src/main/resources/icons/Kotlin11.webp" alt="Kotlin Logo 1" width="65px">
  <img src="src/main/resources/icons/Kotlin2.webp" alt="Kotlin Logo 2" width="65px">
  <img src="src/main/resources/icons/func.webp" alt="Funcional Icon" width="65px">
</p>

## Desafios e Projetos:

<p align="center">
  <img src="src/main/resources/icons/Desafio.webp" alt="Desafio Icon" width="65px">
  <img src="src/main/resources/icons/Gold.webp" alt="Ouro Icon" width="65px">
</p>

Abaixo listo os desafios práticos do curso, organizados por nível de complexidade e módulo.

------------------------------------------------------------------------------------------

### Nível Básico: Fundamentos e Lógica. 

<img src="src/main/resources/icons/Android1.webp" alt="Android Icon" width="60px">

Foco em sintaxe Kotlin, Orientação a Objetos e estruturas de controle.

| Ícone | Desafio | Minha Solução e Tecnologias | Link |
|:---:|---------|-----------------------------|------|
| <img src="src/main/resources/icons/Abstração.webp" alt="Abstração Icon" width="72px"> | Abstraindo Formações da DIO | POO em Kotlin<br>Modelei as classes Conteudo, Curso e Mentoria para representar a plataforma, aplicando herança e polimorfismo.<br><br> *Techs: Kotlin, POO* | 🔗 [Código](https://github.com/CelioPedro/UnitKotlin/blob/main/src/main/kotlin/desafioAbstra%C3%A7%C3%A3oForma%C3%A7%C3%B5es) |
| <img src="src/main/resources/icons/func.webp" alt="Funcional Icon" width="72px"> | Controle de Fluxo e Coleções | Desafio de Código<br>Scripts focados em manipulação de Lists, Maps e estruturas condicionais para resolver problemas lógicos. | Auto check 🆗 |

------------------------------------------------------------------------------------------

### Nível Intermediário: Interfaces Nativas. 

<img src="src/main/resources/icons/Android2.webp" alt="Android Icon" width="60px">

Criação de Apps Android tradicionais (XML/View System) e recursos essenciais.

| Ícone | Desafio | Minha Solução e Tecnologias | Link |
|:---:|---------|-----------------------------|------|
| <img src="src/main/resources/icons/Idiomas.webp" alt="Idiomas Icon" width="72px"> | App com Suporte a Vários Idiomas | Internacionalização<br>Implementação de recursos de String resources e configuração de Locales no Android Studio.<br><br> *Techs: Android XML, Resources* | 🔗 [Código](https://github.com/CelioPedro/UnitKotlin/tree/main/src/main/kotlin/desafioInternationalApp) |
| <img src="src/main/resources/icons/github.webp" alt="GitHub Icon" width="72px"> | App para Compartilhamento de Projetos | Portfólio de projetos<br>Criação de um App Android para compartilhar seus projetos.<br><br> *Techs: Android XML, Resources* | 🔗 [Código](https://github.com/CelioPedro/UnitKotlin/tree/main/src/main/kotlin/desafioGithubSearch/app/src) |

------------------------------------------------------------------------------------------

### Nível Avançado: Jetpack Compose & Arquitetura. 

<img src="src/main/resources/icons/Android3.webp" alt="Android Icon" width="60px">

Desenvolvimento moderno com interfaces declarativas e injeção de dependência.

| Ícone | Desafio | Minha Solução e Tecnologias | Link |
|:---:|---------|-----------------------------|------|
| <img src="src/main/resources/icons/Cup.webp" alt="Cup Icon" width="72px"> | App para Acompanhar a Copa | Projeto Capstone<br>App completo consumindo API de jogos. Utilizei WorkManager para tarefas em background e Hilt para injeção de dependências.<br><br> *Techs: Jetpack Compose, Retrofit, Hilt* | 🔗 [Código](https://github.com/CelioPedro/UnitKotlin/tree/main/src/main/kotlin/desafioGithubSearch/app/src) |
------------------------------------------------------------------------------------------

## Tecnologias e Ferramentas:

### Tópicos Estudados

| Categoria | Tecnologias | Ícones |
|-----------|-------------|--------|
| **Arquitetura** | MVVM, Clean Architecture | ![CLean](https://img.shields.io/badge/Clean%20Architecture%20-7F52FF?style=for-the-badge&logo=jetpack-compose&logoColor=white)|
| **Bibliotecas** | Retrofit, Room, Hilt, WorkManager |  ![Retrofit](https://img.shields.io/badge/Retrofit-3DDC84?style=for-the-badge&logo=android&logoColor=white) |
| **UI** | XML Layouts, Jetpack Compose | ![Jetpack](https://img.shields.io/badge/Jetpack%20Compose-7F52FF?style=for-the-badge&logo=jetpack-compose&logoColor=white) |
| **Linguagem** | Kotlin | ![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=for-the-badge&logo=kotlin&logoColor=white) |
| **IDE** | Android Studio | ![Android Studio](https://img.shields.io/badge/Android%20Studio-3DDC84?style=for-the-badge&logo=android-studio&logoColor=white) |
| **Plataforma** | Android | ![Android](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white) |
------------------------------------------------------------------------------------------

## 📂 Estrutura do Repositório

Como este repositório agrupa vários laboratórios, a estrutura segue o padrão do curso:

```
├── 📁 .idea/                # Configurações do IntelliJ/Android Studio
├── 📁 src/
│   └── 📁 main/
│       └── 📁 kotlin/       # Código fonte dos desafios de lógica (Labs)
│           ├── 📁 desafio1  # Solução do desafio de POO
│           └── 📁 desafio2  # Solução do desafio de Controle de Fluxo
├── 📁 projetos/             # Apps Android completos (Copa, Idiomas, etc)
└── 📄 README.md             # Documentação principal
```


🤝 Contato

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/celiopedro)

<p align="center">Desenvolvido por [Celio Pedro](https://github.com/CelioPedro) durante o Bootcamp da DIO.</p>
