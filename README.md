<div align="center">

# ☕ JARVIS do Java

### Assistente de estudos para a jornada de aprendizado em Java

Repositório de apresentação e documentação de um caderno educacional criado no NotebookLM para apoiar estudos de Java, lógica de programação, orientação a objetos e desenvolvimento profissional.

![Java](https://img.shields.io/badge/Java-Estudos-ED8B00?style=for-the-badge\&logo=openjdk\&logoColor=white)
![NotebookLM](https://img.shields.io/badge/NotebookLM-Assistente_de_Estudos-4285F4?style=for-the-badge\&logo=google\&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-Documentação-181717?style=for-the-badge\&logo=github)
![Status](https://img.shields.io/badge/Status-Em_evolução-yellow?style=for-the-badge)

<br>

[![Acessar Notebook](https://img.shields.io/badge/Acessar-JARVIS_do_Java-ED8B00?style=for-the-badge\&logo=openjdk\&logoColor=white)](https://notebooklm.google.com/notebook/e0e94c6d-6f62-413c-b93e-109bf24874c5)

</div>

---

## 📌 Sobre o projeto

O **JARVIS do Java** é um caderno educacional criado no NotebookLM para auxiliar estudantes durante o aprendizado da linguagem Java.

A proposta é reunir fontes, explicações e materiais relacionados a:

* fundamentos da linguagem;
* lógica de programação;
* programação orientada a objetos;
* recursos intermediários;
* boas práticas;
* preparação para projetos;
* evolução para o ecossistema Java.

O NotebookLM pode utilizar as fontes adicionadas ao caderno para responder perguntas, resumir conteúdos, criar guias de estudo e ajudar na revisão dos temas.

> Este repositório não contém uma aplicação Java nem o código-fonte de um assistente virtual. Ele documenta e direciona para um caderno educacional hospedado no NotebookLM.

---

## 🚀 Acessar o caderno

O material principal está disponível no NotebookLM:

### [Abrir o JARVIS do Java](https://notebooklm.google.com/notebook/e0e94c6d-6f62-413c-b93e-109bf24874c5)

> O acesso ao caderno pode depender das configurações de compartilhamento definidas no NotebookLM e de uma conta Google.

---

## 🎯 Objetivos

Os principais objetivos do projeto são:

* centralizar materiais de estudo sobre Java;
* facilitar consultas sobre os conteúdos;
* apoiar revisões;
* organizar uma sequência de aprendizagem;
* fortalecer os fundamentos;
* evitar o estudo baseado apenas em memorização;
* incentivar a prática com código;
* apoiar a preparação para projetos futuros;
* servir como complemento aos estudos em cursos e graduações.

---

## 🧠 Proposta de aprendizagem

Aprender Java não significa apenas memorizar comandos.

É necessário compreender:

* como os programas são estruturados;
* como os dados são representados;
* como controlar o fluxo da aplicação;
* como dividir responsabilidades;
* como modelar objetos;
* como tratar erros;
* como organizar coleções;
* como escrever código legível;
* como testar o que foi desenvolvido;
* como evoluir uma aplicação com segurança.

O JARVIS do Java busca atuar como apoio durante esse processo.

---

## 📚 Trilha de conteúdos

### 1. Fundamentos da linguagem

Conteúdos introdutórios:

* estrutura de um programa Java;
* método `main`;
* variáveis;
* constantes;
* tipos primitivos;
* tipos por referência;
* operadores;
* entrada e saída;
* conversão de tipos;
* estruturas condicionais;
* estruturas de repetição;
* métodos.

Exemplo:

```java
public class Main {
    public static void main(String[] args) {
        String nome = "Ernesto";

        System.out.println("Olá, " + nome + "!");
    }
}
```

---

### 2. Programação orientada a objetos

Conteúdos relacionados à modelagem de sistemas:

* classes;
* objetos;
* atributos;
* métodos;
* construtores;
* encapsulamento;
* herança;
* polimorfismo;
* abstração;
* interfaces;
* modificadores de acesso.

Exemplo:

```java
public class Conta {
    private double saldo;

    public void depositar(double valor) {
        if (valor <= 0) {
            throw new IllegalArgumentException(
                "O valor deve ser maior que zero."
            );
        }

        saldo += valor;
    }

    public double getSaldo() {
        return saldo;
    }
}
```

---

### 3. Tratamento de exceções

Conteúdos relacionados à identificação e tratamento de erros:

* `try`;
* `catch`;
* `finally`;
* `throw`;
* `throws`;
* exceções verificadas;
* exceções não verificadas;
* criação de exceções próprias.

Exemplo:

```java
try {
    int resultado = 10 / 0;
    System.out.println(resultado);
} catch (ArithmeticException exception) {
    System.out.println("Não é possível dividir por zero.");
}
```

---

### 4. Collections Framework

Estruturas utilizadas para armazenar e manipular grupos de objetos:

* `List`;
* `ArrayList`;
* `Set`;
* `HashSet`;
* `Map`;
* `HashMap`;
* filas;
* ordenação;
* percursos;
* comparadores.

Exemplo:

```java
import java.util.ArrayList;
import java.util.List;

public class Main {
    public static void main(String[] args) {
        List<String> linguagens = new ArrayList<>();

        linguagens.add("Java");
        linguagens.add("Python");

        for (String linguagem : linguagens) {
            System.out.println(linguagem);
        }
    }
}
```

---

### 5. Generics

Generics ajudam a criar estruturas reutilizáveis e seguras em relação aos tipos.

Exemplo:

```java
public class Caixa<T> {
    private T valor;

    public void guardar(T valor) {
        this.valor = valor;
    }

    public T obter() {
        return valor;
    }
}
```

---

### 6. Expressões lambda

As expressões lambda permitem representar comportamentos de forma mais direta.

Exemplo:

```java
List<String> nomes = List.of(
    "Ana",
    "Bruno",
    "Carlos"
);

nomes.forEach(nome -> System.out.println(nome));
```

---

### 7. Streams API

Streams podem ser utilizados para filtrar, transformar e processar coleções.

Exemplo:

```java
List<Integer> numeros = List.of(1, 2, 3, 4, 5, 6);

List<Integer> pares = numeros.stream()
    .filter(numero -> numero % 2 == 0)
    .toList();

System.out.println(pares);
```

---

## 🧹 Boas práticas

O material busca incentivar práticas como:

* nomes claros;
* métodos pequenos;
* responsabilidades bem definidas;
* código sem duplicação desnecessária;
* validação de entradas;
* tratamento adequado de erros;
* separação entre regras e interface;
* documentação útil;
* testes;
* organização por pacotes.

---

## 🛠️ Como utilizar o JARVIS do Java

Uma rotina recomendada é:

1. escolha um conteúdo;
2. leia a fonte principal;
3. peça ao NotebookLM uma explicação;
4. solicite exemplos;
5. escreva o código na sua IDE;
6. modifique o exemplo;
7. resolva exercícios;
8. revise os erros;
9. registre os aprendizados;
10. desenvolva um pequeno projeto.

O assistente deve complementar o estudo, não substituir a prática.

---

## 💬 Exemplos de perguntas

Perguntas que podem ser utilizadas no NotebookLM:

```text
Explique a diferença entre variável primitiva e referência em Java.
```

```text
Crie um exercício básico sobre estruturas condicionais.
```

```text
Explique encapsulamento com um exemplo de conta bancária.
```

```text
Compare ArrayList, HashSet e HashMap.
```

```text
Crie cinco questões sobre tratamento de exceções.
```

```text
Analise este código e explique cada linha.
```

```text
Monte um plano de revisão sobre orientação a objetos.
```

---

## 🧪 Uso responsável da inteligência artificial

Respostas geradas por IA podem conter:

* erros;
* simplificações;
* APIs inexistentes;
* códigos incompletos;
* práticas inadequadas;
* informações desatualizadas.

Por isso, recomenda-se:

* executar todos os exemplos;
* consultar a documentação oficial;
* conferir mensagens do compilador;
* escrever testes;
* evitar copiar código sem entender;
* comparar a resposta com as fontes do caderno.

---

## 🧰 Ferramentas recomendadas

| Ferramenta    | Aplicação                     |
| ------------- | ----------------------------- |
| NotebookLM    | Consulta e revisão das fontes |
| JDK           | Compilação e execução         |
| IntelliJ IDEA | Desenvolvimento Java          |
| VS Code       | Alternativa de editor         |
| Git           | Controle de versão            |
| GitHub        | Publicação de exercícios      |
| Maven         | Gerenciamento de projetos     |
| Gradle        | Alternativa de build          |

---

## 💻 Ambiente Java

Verifique a instalação:

```bash
java --version
```

Verifique o compilador:

```bash
javac --version
```

Compile um arquivo:

```bash
javac Main.java
```

Execute:

```bash
java Main
```

---

## 🗺️ Evolução planejada

Depois dos fundamentos, a trilha poderá avançar para:

* Maven;
* Gradle;
* testes com JUnit;
* Mockito;
* JDBC;
* bancos de dados;
* APIs REST;
* Spring;
* Spring Boot;
* Spring Data JPA;
* Hibernate;
* autenticação;
* Docker;
* arquitetura de software;
* microsserviços.

> Esses temas representam uma evolução planejada e não significam que todos já estejam disponíveis no caderno.

---

## 📁 Estrutura atual do repositório

```text
NotebookLM/
└── README.md
```

Atualmente, o repositório contém apenas a documentação e o link de acesso ao caderno.

Não estão armazenados aqui:

* códigos Java;
* exercícios;
* projetos;
* fontes do NotebookLM;
* arquivos de configuração;
* testes;
* exemplos executáveis.

---

## 📁 Estrutura recomendada

Para transformar este repositório em uma base de estudos mais completa:

```text
NotebookLM/
│
├── exemplos/
│   ├── fundamentos/
│   ├── orientacao-a-objetos/
│   ├── collections/
│   └── streams/
│
├── exercicios/
│   ├── nivel-basico/
│   ├── nivel-intermediario/
│   └── nivel-avancado/
│
├── projetos/
│   ├── sistema-bancario/
│   └── gerenciador-de-tarefas/
│
├── docs/
│   ├── trilha-de-estudos.md
│   └── fontes.md
│
└── README.md
```

---

## 🧩 Projetos sugeridos

Para consolidar o aprendizado:

### Nível básico

* calculadora;
* conversor de unidades;
* sistema de notas;
* jogo de adivinhação.

### Nível intermediário

* sistema bancário;
* gerenciador de tarefas;
* catálogo de produtos;
* sistema de biblioteca.

### Evolução para backend

* API de tarefas;
* API de clientes;
* sistema de agendamentos;
* controle financeiro.

---

## ⚠️ Limitações atuais

O projeto possui algumas limitações:

* depende de um serviço externo;
* pode exigir autenticação;
* o acesso pode ser restrito;
* as fontes não estão versionadas no GitHub;
* não existe histórico público do conteúdo;
* não há código Java no repositório;
* não existem exercícios armazenados;
* não há testes;
* não existe aplicação executável;
* o conteúdo do caderno não pode ser revisado pelo GitHub.

---

## 🔐 Cuidados com as fontes

Não adicione ao NotebookLM ou ao GitHub materiais que contenham:

* dados pessoais;
* documentos privados;
* credenciais;
* chaves de API;
* conteúdo confidencial;
* livros completos sem autorização;
* materiais protegidos distribuídos ilegalmente.

Utilize fontes próprias, públicas ou com licença compatível.

---

## 📚 Aprendizados desenvolvidos

Este projeto permite praticar:

* organização de estudos;
* curadoria de fontes;
* aprendizado assistido por IA;
* formulação de perguntas;
* revisão;
* documentação;
* planejamento de trilhas;
* fundamentos de Java;
* orientação a objetos;
* boas práticas.

---

## 🎓 Contexto do projeto

O JARVIS do Java foi criado como uma ferramenta de apoio à jornada de aprendizado em Java.

O GitHub funciona como página pública de apresentação, enquanto o conteúdo principal está organizado no NotebookLM.

---

## 👨‍💻 Autor

Desenvolvido por **Ernesto — ONestoDev**.

[![GitHub](https://img.shields.io/badge/GitHub-ONestoDev-181717?style=for-the-badge\&logo=github)](https://github.com/ONestoDev)

---

## 📄 Licença

Este repositório ainda não possui uma licença definida.

A licença do README não concede automaticamente direitos sobre as fontes utilizadas no NotebookLM. Cada material deve respeitar sua própria licença e seus direitos autorais.
