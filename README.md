# 📚 Exercícios de Java Básico - 10 Questões

Esta atividade contém 10 exercícios de Java básico para você resolver. Cada exercício foca em um conceito específico e está preparado para alunos novatos.

## 🎯 Objetivos dos Exercícios

- Praticar conceitos fundamentais de Java
- Desenvolver habilidades de programação básica
- Aprender a usar Scanner, estruturas condicionais e laços de repetição
- Criar e utilizar métodos

## 📋 Exercícios para Resolver

### **Questão 1 - Scanner (Entrada de Dados)**
**Objetivo:** Aprender a usar o Scanner para entrada de dados
- Crie um programa que leia o nome e a idade de uma pessoa
- Exiba uma mensagem de boas-vindas personalizada

**Exemplo de saída esperada:**
```
=== QUESTÃO 1 - SCANNER ===
Informe seu nome: João
Informe sua idade: 20
Olá João! Você tem 20 anos. Seja bem-vindo(a)!
```

### **Questão 2 - Print (Saída de Dados)**
**Objetivo:** Praticar formatação de saída
- Crie um programa que exiba uma tabela de multiplicação do 5 (de 1 a 10)
- Formate a saída de forma organizada

**Exemplo de saída esperada:**
```
=== QUESTÃO 2 - PRINT ===
Tabela de multiplicação do 5:
5 x 1 = 5
5 x 2 = 10
5 x 3 = 15
...
5 x 10 = 50
```

### **Questão 3 - For (Laço de Repetição)**
**Objetivo:** Aprender a usar o laço for
- Crie um programa que calcule e exiba a soma dos números de 1 até 100
- Use um laço for para fazer o cálculo

**Exemplo de saída esperada:**
```
=== QUESTÃO 3 - FOR ===
A soma dos números de 1 até 100 é: 5050
```

### **Questão 4 - If (Estrutura Condicional)**
**Objetivo:** Praticar estruturas condicionais
- Crie um programa que leia uma nota
- Informe se o aluno foi aprovado (nota >= 7), reprovado (nota < 4) ou está em recuperação (4 <= nota < 7)

**Exemplo de saída esperada:**
```
=== QUESTÃO 4 - IF ===
Informe sua nota: 8.5
Parabéns! Você foi APROVADO!
```

### **Questão 5 - While (Laço de Repetição)**
**Objetivo:** Aprender a usar o laço while
- Crie um programa que leia números inteiros até que o usuário digite 0
- Exiba a soma de todos os números digitados

**Exemplo de saída esperada:**
```
=== QUESTÃO 5 - WHILE ===
Digite números inteiros (digite 0 para parar):
5
3
7
0
A soma de todos os números digitados é: 15
```

### **Questão 6 - Métodos (Função)**
**Objetivo:** Criar e usar métodos
- Implemente o método `encontrarMaior()` que receba dois números e retorne o maior entre eles
- Teste o método com diferentes valores no main

**Exemplo de saída esperada:**
```
=== QUESTÃO 6 - MÉTODOS ===
Informe dois números para comparar:
10
5
O maior número entre 10 e 5 é: 10
```

### **Questão 7 - Scanner + If**
**Objetivo:** Combinar entrada de dados com estruturas condicionais
- Crie um programa que leia um número
- Informe se ele é par ou ímpar usando o operador % (módulo)

**Exemplo de saída esperada:**
```
=== QUESTÃO 7 - SCANNER + IF ===
Informe um número para verificar se é par ou ímpar:
8
O número 8 é PAR.
```

### **Questão 8 - For + Print**
**Objetivo:** Combinar laço for com saída formatada
- Crie um programa que exiba todos os números pares de 2 até 20
- Exiba um número por linha

**Exemplo de saída esperada:**
```
=== QUESTÃO 8 - FOR + PRINT ===
Números pares de 2 até 20:
2
4
6
8
10
12
14
16
18
20
```

### **Questão 9 - While + Scanner**
**Objetivo:** Combinar laço while com entrada de dados
- Crie um programa que leia números até que o usuário digite um número negativo
- Conte quantos números positivos foram digitados

**Exemplo de saída esperada:**
```
=== QUESTÃO 9 - WHILE + SCANNER ===
Digite números (digite um número negativo para parar):
5
3
7
2
-1
Foram digitados 4 números positivos.
```

### **Questão 10 - Métodos + For**
**Objetivo:** Criar métodos que usam laços de repetição
- Implemente o método `calcularFatorial()` que receba um número e retorne o fatorial desse número
- Teste o método com os valores 5 e 7

**Exemplo de saída esperada:**
```
=== QUESTÃO 10 - MÉTODOS + FOR ===
Testando fatorial de 5: 120
Testando fatorial de 7: 5040
```

## 🚀 Como Resolver os Exercícios

### Passo 1: Abrir o Arquivo
Abra o arquivo `src/fag/Principal.java` no seu editor de código.

### Passo 2: Implementar as Questões
- Cada questão tem um comentário `// SEU CÓDIGO AQUI` onde você deve implementar sua solução
- Leia atentamente as instruções de cada questão
- Use os exemplos de saída como referência

### Passo 3: Testar sua Implementação
```bash
# Compilar e executar com Maven
mvn compile exec:java -Dexec.mainClass="fag.Principal"

# Ou compilar manualmente
javac -d target/classes -cp "target/classes" src/main/java/fag/*.java
java -cp target/classes fag.Principal
```

### Passo 4: Verificar com Testes Automáticos
Para as questões 6 e 10, você pode verificar se sua implementação está correta executando os testes:

#### Opção 1: Com Maven (Recomendado)
```bash
# Executar todos os testes
mvn test

# Executar apenas os testes de fatorial
mvn test -Dtest=PrincipalTest#testCalcularFatorial*

# Executar apenas os testes de encontrar maior
mvn test -Dtest=PrincipalTest#testEncontrarMaior*

# Ver relatório amigável após os testes
mvn compile exec:java -Dexec.mainClass="fag.RelatorioTestes"
```

#### Opção 2: Compilação Manual
```bash
# 1. Baixar as dependências do JUnit (se não tiver Maven)
# Baixe os arquivos JAR do JUnit 5 do site oficial

# 2. Compilar o código
javac -cp "junit-jupiter-api-5.9.2.jar:junit-jupiter-engine-5.9.2.jar" -d bin src/fag/*.java

# 3. Executar os testes
java -cp "bin:junit-jupiter-api-5.9.2.jar:junit-jupiter-engine-5.9.2.jar" org.junit.platform.console.ConsoleLauncher --scan-classpath
```

#### Opção 3: IDE (Eclipse/IntelliJ)
- Clique com botão direito no arquivo `PrincipalTest.java`
- Selecione "Run Tests" ou "Executar Testes"
- Ou use o atalho `Ctrl+Shift+F10` (IntelliJ) ou `Alt+Shift+X, T` (Eclipse)

### Interpretando os Resultados dos Testes

#### ✅ Teste Passou
```
✅ testEncontrarMaior_PrimeiroMaior() - PASSED
```
Significa que sua implementação está correta!

#### ❌ Teste Falhou
```
❌ testCalcularFatorial_Numero5() - FAILED
Expected: 120
Actual: 0
```
Significa que há um erro na sua implementação. Verifique:
- Se você removeu o `return 0;` do método
- Se a lógica do fatorial está correta
- Se está usando o tipo `long` para evitar overflow

### 🔧 Solução de Problemas Comuns

#### Erro: "assertEquals is undefined" ou "Test cannot be resolved"
**Problema:** O JUnit não está sendo reconhecido pelo IDE.

**Soluções:**
1. **Use Maven:** Execute `mvn test` (mais confiável)
2. **Verifique as dependências:** Certifique-se de que o JUnit está no classpath
3. **Baixe os JARs:** Baixe os arquivos JAR do JUnit 5 do site oficial

#### Erro: "Method not found"
**Problema:** Os métodos `encontrarMaior()` ou `calcularFatorial()` não foram implementados.

**Solução:** Implemente os métodos no arquivo `Principal.java` conforme os exemplos no README.

#### Erro: "Compilation failed"
**Problema:** Erro de sintaxe no código.

**Solução:** Verifique se:
- Todos os `{` e `}` estão balanceados
- Não há ponto e vírgula faltando
- Os tipos de dados estão corretos (`int`, `long`, etc.)

#### Erro: "Module not found"
**Problema:** Problemas com configuração de módulos.

**Solução:** O arquivo `module-info.java` foi removido para simplificar. Use apenas:
```bash
mvn test
```

#### Erro: "No tests to run"
**Problema:** Maven não está encontrando os testes.

**Solução:** Certifique-se de que os arquivos estão na estrutura correta:
- Código principal: `src/main/java/fag/Principal.java`
- Testes: `src/test/java/fag/PrincipalTest.java`

#### Exemplo de Saída Completa dos Testes
```bash
$ mvn test

[INFO] Scanning for projects...
[INFO] 
[INFO] --- maven-surefire-plugin:3.0.0:test (default-test) ---
[INFO] Using auto detected provider org.apache.maven.surefire.junitplatform.JUnitPlatformProvider
[INFO] 
[INFO] -------------------------------------------------------
[INFO]  T E S T S
[INFO] -------------------------------------------------------
[INFO] Running fag.PrincipalTest
[INFO] Tests run: 10, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.123 s
[INFO] 
[INFO] Results:
[INFO] 
[INFO] Tests run: 10, Failures: 0, Errors: 0, Skipped: 0
[INFO] 
[INFO] BUILD SUCCESS
```

## 🧪 Testes Automáticos

O projeto inclui testes unitários para verificar se suas implementações estão corretas:

- **Questão 6:** Testa o método `encontrarMaior()`
- **Questão 10:** Testa o método `calcularFatorial()`

### Executar os Testes:
```bash
# Com Maven (Recomendado)
mvn test

# Com JUnit diretamente (se configurado)
javac -cp "junit-jupiter-api-5.9.2.jar:junit-jupiter-engine-5.9.2.jar" -d bin src/fag/*.java
java -cp "bin:junit-jupiter-api-5.9.2.jar:junit-jupiter-engine-5.9.2.jar" org.junit.platform.console.ConsoleLauncher --scan-classpath
```

## 📁 Estrutura do Projeto

```
Prova1bt02/
├── src/
│   ├── main/java/fag/
│   │   └── Principal.java      # Template com exercícios para resolver
│   └── test/java/fag/
│       └── PrincipalTest.java  # Testes unitários automáticos
├── target/                     # Arquivos compilados pelo Maven
├── pom.xml                     # Configuração do Maven
└── README.md                   # Este arquivo
```

## 🎓 Conceitos Abordados

- ✅ **Scanner:** Entrada de dados do usuário
- ✅ **Print:** Saída formatada de dados
- ✅ **For:** Laço de repetição com contador
- ✅ **If/Else:** Estruturas condicionais
- ✅ **While:** Laço de repetição com condição
- ✅ **Métodos:** Criação e uso de funções
- ✅ **Combinações:** Uso de múltiplos conceitos juntos

## 💡 Dicas para Resolver

1. **Leia atentamente** cada questão antes de começar a implementar
2. **Use os exemplos de saída** como referência para o formato esperado
3. **Teste cada questão** individualmente antes de passar para a próxima
4. **Para as questões 6 e 10**, use os testes unitários para verificar se está correto
5. **Se tiver dúvidas**, revise os conceitos básicos de Java antes de continuar

## 🔧 Exemplos de Código

### Questão 6 - Método Encontrar Maior
```java
public static int encontrarMaior(int a, int b) {
    if (a > b) {
        return a;
    } else {
        return b;
    }
}
```

### Questão 10 - Método Calcular Fatorial
```java
public static long calcularFatorial(int n) {
    long fatorial = 1;
    for (int i = 1; i <= n; i++) {
        fatorial *= i;
    }
    return fatorial;
}
```

### Exemplo de Uso no Main (Questão 6)
```java
System.out.println("Informe dois números para comparar:");
int num1 = scan.nextInt();
int num2 = scan.nextInt();
int maior = encontrarMaior(num1, num2);
System.out.println("O maior número entre " + num1 + " e " + num2 + " é: " + maior);
```

### Exemplo de Uso no Main (Questão 10)
```java
System.out.println("Testando fatorial de 5: " + calcularFatorial(5));
System.out.println("Testando fatorial de 7: " + calcularFatorial(7));
```

## 🔧 Dependências

- Java 11 ou superior
- JUnit 5 (para testes)
- Maven (opcional, para gerenciamento de dependências)

## 📝 Critérios de Avaliação

- **Implementação correta** da lógica de cada questão
- **Formatação adequada** da saída conforme os exemplos
- **Uso correto** dos conceitos solicitados (Scanner, For, If, While, Métodos)
- **Testes unitários** passando para as questões 6 e 10

---

**Boa sorte com os exercícios! 🍀**

*Lembre-se: a prática leva à perfeição. Não desista se algo não funcionar na primeira tentativa!*
