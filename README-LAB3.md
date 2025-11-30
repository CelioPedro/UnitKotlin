# Desafio de Projeto (Lab 3): GitHub Search App

Este desafio consistiu em transformar um projeto Android esqueleto, cheio de `TODOs`, em um aplicativo funcional que permite aos usuários pesquisar repositórios de um usuário no GitHub, visualizar a lista, abrir um repositório no navegador e compartilhar seu link.

---

## Jornada de Desenvolvimento e Depuração

O processo de desenvolvimento foi um ciclo completo de implementação e depuração. Começamos com um ambiente de compilação quebrado, implementamos a lógica principal do aplicativo e, em seguida, corrigimos uma série de bugs, desde problemas de interface do usuário até crashes críticos em tempo de execução.

### Problema 1: Ambiente de Compilação Quebrado (Gradle)

-   **Problema:** O projeto não compilava, com o Gradle Sync falhando devido a uma incompatibilidade entre a versão do Gradle (8.5) e a versão do Android Gradle Plugin (AGP 7.2.2).
-   **Solução:**
    1.  Ajustamos a versão do Gradle no arquivo `gradle/wrapper/gradle-wrapper.properties` para `7.4.2`.
    2.  Atualizamos o AGP para `7.3.1` e o plugin do Kotlin para `1.7.20` no arquivo `build.gradle` do projeto.
    3.  Atualizamos dependências como `appcompat` e `material` para garantir a estabilidade.
-   **Aprendizado:** A configuração do ambiente de compilação é a base de tudo. Manter a compatibilidade entre Gradle, AGP e o plugin do Kotlin é fundamental.

### Problema 2: Entrada de Usuário Aceitava Apenas Números

-   **Problema:** O campo de texto para o nome de usuário do GitHub só permitia a entrada de números.
-   **Solução:** No arquivo `activity_main.xml`, alteramos o atributo `android:inputType` do `EditText` de `"numberDecimal"` para `"text"`.
-   **Aprendizado:** A interface do usuário deve sempre corresponder à natureza dos dados que ela manipula.

### Problema 3: O Aplicativo Fechava ao Clicar em "Confirmar"

-   **Problema:** O aplicativo sofria um *crash* ao tentar realizar a busca, pois tentava acessar a internet sem a permissão necessária.
-   **Solução:** Adicionamos a permissão de internet ao `AndroidManifest.xml` com a linha `<uses-permission android:name="android.permission.INTERNET" />`.
-   **Aprendizado:** Permissões críticas, como o acesso à internet, devem ser declaradas explicitamente no manifesto.

### Problema 4: Erros de Compilação por Referências Não Resolvidas

-   **Problema:** O código em `MainActivity.kt` não compilava, mostrando erros de `Unresolved reference` para recursos de string.
-   **Solução:** Adicionamos as definições de string que faltavam (`saved_user_key`, `response_error`, etc.) ao arquivo `res/values/strings.xml`.
-   **Aprendizado:** Externalizar todas as strings para o arquivo `strings.xml` é uma boa prática que organiza o código, facilita a tradução e evita erros de compilação.

---

## Como Encontrar os Arquivos da Solução

Os principais arquivos que foram modificados para a solução deste desafio podem ser encontrados nos seguintes caminhos, dentro da pasta do projeto (`src/main/kotlin/desafioGithubSearch/`):

-   **Lógica Principal:** `app/src/main/java/com/dio/github/ui/MainActivity.kt`
-   **Layouts da Interface:** `app/src/main/res/layout/`
-   **Strings e Recursos:** `app/src/main/res/values/strings.xml`
-   **Manifesto (Permissões):** `app/src/main/AndroidManifest.xml`
-   **Scripts de Build (Gradle):** `build.gradle` (projeto) e `app/build.gradle` (módulo)

## Conclusão

Este desafio reforçou a importância da configuração correta do ambiente, da atenção aos detalhes no layout e da compreensão do sistema de permissões do Android. Passar pelo ciclo de depuração, desde um ambiente quebrado até um aplicativo funcional, proporcionou lições valiosas e práticas sobre o desenvolvimento Android no dia a dia.
