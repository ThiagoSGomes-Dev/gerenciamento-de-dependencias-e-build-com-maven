# Gerenciamento de dependências e build com Maven
📦 Repositório da aula de gerenciamento de dependências e build utilizando Maven do BootCamp Santander 2024 - Backend com Java. Aqui, exploramos como configurar e otimizar projetos Java com Maven de maneira eficiente!

## Iniciar um projeto com Maven

No seu terminal, inicie usando o comando `mvn archetype:generate`. Nessa abordagem, vamos seguir o curso padrão de instalação do Maven, passando por cada etapa.

```markdown
mvn archetype:generate
````

## Escolha o Arquétipo:

```markdown
Pergunta:
Choose a number or apply filter (format: [groupId:]artifactId, case sensitive contains): 2155:
Tradução:
Escolha um número ou aplique o filtro (formato: [groupId:]artifactId, diferenciação de maiúsculas e minúsculas): 2155:
````

Em Maven, um "arquétipo" (archetype, em inglês) é um modelo ou padrão de projeto que você pode usar como base para criar novos projetos Maven. Ele define a estrutura inicial do projeto, os diretórios e os arquivos básicos que serão criados.

Quando você executa o comando `mvn archetype:generate`, o Maven oferece uma lista de arquétipos disponíveis para você escolher. Cada arquétipo pode ser pensado como um tipo de projeto pré-configurado para diferentes finalidades.

Por exemplo, o arquétipo `maven-archetype-quickstart` é um modelo básico para projetos Java simples. Ele cria uma estrutura mínima com um arquivo de classe principal e um arquivo de configuração de build (pom.xml).

### Exemplo da Lista:

```markdown
2155: remote -> org.apache.maven.archetypes:maven-archetype-quickstart 
2156: remote -> org.apache.maven.archetypes:maven-archetype-simple 
````

Com isso, responda a primeira etapa com o número que corresponde ao `maven-archetype-quickstart`.

## Escolha a versão do Maven:

```markdown
Pergunta:
Choose org.apache.maven.archetypes:maven-archetype-quickstart version:
Tradução:
Escolha a versão de org.apache.maven.archetypes:maven-archetype-quickstart:
````

Como no passo anterior, o Maven exibirá uma lista com as versões disponíveis para criar um projeto em Maven.

### Exemplo da Lista:

````
1: 1.0-alpha-1
2: 1.0-alpha-2
3: 1.0-alpha-3
4: 1.0-alpha-4
5: 1.0
6: 1.1
7: 1.3
8: 1.4
Choose a number: 8: 8
````

## Definição das Propriedades do Projeto Maven

Ao gerar um novo projeto Maven, você precisará definir algumas propriedades importantes que ajudarão a identificar e organizar seu projeto. Vamos explicar cada uma dessas propriedades:

1. **Define value for property 'groupId': com.meuprojetojavacommaven**

    - **groupId**: Este campo define o identificador do grupo para o projeto, geralmente baseado na estrutura de domínio invertida do seu pacote. É uma maneira de organizar os projetos e evitar conflitos de nomes. Por exemplo, `com.meuprojetojavacommaven` indica que este projeto pertence ao grupo `com.meuprojetojavacommaven`.

2. **Define value for property 'artifactId': gerd-dependencias-com-maven**

    - **artifactId**: Este campo define o identificador exclusivo do artefato dentro do grupo. Ele representa o nome do projeto ou módulo. Por exemplo, `gerd-dependencias-com-maven` é o nome do artefato que está sendo criado.

3. **Define value for property 'version' 1.0-SNAPSHOT: : 1.0**

    - **version**: Este campo define a versão do artefato. Versões podem seguir diferentes convenções, mas uma prática comum é usar números de versão que seguem um esquema como `1.0`, `1.1`, etc. A palavra `SNAPSHOT` indica uma versão de desenvolvimento que pode mudar antes da próxima versão estável. No exemplo, estamos definindo a versão como `1.0`.

4. **Define value for property 'package' com.meuprojetojavacommaven: : com.meuprojetojavacommaven**

    - **package**: Este campo define o pacote base para o código-fonte gerado. É comum usar o mesmo valor do `groupId` para manter a consistência. No exemplo, `com.meuprojetojavacommaven` é usado como o pacote base para todas as classes Java no projeto.

## Confirm properties configuration:

Após definir todos os valores, o Maven pedirá uma confirmação para garantir que todas as propriedades foram inseridas corretamente:

### Exemplo que você vai visualizar:

```markdown
Confirm properties configuration:
groupId: com.meuprojetojavacommaven
artifactId: gerd-dependencias-com-maven
version: 1.0
package: com.meuprojetojavacommaven
 Y: : 
````

## Confirmação:

Revise todas as propriedades configuradas. Se estiverem corretas, confirme digitando `Y`. Isso informará ao Maven que você deseja prosseguir com a criação do projeto usando as configurações fornecidas.
