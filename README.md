# 🕷️ JSoup Example - Web Scraping com Java

<div align="center">

![Java](https://img.shields.io/badge/Java-7+-ED8B00?logo=openjdk&logoColor=white)
![JSoup](https://img.shields.io/badge/JSoup-1.14.2+-orange?logo=java&logoColor=white)
![Maven](https://img.shields.io/badge/Maven-3.7+-C71A36?logo=apache-maven&logoColor=white)
![HTML](https://img.shields.io/badge/HTML5-Parsing-E34F26?logo=html5&logoColor=white)
![License](https://img.shields.io/badge/license-MIT-green)

**Exemplo prático de Web Scraping e parsing de HTML usando a biblioteca JSoup**

</div>

---

## 📋 Índice

- [Sobre o Projeto](#-sobre-o-projeto)
- [O que é JSoup](#-o-que-é-jsoup)
- [Funcionalidades](#-funcionalidades)
- [Tecnologias Utilizadas](#%EF%B8%8F-tecnologias-utilizadas)
- [Pré-requisitos](#-pré-requisitos)
- [Instalação](#-instalação)
- [Executando o Projeto](#%EF%B8%8F-executando-o-projeto)
- [Como Funciona](#-como-funciona)
- [Exemplos de Uso](#-exemplos-de-uso)
- [Casos de Uso](#-casos-de-uso)
- [Seletores CSS](#-seletores-css)
- [Recursos Avançados](#-recursos-avançados)
- [Boas Práticas](#-boas-práticas)
- [Exemplos Práticos Completos](#-exemplos-práticos-completos)
- [Limitações e Considerações](#%EF%B8%8F-limitações-e-considerações)
- [Troubleshooting](#-troubleshooting)
- [Recursos Adicionais](#-recursos-adicionais)
- [Contribuindo](#-contribuindo)
- [Licença](#-licença)
- [Autor](#%E2%80%8D-autor)

---

## 📖 Sobre o Projeto

Este projeto é um **exemplo prático** de uso da biblioteca **JSoup** em Java para realizar **web scraping** e **parsing de HTML**. A aplicação demonstra como extrair dados de páginas web de forma simples e eficiente.

### 🎯 Objetivos

- 🕸️ Demonstrar web scraping básico com JSoup
- 📄 Ensinar parsing e manipulação de documentos HTML
- 🔍 Mostrar uso de seletores CSS para encontrar elementos
- 💡 Fornecer base para projetos de extração de dados
- 📚 Servir como material de estudo para iniciantes

### 🌟 O que o Projeto Faz

O exemplo conecta-se à URL `https://try.jsoup.org`, extrai todos os elementos HTML com a tag `<b>` (negrito) e imprime o texto contido neles no console.

**Fluxo:**
```
URL → Conectar → Baixar HTML → Parsear → Selecionar elementos → Extrair texto → Exibir
```

---

## 🤔 O que é JSoup

### Descrição

**JSoup** é uma biblioteca Java de código aberto projetada para trabalhar com HTML da vida real. Ela fornece uma API muito conveniente para:

- 📥 **Buscar e parsear** HTML de URLs, arquivos ou strings
- 🔍 **Encontrar e extrair** dados usando seletores CSS ou traversing DOM
- 🛠️ **Manipular** HTML (adicionar, remover, modificar elementos)
- 🧹 **Limpar** HTML de entrada de usuários (prevenir XSS)
- 📝 **Gerar** HTML bem formatado

### Características Principais

- ✅ **Simples de usar** - API intuitiva semelhante ao jQuery
- ✅ **Robusta** - Trata HTML malformado
- ✅ **Poderosa** - Seletores CSS completos
- ✅ **Leve** - Sem dependências externas
- ✅ **Open Source** - MIT License
- ✅ **Bem documentada** - Excelente documentação oficial

### Por que Usar JSoup?

| Necessidade | Solução JSoup |
|-------------|---------------|
| Extrair dados de sites | Scraping fácil e eficiente |
| Validar HTML | Parse e validação automática |
| Limpar HTML de usuários | Whitelist-based sanitizer |
| Manipular DOM | API similar ao jQuery |
| Trabalhar com XML | Suporta também XML |

---

## ✨ Funcionalidades

### Implementadas no Projeto

- ✅ **Conexão HTTP** - Conectar a URLs e baixar conteúdo
- ✅ **Parsing HTML** - Converter HTML em Document Object Model
- ✅ **Seleção de Elementos** - Usar seletores CSS (`select("b")`)
- ✅ **Extração de Texto** - Obter texto de elementos
- ✅ **Iteração** - Percorrer coleção de elementos
- ✅ **Tratamento de Exceções** - Gerenciar erros de conexão

### Recursos JSoup Disponíveis

- 🔗 **Conectar a URLs** - `Jsoup.connect(url)`
- 📄 **Parsear HTML** - `Jsoup.parse(html)`
- 📁 **Ler arquivos** - `Jsoup.parse(file, charset)`
- 🔍 **Seletores CSS** - `doc.select("div.class")`
- 🎯 **Encontrar por ID** - `doc.getElementById("id")`
- 🏷️ **Encontrar por tag** - `doc.getElementsByTag("a")`
- 📊 **Atributos** - `element.attr("href")`
- 📝 **Texto** - `element.text()`, `element.html()`
- ✏️ **Manipulação** - Adicionar, remover, modificar elementos
- 🧹 **Sanitização** - `Jsoup.clean(html, whitelist)`

---

## 🛠️ Tecnologias Utilizadas

### Linguagem e Framework

- **[Java 7+](https://www.oracle.com/java/)** - Linguagem de programação
  - Compatível com Java 7, 8, 11, 17+
  - Orientada a objetos

### Biblioteca Principal

- **[JSoup 1.14.2+](https://jsoup.org/)** - HTML parser
  - Web scraping
  - Parsing de HTML/XML
  - Manipulação de DOM
  - Sanitização de HTML

### Build Tool

- **[Maven 3.7+](https://maven.apache.org/)** - Gerenciamento de dependências
  - Build automation
  - Dependency management
  - Lifecycle management

### Ferramentas de Desenvolvimento

- **Eclipse** - Arquivo `.classpath` e `.project` incluídos
- **IntelliJ IDEA** - Arquivo `.iml` suportado
- **Maven Compiler Plugin 3.7.0** - Compilação Java

---

## 📋 Pré-requisitos

### Software Necessário

- **[Java JDK 7+](https://www.oracle.com/java/technologies/downloads/)** - Kit de desenvolvimento Java
  - Recomendado: Java 8 ou superior
  - OpenJDK ou Oracle JDK

- **[Maven 3.6+](https://maven.apache.org/download.cgi)** - Build tool
  - Para gerenciar dependências
  - Para compilar e executar

### Opcional

- **IDE:** Eclipse, IntelliJ IDEA ou VS Code
- **Git** - Para clonar repositório

### Verificar Instalações

```bash
# Verificar Java
java -version

# Verificar Maven
mvn -version

# Saída esperada
# Java version "1.8.0_xxx" ou superior
# Apache Maven 3.x.x
```

---

## 🚀 Instalação

### 1. Obter o Projeto

```bash
# Clonar repositório
git clone <url-do-repositorio>
cd jsoup-example-master

# Ou extrair ZIP
unzip jsoup-example-master.zip
cd jsoup-example-master
```

### 2. Instalar Dependências

```bash
# Maven baixará automaticamente o JSoup
mvn clean install
```

### 3. Verificar Estrutura

```bash
# Verificar que tudo está OK
ls -la
# Deve ver: pom.xml, src/, README.md
```

---

## ▶️ Executando o Projeto

### Método 1: Maven

```bash
# Compilar e executar
mvn clean compile exec:java -Dexec.mainClass="Main"

# Ou compilar primeiro, depois executar
mvn clean package
java -cp target/jsoup-example-0.0.1-SNAPSHOT.jar Main
```

### Método 2: IDE

#### Eclipse
1. **Importar projeto:**
   - File → Import → Existing Maven Projects
   - Selecionar pasta do projeto
   - Finish

2. **Executar:**
   - Botão direito em `Main.java`
   - Run As → Java Application
   - Ver saída no Console

#### IntelliJ IDEA
1. **Abrir projeto:**
   - File → Open → Selecionar pasta
   - Aguardar indexação Maven

2. **Executar:**
   - Abrir `Main.java`
   - Clicar no ícone ▶️ ao lado do método main
   - Ou usar `Shift + F10`

#### VS Code
1. **Abrir pasta:**
   - File → Open Folder

2. **Instalar extensões:**
   - Extension Pack for Java (Microsoft)

3. **Executar:**
   - Clicar em "Run" acima do método main

### Método 3: Linha de Comando (Sem Maven)

```bash
# Baixar JSoup manualmente
wget https://repo1.maven.org/maven2/org/jsoup/jsoup/1.14.2/jsoup-1.14.2.jar

# Compilar
javac -cp jsoup-1.14.2.jar src/Main.java

# Executar
java -cp ".:jsoup-1.14.2.jar:src" Main
```

### Saída Esperada

```
Elementos com a tag <b>:
JSoup
HTML parser
[Textos em negrito da página]
```

---

## 🔍 Como Funciona

### Código Passo a Passo

```java
import org.jsoup.Jsoup;
import org.jsoup.nodes.Document;
import org.jsoup.nodes.Element;
import org.jsoup.select.Elements;

public class Main {
    public static void main(String[] args) {
        
        // 1. Definir URL alvo
        String url = "https://try.jsoup.org";
        
        try {
            // 2. Conectar e baixar HTML
            Document doc = Jsoup.connect(url).get();
            
            // 3. Selecionar elementos usando seletor CSS
            Elements elementosTag = doc.select("b");
            
            // 4. Exibir mensagem
            System.out.println("Elementos com a tag <b>:");
            
            // 5. Iterar e extrair texto
            for(Element el: elementosTag) {
                System.out.println(el.text());
            }
            
        } catch (IOException e) {
            e.printStackTrace();
        }
    }
}
```

### Explicação Detalhada

#### 1. Conexão HTTP
```java
Document doc = Jsoup.connect(url).get();
```
- Conecta à URL especificada
- Faz requisição HTTP GET
- Baixa o HTML da página
- Parseia e retorna um objeto `Document`

#### 2. Seleção de Elementos
```java
Elements elementosTag = doc.select("b");
```
- Usa seletor CSS para encontrar elementos
- `"b"` seleciona todas as tags `<b>` (negrito)
- Retorna uma coleção `Elements`

#### 3. Extração de Dados
```java
for(Element el: elementosTag) {
    System.out.println(el.text());
}
```
- Itera sobre cada elemento encontrado
- `.text()` extrai apenas o texto (sem tags HTML)
- Imprime no console

---

## 📝 Exemplos de Uso

### Exemplo 1: Extrair Links

```java
import org.jsoup.Jsoup;
import org.jsoup.nodes.Document;
import org.jsoup.nodes.Element;
import org.jsoup.select.Elements;

public class ExtrairLinks {
    public static void main(String[] args) throws IOException {
        
        String url = "https://www.exemplo.com";
        Document doc = Jsoup.connect(url).get();
        
        // Selecionar todos os links
        Elements links = doc.select("a[href]");
        
        System.out.println("Links encontrados:");
        for (Element link : links) {
            String href = link.attr("href");      // URL do link
            String texto = link.text();            // Texto do link
            System.out.println("Texto: " + texto + " | URL: " + href);
        }
    }
}
```

### Exemplo 2: Extrair Imagens

```java
public class ExtrairImagens {
    public static void main(String[] args) throws IOException {
        
        String url = "https://www.exemplo.com";
        Document doc = Jsoup.connect(url).get();
        
        // Selecionar todas as imagens
        Elements imagens = doc.select("img[src]");
        
        System.out.println("Imagens encontradas:");
        for (Element img : imagens) {
            String src = img.attr("abs:src");     // URL absoluta
            String alt = img.attr("alt");         // Texto alternativo
            System.out.println("ALT: " + alt + " | SRC: " + src);
        }
    }
}
```

### Exemplo 3: Extrair Tabela HTML

```java
public class ExtrairTabela {
    public static void main(String[] args) throws IOException {
        
        String url = "https://www.exemplo.com/tabela";
        Document doc = Jsoup.connect(url).get();
        
        // Selecionar primeira tabela
        Element tabela = doc.select("table").first();
        
        if (tabela != null) {
            // Linhas da tabela
            Elements linhas = tabela.select("tr");
            
            for (Element linha : linhas) {
                // Células da linha
                Elements celulas = linha.select("td, th");
                
                for (Element celula : celulas) {
                    System.out.print(celula.text() + "\t");
                }
                System.out.println();
            }
        }
    }
}
```

### Exemplo 4: Extrair Metadados

```java
public class ExtrairMetadados {
    public static void main(String[] args) throws IOException {
        
        String url = "https://www.exemplo.com";
        Document doc = Jsoup.connect(url).get();
        
        // Título da página
        String titulo = doc.title();
        
        // Meta description
        String description = doc.select("meta[name=description]")
                               .attr("content");
        
        // Meta keywords
        String keywords = doc.select("meta[name=keywords]")
                            .attr("content");
        
        System.out.println("Título: " + titulo);
        System.out.println("Descrição: " + description);
        System.out.println("Keywords: " + keywords);
    }
}
```

### Exemplo 5: Extrair Notícias de Site

```java
public class ExtrairNoticias {
    public static void main(String[] args) throws IOException {
        
        String url = "https://www.exemplo-noticias.com";
        Document doc = Jsoup.connect(url).get();
        
        // Selecionar artigos de notícias
        Elements noticias = doc.select("article.noticia");
        
        for (Element noticia : noticias) {
            String titulo = noticia.select("h2.titulo").text();
            String resumo = noticia.select("p.resumo").text();
            String link = noticia.select("a").attr("href");
            String data = noticia.select("time").attr("datetime");
            
            System.out.println("Título: " + titulo);
            System.out.println("Resumo: " + resumo);
            System.out.println("Link: " + link);
            System.out.println("Data: " + data);
            System.out.println("---");
        }
    }
}
```

---

## 🎯 Casos de Uso

### 1. Monitoramento de Preços 💰

Extrair preços de produtos de e-commerce para comparação:

```java
public class MonitoramentoPrecos {
    public static void main(String[] args) throws IOException {
        String url = "https://www.loja.com/produto";
        Document doc = Jsoup.connect(url).get();
        
        String preco = doc.select(".preco-principal").text();
        String produto = doc.select("h1.nome-produto").text();
        
        System.out.println(produto + ": R$ " + preco);
    }
}
```

**Aplicações:**
- Comparador de preços
- Alertas de promoção
- Histórico de variação de preço

### 2. Agregador de Notícias 📰

Coletar manchetes de múltiplos sites:

```java
public class AgregadorNoticias {
    public static void main(String[] args) throws IOException {
        String[] sites = {
            "https://g1.globo.com",
            "https://www.uol.com.br",
            "https://www.folha.com.br"
        };
        
        for (String site : sites) {
            Document doc = Jsoup.connect(site).get();
            Elements manchetes = doc.select("h2.manchete");
            
            System.out.println("Manchetes de " + site + ":");
            manchetes.forEach(m -> System.out.println("- " + m.text()));
        }
    }
}
```

### 3. Validação de SEO 🔍

Verificar elementos importantes para SEO:

```java
public class ValidadorSEO {
    public static void main(String[] args) throws IOException {
        String url = "https://www.meusite.com";
        Document doc = Jsoup.connect(url).get();
        
        // Verificações SEO
        System.out.println("Título: " + doc.title() + 
            " (tamanho: " + doc.title().length() + ")");
        
        System.out.println("Meta description: " + 
            doc.select("meta[name=description]").attr("content"));
        
        System.out.println("H1s: " + doc.select("h1").size());
        System.out.println("Links internos: " + 
            doc.select("a[href^=/]").size());
        System.out.println("Links externos: " + 
            doc.select("a[href^=http]").size());
        System.out.println("Imagens sem ALT: " + 
            doc.select("img:not([alt])").size());
    }
}
```

### 4. Extração de Dados Estruturados 📊

Extrair dados de tabelas para análise:

```java
public class ExtratorDados {
    public static void main(String[] args) throws IOException {
        String url = "https://www.exemplo.com/dados";
        Document doc = Jsoup.connect(url).get();
        
        // Criar CSV
        Elements linhas = doc.select("table#dados tr");
        
        for (Element linha : linhas) {
            Elements colunas = linha.select("td");
            String csv = colunas.stream()
                .map(Element::text)
                .collect(Collectors.joining(","));
            System.out.println(csv);
        }
    }
}
```

### 5. Monitoramento de Vagas 💼

Coletar vagas de emprego de sites:

```java
public class MonitoradorVagas {
    public static void main(String[] args) throws IOException {
        String url = "https://www.emprego.com/vagas/java";
        Document doc = Jsoup.connect(url).get();
        
        Elements vagas = doc.select("div.vaga");
        
        for (Element vaga : vagas) {
            String titulo = vaga.select("h3.titulo-vaga").text();
            String empresa = vaga.select("span.empresa").text();
            String local = vaga.select("span.localizacao").text();
            String link = vaga.select("a").attr("abs:href");
            
            System.out.println(titulo + " - " + empresa + " (" + local + ")");
            System.out.println("Link: " + link);
            System.out.println();
        }
    }
}
```

---

## 🎨 Seletores CSS

JSoup suporta a maioria dos seletores CSS. Aqui estão os mais comuns:

### Seletores Básicos

| Seletor | Exemplo | Descrição |
|---------|---------|-----------|
| `tag` | `doc.select("p")` | Seleciona todas as tags `<p>` |
| `#id` | `doc.select("#main")` | Seleciona elemento com id="main" |
| `.class` | `doc.select(".destaque")` | Seleciona elementos com class="destaque" |
| `*` | `doc.select("*")` | Seleciona todos os elementos |

### Seletores Combinados

| Seletor | Exemplo | Descrição |
|---------|---------|-----------|
| `el1 el2` | `doc.select("div p")` | `<p>` dentro de `<div>` (descendente) |
| `el1 > el2` | `doc.select("div > p")` | `<p>` filho direto de `<div>` |
| `el1 + el2` | `doc.select("h1 + p")` | `<p>` imediatamente após `<h1>` |
| `el1, el2` | `doc.select("h1, h2, h3")` | Múltiplos seletores |

### Seletores de Atributo

| Seletor | Exemplo | Descrição |
|---------|---------|-----------|
| `[attr]` | `doc.select("a[href]")` | Tem atributo href |
| `[attr=value]` | `doc.select("a[href=/]")` | href igual a "/" |
| `[attr^=value]` | `doc.select("a[href^=http]")` | href começa com "http" |
| `[attr$=value]` | `doc.select("img[src$=.png]")` | src termina com ".png" |
| `[attr*=value]` | `doc.select("a[href*=google]")` | href contém "google" |

### Pseudo-seletores

| Seletor | Exemplo | Descrição |
|---------|---------|-----------|
| `:first-child` | `doc.select("li:first-child")` | Primeiro filho |
| `:last-child` | `doc.select("li:last-child")` | Último filho |
| `:nth-child(n)` | `doc.select("tr:nth-child(2)")` | N-ésimo filho |
| `:not(selector)` | `doc.select("div:not(.ignore)")` | Negação |
| `:has(selector)` | `doc.select("div:has(p)")` | Contém `<p>` |
| `:contains(text)` | `doc.select("p:contains(Java)")` | Contém texto "Java" |

### Exemplos Práticos de Seletores

```java
// Selecionar todos os parágrafos com classe "destaque"
Elements p = doc.select("p.destaque");

// Selecionar links externos
Elements linksExternos = doc.select("a[href^=http]");

// Selecionar primeira imagem
Element primeiraImg = doc.select("img").first();

// Selecionar div com id "conteudo"
Element conteudo = doc.selectFirst("#conteudo");

// Selecionar todos os inputs type=text
Elements inputs = doc.select("input[type=text]");

// Selecionar elementos que contêm texto específico
Elements elementos = doc.select("*:contains(Java)");

// Selecionar elementos irmãos
Elements irmãos = doc.select("h1 ~ p");
```

---

## 🚀 Recursos Avançados

### 1. Configurações de Conexão

```java
// Timeout personalizado
Document doc = Jsoup.connect(url)
    .timeout(5000)  // 5 segundos
    .get();

// User-Agent customizado
Document doc = Jsoup.connect(url)
    .userAgent("Mozilla/5.0 (Windows NT 10.0; Win64; x64)")
    .get();

// Seguir redirects
Document doc = Jsoup.connect(url)
    .followRedirects(true)
    .get();

// Cookies
Document doc = Jsoup.connect(url)
    .cookie("auth", "token123")
    .get();

// Headers customizados
Document doc = Jsoup.connect(url)
    .header("Accept", "text/html")
    .header("Accept-Language", "pt-BR")
    .get();

// POST request
Document doc = Jsoup.connect(url)
    .data("username", "admin")
    .data("password", "pass")
    .post();

// Configuração completa
Document doc = Jsoup.connect(url)
    .userAgent("Mozilla/5.0")
    .timeout(10000)
    .followRedirects(true)
    .referrer("https://www.google.com")
    .ignoreHttpErrors(true)
    .get();
```

### 2. Manipulação de Elementos

```java
// Adicionar classe
element.addClass("nova-classe");

// Remover classe
element.removeClass("classe-antiga");

// Modificar atributo
element.attr("href", "https://novo-link.com");

// Modificar texto
element.text("Novo texto");

// Modificar HTML interno
element.html("<p>Novo conteúdo HTML</p>");

// Adicionar elemento filho
element.append("<span>Texto adicional</span>");

// Remover elemento
element.remove();

// Substituir elemento
element.replaceWith(novoElement);
```

### 3. Navegação no DOM

```java
// Elemento pai
Element pai = element.parent();

// Elementos filhos
Elements filhos = element.children();

// Primeiro filho
Element primeiroFilho = element.child(0);

// Elementos irmãos
Elements irmaos = element.siblingElements();

// Próximo irmão
Element proximo = element.nextElementSibling();

// Irmão anterior
Element anterior = element.previousElementSibling();

// Percorrer árvore
for (Element filho : element.getAllElements()) {
    System.out.println(filho.tagName());
}
```

### 4. Extração de Dados

```java
// Texto limpo (sem HTML)
String texto = element.text();

// HTML interno
String html = element.html();

// HTML completo (incluindo a tag)
String htmlCompleto = element.outerHtml();

// Texto próprio (sem filhos)
String textoProprio = element.ownText();

// Atributo
String valor = element.attr("href");

// Atributo absoluto (resolve URLs relativas)
String urlAbsoluta = element.attr("abs:href");

// Verificar se tem atributo
boolean temHref = element.hasAttr("href");

// Verificar se tem texto
boolean temTexto = element.hasText();

// Dados especiais
String data = element.data();  // Para tags <script>, <style>
```

### 5. Validação e Limpeza de HTML

```java
import org.jsoup.safety.Safelist;

// Limpar HTML de entrada de usuário (prevenir XSS)
String htmlUsuario = "<p>Texto seguro</p><script>alert('XSS')</script>";
String htmlLimpo = Jsoup.clean(htmlUsuario, Safelist.basic());
System.out.println(htmlLimpo);  // "<p>Texto seguro</p>"

// Whitelist personalizada
Safelist whitelist = new Safelist()
    .addTags("p", "b", "i", "u", "a")
    .addAttributes("a", "href");

String limpo = Jsoup.clean(htmlUsuario, whitelist);

// Diferentes níveis de limpeza
Jsoup.clean(html, Safelist.none());          // Remove todas as tags
Jsoup.clean(html, Safelist.simpleText());    // Apenas texto, br e p
Jsoup.clean(html, Safelist.basic());         // Tags básicas de formatação
Jsoup.clean(html, Safelist.basicWithImages());  // + imagens
Jsoup.clean(html, Safelist.relaxed());       // Mais permissivo
```

### 6. Parsear HTML de Diferentes Fontes

```java
// De URL
Document doc = Jsoup.connect("https://exemplo.com").get();

// De String HTML
String html = "<html><body><p>Teste</p></body></html>";
Document doc = Jsoup.parse(html);

// De arquivo local
File arquivo = new File("pagina.html");
Document doc = Jsoup.parse(arquivo, "UTF-8");

// De InputStream
InputStream stream = new FileInputStream("pagina.html");
Document doc = Jsoup.parse(stream, "UTF-8", "https://exemplo.com");

// De fragmento HTML
String fragmento = "<div><p>Fragmento</p></div>";
Document doc = Jsoup.parseBodyFragment(fragmento);

// XML (não HTML)
Document doc = Jsoup.parse(xml, "", Parser.xmlParser());
```

---

## 📚 Estrutura do Código

### Hierarquia de Classes JSoup

```
Document (extends Element)
    ├── head()
    ├── body()
    └── select(String cssQuery)
        └── Elements (extends ArrayList<Element>)
            └── Element
                ├── text()
                ├── html()
                ├── attr(String)
                ├── select(String)
                └── children()
```

### Principais Classes

| Classe | Descrição | Uso Principal |
|--------|-----------|---------------|
| `Jsoup` | Classe de entrada | Conectar, parsear, limpar |
| `Document` | Documento HTML completo | Raiz do DOM |
| `Element` | Elemento HTML | Manipular tags |
| `Elements` | Coleção de elementos | Iterar, filtrar |
| `Connection` | Configurar requisição HTTP | Headers, cookies, timeout |
| `Safelist` | Whitelist de HTML | Sanitização |

---

## 🎓 Boas Práticas

### 1. Tratamento de Exceções

```java
// ✅ Bom - Tratar exceções específicas
try {
    Document doc = Jsoup.connect(url).get();
    // processar
} catch (IOException e) {
    System.err.println("Erro ao conectar: " + e.getMessage());
    // Logging apropriado
    logger.error("Falha ao acessar URL: {}", url, e);
}

// ❌ Evitar - Ignorar exceções
try {
    Document doc = Jsoup.connect(url).get();
} catch (Exception e) {
    // Vazio - nunca faça isso!
}
```

### 2. Verificar Existência de Elementos

```java
// ✅ Bom - Verificar antes de usar
Element elemento = doc.selectFirst("div.conteudo");
if (elemento != null) {
    String texto = elemento.text();
    System.out.println(texto);
}

// ✅ Melhor ainda - Optional (Java 8+)
Optional.ofNullable(doc.selectFirst("div.conteudo"))
    .map(Element::text)
    .ifPresent(System.out::println);

// ❌ Evitar - Pode causar NullPointerException
String texto = doc.selectFirst("div.conteudo").text();
```

### 3. Configurar Timeout

```java
// ✅ Sempre definir timeout
Document doc = Jsoup.connect(url)
    .timeout(10 * 1000)  // 10 segundos
    .get();

// Para sites lentos
Document doc = Jsoup.connect(url)
    .timeout(30 * 1000)  // 30 segundos
    .get();
```

### 4. Respeitar robots.txt

```java
// Verificar se scraping é permitido
// 1. Ler robots.txt do site
// 2. Respeitar delay entre requisições
// 3. Usar User-Agent identificável

Thread.sleep(1000);  // Esperar 1 segundo entre requisições
```

### 5. Cache Local

```java
// Evitar requisições desnecessárias
public class CacheHTML {
    private Map<String, Document> cache = new HashMap<>();
    
    public Document getDocument(String url) throws IOException {
        if (!cache.containsKey(url)) {
            Document doc = Jsoup.connect(url).get();
            cache.put(url, doc);
        }
        return cache.get(url);
    }
}
```

---

## 🔧 Recursos Úteis do JSoup

### Trabalhar com Formulários

```java
// Preencher e submeter formulário
Document loginPage = Jsoup.connect("https://site.com/login").get();

Connection.Response response = Jsoup.connect("https://site.com/login")
    .data("username", "usuario")
    .data("password", "senha")
    .cookies(loginPage.cookies())
    .method(Connection.Method.POST)
    .execute();

Document loggedIn = response.parse();
```

### Download de Arquivos

```java
// Obter resposta como bytes (para imagens, PDFs, etc)
Connection.Response response = Jsoup.connect("https://site.com/arquivo.pdf")
    .ignoreContentType(true)
    .execute();

byte[] bytes = response.bodyAsBytes();

// Salvar em arquivo
FileOutputStream fos = new FileOutputStream("arquivo.pdf");
fos.write(bytes);
fos.close();
```

### Trabalhar com JSON em HTML

```java
// Extrair JSON de tag <script>
Element scriptTag = doc.select("script#json-data").first();
if (scriptTag != null) {
    String json = scriptTag.data();
    // Parsear JSON com biblioteca apropriada (Gson, Jackson)
}
```

### Preservar Formatação

```java
// Preservar quebras de linha
Document doc = Jsoup.parse(html);
doc.outputSettings().prettyPrint(false);
String htmlSemFormatacao = doc.html();
```

---

## 📊 Exemplos Práticos Completos

### Scraper de E-commerce

```java
import org.jsoup.Jsoup;
import org.jsoup.nodes.Document;
import org.jsoup.nodes.Element;
import org.jsoup.select.Elements;
import java.io.IOException;
import java.util.ArrayList;
import java.util.List;

public class EcommerceScraper {
    
    static class Produto {
        String nome;
        String preco;
        String imagem;
        String link;
        
        @Override
        public String toString() {
            return String.format("%s - %s (%s)", nome, preco, link);
        }
    }
    
    public static List<Produto> extrairProdutos(String url) throws IOException {
        List<Produto> produtos = new ArrayList<>();
        
        Document doc = Jsoup.connect(url)
            .userAgent("Mozilla/5.0")
            .timeout(10000)
            .get();
        
        Elements items = doc.select("div.produto");
        
        for (Element item : items) {
            Produto p = new Produto();
            p.nome = item.select("h3.nome").text();
            p.preco = item.select("span.preco").text();
            p.imagem = item.select("img").attr("abs:src");
            p.link = item.select("a").attr("abs:href");
            
            produtos.add(p);
        }
        
        return produtos;
    }
    
    public static void main(String[] args) throws IOException {
        String url = "https://www.loja.com/produtos";
        List<Produto> produtos = extrairProdutos(url);
        
        produtos.forEach(System.out::println);
    }
}
```

### Extrator de Artigos de Blog

```java
import org.jsoup.Jsoup;
import org.jsoup.nodes.Document;
import org.jsoup.nodes.Element;
import org.jsoup.select.Elements;
import java.io.IOException;
import java.time.LocalDate;

public class BlogScraper {
    
    static class Artigo {
        String titulo;
        String autor;
        LocalDate data;
        String resumo;
        String url;
    }
    
    public static void extrairArtigos(String blogUrl) throws IOException {
        Document doc = Jsoup.connect(blogUrl).get();
        Elements artigos = doc.select("article");
        
        for (Element artigo : artigos) {
            String titulo = artigo.select("h2.titulo").text();
            String autor = artigo.select("span.autor").text();
            String data = artigo.select("time").attr("datetime");
            String resumo = artigo.select("p.resumo").text();
            String link = artigo.select("a.ler-mais").attr("abs:href");
            
            System.out.println("=== " + titulo + " ===");
            System.out.println("Autor: " + autor);
            System.out.println("Data: " + data);
            System.out.println("Resumo: " + resumo);
            System.out.println("Link: " + link);
            System.out.println();
        }
    }
    
    public static void main(String[] args) throws IOException {
        extrairArtigos("https://blog.exemplo.com");
    }
}
```

### Verificador de Links Quebrados

```java
import org.jsoup.Jsoup;
import org.jsoup.nodes.Document;
import org.jsoup.select.Elements;
import java.io.IOException;

public class LinkChecker {
    
    public static void verificarLinks(String url) throws IOException {
        Document doc = Jsoup.connect(url).get();
        Elements links = doc.select("a[href]");
        
        System.out.println("Verificando " + links.size() + " links...\n");
        
        for (Element link : links) {
            String href = link.attr("abs:href");
            
            try {
                int statusCode = Jsoup.connect(href)
                    .timeout(5000)
                    .ignoreContentType(true)
                    .execute()
                    .statusCode();
                
                if (statusCode == 200) {
                    System.out.println("✅ OK: " + href);
                } else {
                    System.out.println("⚠️  " + statusCode + ": " + href);
                }
                
            } catch (IOException e) {
                System.out.println("❌ ERRO: " + href + " (" + e.getMessage() + ")");
            }
            
            // Delay entre requisições
            Thread.sleep(500);
        }
    }
    
    public static void main(String[] args) throws Exception {
        verificarLinks("https://www.meusite.com");
    }
}
```

---

## ⚖️ Limitações e Considerações

### Aspectos Legais

> ⚠️ **IMPORTANTE:** Web scraping pode ter implicações legais.

**Antes de fazer scraping:**

1. **Verificar Termos de Serviço** - Muitos sites proíbem scraping nos ToS
2. **Consultar robots.txt** - Respeitar diretrizes: `https://site.com/robots.txt`
3. **Uso Ético** - Não sobrecarregar servidores
4. **Dados Pessoais** - Respeitar LGPD/GDPR
5. **Copyright** - Não violar direitos autorais

### Limitações Técnicas

❌ **JSoup NÃO executa JavaScript**
- Não funciona com sites SPA (React, Angular, Vue)
- Não carrega conteúdo dinâmico via AJAX
- Para esses casos, use: Selenium, Puppeteer, Playwright

✅ **JSoup É IDEAL para:**
- HTML estático
- Páginas server-side rendered
- Extração de metadados
- Parsing de HTML local

### Boas Práticas de Scraping

```java
public class ScraperEtico {
    
    private static final int DELAY_MS = 1000;  // 1 segundo entre requisições
    private static final String USER_AGENT = "MeuScraper/1.0 (contato@email.com)";
    
    public static Document baixarPagina(String url) throws IOException {
        // Delay para não sobrecarregar servidor
        Thread.sleep(DELAY_MS);
        
        return Jsoup.connect(url)
            .userAgent(USER_AGENT)  // Identificação
            .timeout(10000)
            .followRedirects(true)
            .get();
    }
}
```

---

## 🐛 Troubleshooting

### Erro: Connection timeout

**Problema:** Timeout ao conectar

**Solução:**
```java
// Aumentar timeout
Document doc = Jsoup.connect(url)
    .timeout(30 * 1000)  // 30 segundos
    .get();
```

### Erro: 403 Forbidden

**Problema:** Site bloqueia requisição

**Solução:**
```java
// Adicionar User-Agent
Document doc = Jsoup.connect(url)
    .userAgent("Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36")
    .referrer("https://www.google.com")
    .get();
```

### Erro: SSL/Certificate

**Problema:** Erro de certificado SSL

**Solução:**
```java
// Ignorar validação SSL (apenas para desenvolvimento!)
Document doc = Jsoup.connect(url)
    .validateTLSCertificates(false)
    .get();
```

### Elementos não encontrados

**Problema:** Seletor não retorna elementos

**Solução:**
```java
// Debug: Imprimir HTML para ver estrutura
System.out.println(doc.html());

// Ou salvar em arquivo
try (FileWriter fw = new FileWriter("debug.html")) {
    fw.write(doc.html());
}

// Verificar seletores passo a passo
System.out.println("Divs: " + doc.select("div").size());
System.out.println("Com classe: " + doc.select("div.conteudo").size());
```

### Encoding incorreto

**Problema:** Caracteres especiais aparecem errados

**Solução:**
```java
// Especificar charset
Document doc = Jsoup.connect(url)
    .get();
doc.charset(Charset.forName("UTF-8"));

// Ou ao parsear arquivo
Document doc = Jsoup.parse(file, "UTF-8");
```

---

## 📦 Dependências Maven

### pom.xml Completo

```xml
<?xml version="1.0" encoding="UTF-8"?>
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 
         http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>
    
    <groupId>jsoup-example</groupId>
    <artifactId>jsoup-example</artifactId>
    <version>0.0.1-SNAPSHOT</version>
    
    <properties>
        <maven.compiler.source>1.8</maven.compiler.source>
        <maven.compiler.target>1.8</maven.compiler.target>
        <project.build.sourceEncoding>UTF-8</project.build.sourceEncoding>
    </properties>
    
    <dependencies>
        <!-- JSoup -->
        <dependency>
            <groupId>org.jsoup</groupId>
            <artifactId>jsoup</artifactId>
            <version>1.15.3</version>
        </dependency>
        
        <!-- SLF4J para logging (opcional) -->
        <dependency>
            <groupId>org.slf4j</groupId>
            <artifactId>slf4j-simple</artifactId>
            <version>1.7.36</version>
        </dependency>
    </dependencies>
    
    <build>
        <sourceDirectory>src</sourceDirectory>
        <plugins>
            <plugin>
                <artifactId>maven-compiler-plugin</artifactId>
                <version>3.8.1</version>
                <configuration>
                    <source>1.8</source>
                    <target>1.8</target>
                </configuration>
            </plugin>
        </plugins>
    </build>
</project>
```

---

## 🔍 Projetos Avançados Sugeridos

### 1. Agregador de Notícias

**Objetivo:** Coletar notícias de múltiplos portais

**Features:**
- Extrair manchetes de vários sites
- Salvar em banco de dados
- Agendar execução periódica (Quartz)
- Detectar duplicatas
- Gerar RSS feed

### 2. Monitorador de Preços

**Objetivo:** Rastrear preços de produtos

**Features:**
- Extrair preço de produto específico
- Armazenar histórico de preços
- Enviar alerta por email quando preço cair
- Gráfico de variação de preço
- Comparar entre lojas

### 3. Extrator de Vagas de Emprego

**Objetivo:** Centralizar vagas de emprego

**Features:**
- Extrair vagas de múltiplos sites
- Filtrar por tecnologia/localização
- Remover duplicatas
- Notificar novas vagas
- Exportar para planilha

### 4. Gerador de Metadados SEO

**Objetivo:** Analisar SEO de sites

**Features:**
- Extrair title, meta description, keywords
- Verificar H1, H2, H3
- Analisar links internos/externos
- Verificar imagens sem ALT
- Gerar relatório de SEO

### 5. Web Crawler Completo

**Objetivo:** Indexar site completo

**Features:**
- Seguir todos os links recursivamente
- Criar mapa do site (sitemap)
- Detectar links quebrados
- Extrair todo o conteúdo
- Criar índice de busca

---

## 📚 Recursos Adicionais

### Documentação Oficial

- **[JSoup Official Website](https://jsoup.org/)** - Site oficial
- **[JSoup Cookbook](https://jsoup.org/cookbook/)** - Receitas práticas
- **[JSoup API JavaDoc](https://jsoup.org/apidocs/)** - Documentação completa da API
- **[GitHub Repository](https://github.com/jhy/jsoup)** - Código fonte

### Tutoriais

- [JSoup Tutorial - Baeldung](https://www.baeldung.com/java-with-jsoup)
- [Web Scraping with Java and JSoup](https://www.scrapingbee.com/blog/web-scraping-java/)
- [JSoup Examples - JavaCodeGeeks](https://www.javacodegeeks.com/)

### Livros

- "Web Scraping with Java" - Kevin Sahin
- "Java Network Programming" - Elliotte Rusty Harold
- "Instant Jsoup How-to" - Pete Houston

### Cursos

- Udemy - Web Scraping com Java
- Pluralsight - Web Scraping Fundamentals
- YouTube - Múltiplos tutoriais em português

### Alternativas ao JSoup

| Biblioteca | Linguagem | Quando Usar |
|------------|-----------|-------------|
| **Selenium** | Java/Python | Sites com JavaScript |
| **HtmlUnit** | Java | Browser headless, JS suportado |
| **Scrapy** | Python | Projetos grandes de scraping |
| **Puppeteer** | JavaScript | Controle completo do Chrome |
| **BeautifulSoup** | Python | Parsing HTML simples |

---

## 🎯 Casos de Uso Reais

### Empresas que Usam Web Scraping

- 🔍 **Google** - Indexar páginas web
- 💰 **Comparadores de preço** - Monitorar preços
- 📰 **Agregadores de notícias** - Coletar manchetes
- 📊 **Empresas de pesquisa** - Coletar dados públicos
- 🏢 **Recrutadores** - Coletar vagas de emprego

### Aplicações Profissionais

1. **Business Intelligence**
   - Monitorar concorrência
   - Análise de mercado
   - Tendências de preço

2. **Pesquisa Acadêmica**
   - Coleta de dados para análise
   - Estudos de mercado
   - Análise de conteúdo

3. **Automação**
   - Preenchimento de formulários
   - Monitoramento de sites
   - Alertas automáticos

4. **Data Mining**
   - Extração de dados em larga escala
   - Análise de sentimentos
   - Machine Learning datasets

---

## 🎓 Exercícios Práticos

### Exercício 1: Extrair Títulos

**Objetivo:** Modificar o código para extrair todos os `<h1>`

```java
// Modificar linha:
Elements elementosTag = doc.select("h1");  // Em vez de "b"
```

### Exercício 2: Extrair Links

**Objetivo:** Extrair todos os links com seus textos

```java
Elements links = doc.select("a[href]");
for (Element link : links) {
    System.out.println(link.text() + " -> " + link.attr("href"));
}
```

### Exercício 3: Contar Elementos

**Objetivo:** Contar quantos parágrafos existem na página

```java
int totalParagrafos = doc.select("p").size();
System.out.println("Total de parágrafos: " + totalParagrafos);
```

### Exercício 4: Extrair de Múltiplas Páginas

**Objetivo:** Extrair dados de várias URLs

```java
String[] urls = {
    "https://site1.com",
    "https://site2.com",
    "https://site3.com"
};

for (String url : urls) {
    Document doc = Jsoup.connect(url).get();
    System.out.println("Título: " + doc.title());
    Thread.sleep(1000);  // Delay ético
}
```

### Exercício 5: Salvar HTML em Arquivo

**Objetivo:** Baixar e salvar página completa

```java
Document doc = Jsoup.connect(url).get();

try (FileWriter fw = new FileWriter("pagina.html")) {
    fw.write(doc.html());
}

System.out.println("Página salva com sucesso!");
```

---

## 🛡️ Segurança e Ética

### Práticas Éticas de Web Scraping

1. **Respeitar robots.txt**
   ```
   # Verificar sempre
   https://site.com/robots.txt
   ```

2. **Rate Limiting**
   ```java
   // Esperar entre requisições
   Thread.sleep(1000);  // 1 segundo
   ```

3. **Identificar-se**
   ```java
   .userAgent("MeuScraper/1.0 (contato@email.com)")
   ```

4. **Horários de baixo tráfego**
   - Evitar horários de pico
   - Usar cache quando possível

5. **Respeitar capacidade do servidor**
   - Não fazer milhares de requisições simultâneas
   - Implementar retry com backoff exponencial

### Prevenção de XSS ao Usar Dados

```java
// SEMPRE limpar HTML de fontes externas antes de exibir
String htmlExterno = element.html();
String htmlSeguro = Jsoup.clean(htmlExterno, Safelist.basic());

// Usar em sua aplicação web
```

---

## 📖 Comandos Úteis

### Maven

```bash
# Limpar e compilar
mvn clean compile

# Executar
mvn exec:java -Dexec.mainClass="Main"

# Empacotar
mvn package

# Instalar dependências
mvn dependency:resolve

# Ver árvore de dependências
mvn dependency:tree
```

### Java

```bash
# Compilar manualmente
javac -cp ~/.m2/repository/org/jsoup/jsoup/1.14.2/jsoup-1.14.2.jar src/Main.java

# Executar
java -cp ".:~/.m2/repository/org/jsoup/jsoup/1.14.2/jsoup-1.14.2.jar:src" Main
```

---

## 🚀 Melhorias Sugeridas

### Features

- [ ] Adicionar configuração via arquivo properties
- [ ] Implementar sistema de logs (SLF4J + Logback)
- [ ] Criar classes separadas para diferentes scrapers
- [ ] Adicionar persistência em banco de dados (H2/MySQL)
- [ ] Implementar cache de páginas
- [ ] Adicionar retry automático em falhas
- [ ] Criar interface CLI interativa
- [ ] Exportar dados para CSV/JSON/XML

### Arquitetura

- [ ] Separar em camadas (Scraper, Parser, Storage)
- [ ] Implementar padrão Strategy para diferentes sites
- [ ] Adicionar interface para novos scrapers
- [ ] Criar fábrica de scrapers
- [ ] Implementar Observer para notificações

### DevOps

- [ ] Adicionar Dockerfile
- [ ] Configurar CI/CD (GitHub Actions)
- [ ] Implementar health checks
- [ ] Adicionar métricas (Prometheus)
- [ ] Criar testes automatizados

---

## 🤝 Contribuindo

Contribuições são bem-vindas! Este é um projeto de exemplo e pode ser expandido.

### Como Contribuir

1. Fork o projeto
2. Crie uma branch (`git checkout -b feature/novo-exemplo`)
3. Commit suas mudanças (`git commit -m 'feat: adiciona exemplo de tabelas'`)
4. Push para a branch (`git push origin feature/novo-exemplo`)
5. Abra um Pull Request

### Ideias de Contribuição

- 📝 Adicionar mais exemplos práticos
- 🐛 Corrigir bugs ou melhorar código
- 📚 Melhorar documentação
- 🎨 Criar novos scrapers de exemplo
- ✅ Adicionar testes unitários

---

## 📄 Licença

Este projeto está sob a licença MIT. Veja o arquivo `LICENSE` para mais detalhes.

---

## 👨‍💻 Autor

**Thiago Adelino**

Projeto de exemplo para demonstrar o uso da biblioteca JSoup em Java.

---

## 🙏 Agradecimentos

- **[Jonathan Hedley](https://github.com/jhy)** - Criador e mantenedor do JSoup
- **Comunidade JSoup** - Por contribuições e suporte
- **Comunidade Java** - Por compartilhar conhecimento
- **Stack Overflow** - Por inúmeras soluções

---

## 📊 Estatísticas do Projeto

| Métrica | Valor |
|---------|-------|
| **Linguagem** | Java 7+ |
| **Biblioteca** | JSoup 1.14.2+ |
| **Build Tool** | Maven 3.7+ |
| **Linhas de código** | ~40 linhas |
| **Dependências** | 1 (JSoup) |
| **Complexidade** | Baixa (exemplo didático) |

---

## 🔖 Glossário

| Termo | Descrição |
|-------|-----------|
| **Web Scraping** | Extração automatizada de dados de sites |
| **HTML Parsing** | Análise e interpretação de código HTML |
| **DOM** | Document Object Model - Estrutura em árvore do HTML |
| **CSS Selector** | Padrão para selecionar elementos HTML |
| **Element** | Elemento HTML (tag) |
| **Node** | Nó na árvore DOM |
| **Attribute** | Atributo de uma tag HTML |
| **User-Agent** | Identificação do cliente HTTP |
| **Whitelist** | Lista de elementos HTML permitidos |
| **XSS** | Cross-Site Scripting (vulnerabilidade) |

---

## 🎯 Cheat Sheet JSoup

### Conexão e Parsing

```java
// Conectar a URL
Document doc = Jsoup.connect("http://exemplo.com").get();

// Parsear HTML string
Document doc = Jsoup.parse("<html>...</html>");

// Parsear arquivo
Document doc = Jsoup.parse(new File("arquivo.html"), "UTF-8");
```

### Seleção de Elementos

```java
// Por tag
Elements ps = doc.select("p");

// Por ID
Element el = doc.getElementById("content");

// Por classe
Elements els = doc.getElementsByClass("destaque");

// Seletor CSS complexo
Elements links = doc.select("div.content a[href]");
```

### Extração de Dados

```java
// Texto
String text = element.text();

// HTML
String html = element.html();

// Atributo
String href = element.attr("href");

// Verificar existência
boolean tem = element.hasAttr("href");
```

### Iteração

```java
// For-each
for (Element el : elements) {
    System.out.println(el.text());
}

// Stream (Java 8+)
elements.stream()
    .map(Element::text)
    .forEach(System.out::println);
```

---

<div align="center">

## 🕷️ Web Scraping Ético com JSoup 🚀

**Parse HTML de forma simples e poderosa com Java**

### ⭐ Se este projeto foi útil, considere dar uma estrela!

### 📚 Continue explorando o mundo do web scraping!

---

**"Dados estão em toda parte, JSoup te ajuda a encontrá-los!"** 🔍

**Java + JSoup = Web Scraping Fácil ❤️**

</div>

---

## 📞 Suporte

### Precisa de Ajuda?

- 📖 Consulte a [documentação oficial do JSoup](https://jsoup.org/)
- 🔍 Pesquise no [Stack Overflow](https://stackoverflow.com/questions/tagged/jsoup)
- 💬 Acesse o [GitHub Issues](https://github.com/jhy/jsoup/issues)
- 📧 Abra uma issue neste repositório

### Comunidades

- [JSoup Google Group](https://groups.google.com/g/jsoup)
- [Stack Overflow - JSoup Tag](https://stackoverflow.com/questions/tagged/jsoup)
- [Reddit - r/webscraping](https://www.reddit.com/r/webscraping/)

---

## 🏅 Recursos de Aprendizado

### Tutoriais Recomendados

1. **[JSoup Cookbook](https://jsoup.org/cookbook/)** - Guia oficial
2. **[Baeldung JSoup Guide](https://www.baeldung.com/java-with-jsoup)** - Tutorial completo
3. **[Web Scraping 101](https://www.scrapingbee.com/blog/)** - Blog especializado

### Vídeos

- YouTube - "JSoup Tutorial Java" (em português)
- YouTube - "Web Scraping with Java" (em inglês)
- Udemy - Cursos de Web Scraping com Java

### Artigos

- [JSoup vs HtmlUnit vs Selenium](https://www.baeldung.com/java-jsoup-vs-htmlunit-vs-selenium)
- [Best Practices for Web Scraping](https://www.scrapingbee.com/blog/web-scraping-best-practices/)
- [Legal Aspects of Web Scraping](https://blog.apify.com/is-web-scraping-legal/)

---

## 💡 Dicas Pro

### Performance

```java
// Reusar conexão para múltiplas requisições
Connection connection = Jsoup.connect(url)
    .userAgent("Mozilla/5.0")
    .timeout(10000);

Document doc1 = connection.get();
Document doc2 = connection.post();  // Mesma conexão

// Pool de threads para scraping paralelo
ExecutorService executor = Executors.newFixedThreadPool(5);
List<String> urls = Arrays.asList(/* URLs */);

urls.forEach(url -> executor.submit(() -> {
    try {
        Document doc = Jsoup.connect(url).get();
        // Processar
    } catch (IOException e) {
        e.printStackTrace();
    }
}));

executor.shutdown();
```

### Debugging

```java
// Ver estrutura HTML
System.out.println(doc.html());

// Ver apenas body
System.out.println(doc.body().html());

// Verificar se seletor encontrou algo
Elements els = doc.select("div.teste");
System.out.println("Encontrados: " + els.size());

// Salvar HTML para análise
Files.write(Paths.get("debug.html"), doc.html().getBytes());
```

### Tratamento Robusto

```java
public class ScraperRobusto {
    
    private static final int MAX_RETRIES = 3;
    private static final int RETRY_DELAY = 2000;
    
    public static Document baixarComRetry(String url) {
        for (int i = 0; i < MAX_RETRIES; i++) {
            try {
                return Jsoup.connect(url)
                    .timeout(10000)
                    .get();
            } catch (IOException e) {
                System.err.println("Tentativa " + (i+1) + " falhou");
                if (i < MAX_RETRIES - 1) {
                    Thread.sleep(RETRY_DELAY);
                } else {
                    throw new RuntimeException("Falha após " + MAX_RETRIES + " tentativas", e);
                }
            }
        }
        return null;
    }
}
```

---

## 🌟 Showcase de Projetos

### Projetos Inspiradores com JSoup

1. **[Apache Nutch](https://nutch.apache.org/)** - Web crawler
2. **[Crawler4j](https://github.com/yasserg/crawler4j)** - Framework de crawling
3. **[StormCrawler](https://github.com/DigitalPebble/storm-crawler)** - Crawler distribuído
4. **[WebMagic](https://github.com/code4craft/webmagic)** - Framework escalável

---

## 📝 Notas Importantes

> ⚠️ **Legalidade:** Web scraping é uma área cinzenta legalmente. Sempre verifique os Termos de Serviço do site e consulte um advogado se for usar comercialmente.

> 🤖 **robots.txt:** Respeite as diretrizes dos sites. Se um site proíbe scraping no robots.txt, não faça scraping.

> 🔒 **LGPD/GDPR:** Tenha cuidado ao coletar dados pessoais. Respeite leis de privacidade.

> 💻 **JavaScript:** JSoup não executa JavaScript. Para sites dinâmicos (React, Angular, Vue), use Selenium ou HtmlUnit.

> 🎯 **Uso Educacional:** Este projeto é para fins educacionais. Use com responsabilidade e ética.

---

## 🔗 Links Úteis

- [JSoup Official](https://jsoup.org/) - Site oficial
- [JSoup GitHub](https://github.com/jhy/jsoup) - Código fonte
- [Maven Central - JSoup](https://mvnrepository.com/artifact/org.jsoup/jsoup) - Repositório Maven
- [JSoup Try Online](https://try.jsoup.org/) - Experimentar JSoup online

---

## 🏆 Conquistas do Projeto

- ✅ Implementação funcional de web scraping
- ✅ Código limpo e bem comentado
- ✅ Tratamento de exceções adequado
- ✅ Estrutura Maven organizada
- ✅ Compatibilidade com IDEs populares
- ✅ Exemplo didático e reutilizável

---

<div align="center">

**Desenvolvido com ☕ Java e 🕷️ JSoup**

**📅 Última atualização:** Abril 2026  
**📌 Versão JSoup:** 1.14.2+  
**✅ Status:** Funcional e educacional

---

**#Java #JSoup #WebScraping #HTMLParsing #DataExtraction #Maven**

</div>
