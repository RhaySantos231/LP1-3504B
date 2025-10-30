# LP1-3504B
## Sub Titulo
### teste
texto normal

# Principais Comandos Git

| Comando | Descrição |
|---------|-----------|
| `git init` | Inicializa um novo repositório Git na pasta atual |
| `git clone <url>` | Clona um repositório remoto para a máquina local |
| `git status` | Mostra o estado atual dos arquivos (modificados, não rastreados etc.) |
| `git add <arquivo>` | Adiciona um arquivo específico para a área de staging |
| `git add .` | Adiciona **todos os arquivos modificados** para a área de staging |
| `git commit -m "mensagem"` | Registra as mudanças adicionadas com uma mensagem |
| `git log` | Mostra o histórico de commits |
| `git branch` | Lista todas as branches (ramificações) |
| `git branch <nome>` | Cria uma nova branch |
| `git checkout <nome>` | Troca para a branch especificada |
| `git merge <nome>` | Mescla a branch especificada com a branch atual |
| `git remote -v` | Mostra os repositórios remotos configurados |
| `git push origin <branch>` | Envia os commits locais para o repositório remoto |
| `git pull origin <branch>` | Atualiza a branch local com alterações do remoto |
| `git fetch` | Busca atualizações do repositório remoto **sem mesclar** |
| `git reset --hard <hash>` | Reseta o repositório para um commit específico (perigoso, pois apaga alterações locais) |

---

📌 **Dica para alunos iniciantes**:  
A sequência mais comum é:  
```bash
git add .
git commit -m "Mensagem explicativa"
```


# Introdução a Linguagem de Programação Kotlin

## Vantagens:
- Criado pela JetBrains em 2011.

- Oficialmente suportado pelo Google para Android desde 2017.

- Estaticamente tipada (tipos definidos em tempo de compilação).

- Pode ser usada em Android, backend, desktop e web.

- Interoperável com Java (funciona junto no mesmo projeto).

- Sintaxe simples e enxuta, com menos código repetitivo.

- Suporta POO e programação funcional.


# Tipos de Variáveis em Kotlin

| Tipo       | Descrição | Exemplo |
|------------|-----------|---------|
| `Int`      | Números inteiros (32 bits) | `val idade: Int = 20` |
| `Long`     | Números inteiros longos (64 bits) | `val populacao: Long = 7500000000` |
| `Short`    | Números inteiros curtos (16 bits) | `val numero: Short = 30000` |
| `Byte`     | Números inteiros pequenos (8 bits) | `val b: Byte = 120` |
| `Double`   | Números decimais (64 bits, maior precisão) | `val peso: Double = 70.5` |
| `Float`    | Números decimais (32 bits, menor precisão) | `val altura: Float = 1.75f` |
| `Char`     | Um único caractere | `val letra: Char = 'A'` |
| `String`   | Texto (sequência de caracteres) | `val nome: String = "Maria"` |
| `Boolean`  | Valores lógicos (true / false) | `val ativo: Boolean = true` |

---

📌 **Dica:**  
- Use `val` para variáveis **imutáveis** (constantes).  
- Use `var` para variáveis **mutáveis** (que podem mudar de valor).  

# Operadores Matemáticos em Programação

## Principais Operadores

1. **`+` (Adição)** → Soma valores.  
   Exemplo: `5 + 3 = 8`

2. **`-` (Subtração)** → Subtrai valores.  
   Exemplo: `10 - 4 = 6`

3. **`*` (Multiplicação)** → Multiplica valores.  
   Exemplo: `6 * 2 = 12`

4. **`/` (Divisão)** → Divide valores.  
   Exemplo: `15 / 3 = 5`

5. **`%` (Módulo ou Resto da Divisão)** → Retorna o resto de uma divisão.  
   Exemplo: `10 % 3 = 1`


# Estruturas Condicionais (if / else)

O `if` e o `else` são usados para tomar decisões no programa.  
Eles verificam uma condição (verdadeira ou falsa) e executam o bloco correspondente.

## Exemplos

1. **If/else simples**  
```kotlin
val idade = 18

if (idade >= 18) {
    println("Você é maior de idade")
}else{
    println("Você é menor de idade")
}
```
## ✅ If/Else Composto (`else if`)

Use quando você precisa **avaliar várias condições diferentes**, e não apenas duas opções.

### Exemplo em Kotlin:
```kotlin
val nota = 75

if (nota >= 90) {
    println("Excelente!")
} else if (nota >= 70) {
    println("Bom desempenho")
} else if (nota >= 50) {
    println("Precisa melhorar")
} else {
    println("Reprovado")
}
```
# Estruturas de Repetição em Kotlin

As estruturas de repetição permitem executar um bloco de código várias vezes, enquanto uma condição for verdadeira. Em Kotlin, as principais estruturas são `while` e `do/while`.

---

## Estrutura `while`

O `while` executa o bloco de código **enquanto a condição for verdadeira**.  
A condição é verificada **antes** de cada execução.

### Sintaxe básica
```kotlin
while (condicao) {
    // código a ser repetido
}
```
## 2. Estrutura `do/while`

O `do/while` executa o bloco **pelo menos uma vez**, e só depois verifica a condição.  
Isso garante que o bloco seja executado mesmo que a condição seja falsa no início.

### Sintaxe
```kotlin
do {
    // código a ser repetido
} while (condicao)
```
# Estrutura `when`

O `when` é uma estrutura de controle de fluxo em Kotlin, semelhante ao `switch` de outras linguagens, mas mais poderosa. Ele permite executar diferentes blocos de código dependendo do valor de uma expressão.

---

## Sintaxe básica

```kotlin
when (expressao) {
    valor1 -> {
        // código a ser executado se expressao == valor1
    }
    valor2 -> {
        // código a ser executado se expressao == valor2
    }
    else -> {
        // código a ser executado se nenhum valor corresponder
    }
}
```
---
# Operadores de Comparação em Kotlin

| Operador | Significado             | Exemplo em Kotlin   | Resultado |
|----------|-------------------------|---------------------|-----------|
| >        | Maior que               | `5 > 3`             | `true`    |
| <        | Menor que               | `2 < 7`             | `true`    |
| >=       | Maior ou igual          | `5 >= 5`            | `true`    |
| <=       | Menor ou igual          | `4 <= 6`            | `true`    |
| ==       | Igualdade entre valores | `10 == 10`          | `true`    |
| !=       | Diferente de            | `8 != 3`            | `true`    |


---
# 📘 Introdução — Arrays e Listas em Kotlin

## 🔹 O que é um Array?

Um **Array** é uma estrutura que armazena **vários valores do mesmo tipo** em uma única variável.  
Cada elemento possui um **índice**, começando em **0**.

### Exemplo:
```kotlin
val numeros = arrayOf(10, 20, 30, 40)
println(numeros[0]) // Exibe 10
```
> ⚠️ **Importante:** O tamanho de um `array` é **fixo** — depois de criado, **não pode ser alterado**.

---

## 🔹 O que é uma List?

Uma **List** é parecida com um `Array`, mas **mais flexível**.  
Existem dois tipos principais:

- `listOf()` → **imutável** (não pode adicionar ou remover itens)  
- `mutableListOf()` → **mutável** (permite adicionar, remover, modificar)

---

### Exemplo:

```kotlin
val frutas = mutableListOf("Maçã", "Banana", "Laranja")
frutas.add("Melancia")       // Adiciona
frutas.remove("Banana")      // Remove
println(frutas[0])           // Exibe "Maçã"
```
# 🧩 Comandos de Manipulação de List em Kotlin

| 💻 Comando / Método | 📝 Descrição | 🧠 Exemplo em Kotlin |
|----------------------|--------------|-----------------------|
| `listOf()` | Cria uma **lista imutável** (não pode ser modificada) | `val frutas = listOf("Maçã", "Banana")` |
| `mutableListOf()` | Cria uma **lista mutável** (permite alterações) | `val frutas = mutableListOf("Maçã", "Banana")` |
| `add(item)` | Adiciona um novo item à lista | `frutas.add("Laranja")` |
| `add(index, item)` | Adiciona um item em uma posição específica | `frutas.add(1, "Uva")` |
| `remove(item)` | Remove o item especificado | `frutas.remove("Banana")` |
| `removeAt(index)` | Remove o item na posição informada | `frutas.removeAt(0)` |
| `clear()` | Remove **todos** os itens da lista | `frutas.clear()` |
| `size` | Retorna o **tamanho da lista** | `println(frutas.size)` |
| `isEmpty()` | Verifica se a lista está vazia (retorna `true` ou `false`) | `frutas.isEmpty()` |
| `contains(item)` | Verifica se um item está presente na lista | `frutas.contains("Maçã")` |
| `get(index)` | Retorna o item de um índice específico | `println(frutas.get(0))` |
| `[index]` | Acessa o item diretamente pelo índice | `println(frutas[1])` |
| `indexOf(item)` | Retorna o índice da primeira ocorrência do item | `println(frutas.indexOf("Laranja"))` |
| `sort()` | Ordena a lista em ordem crescente (alfabética ou numérica) | `frutas.sort()` |
| `reverse()` | Inverte a ordem dos elementos da lista | `frutas.reverse()` |
| `for (item in lista)` | Percorre todos os elementos da lista | `for (f in frutas) println(f)` |
| `joinToString()` | Converte a lista em uma única string formatada | `println(frutas.joinToString(", "))` |

---
# 🔁 Estrutura de Repetição `for` em Kotlin

O `for` é usado para percorrer **intervalos**, **listas**, **arrays** e **strings** de forma simples.

---
## 🧩 Estrutura básica

```kotlin
for (item in colecao) {
    // código a ser repetido
}
```
💡 **Dica:**  
Use `listOf()` para coleções fixas e `mutableListOf()` quando quiser **adicionar ou remover itens** dinamicamente.


# Funções 
Uma função é um bloco de código reutilizável que executa uma tarefa. Elas ajudam a organizar melhor o código, evitar repetição e facilitam a manutenção do programa.
## Estrura de uma Funções
fun nomeDaFuncao(parametros): TipoDeRetorno {
    // ações
}
| Componente      | Descrição                                    |
| --------------- | -------------------------------------------- |
| `fun`           | Palavra-chave usada para declarar uma função |
| `nomeDaFuncao`  | Nome que identifica a função                 |
| `parametros`    | Dados que a função pode receber (opcional)   |
| `TipoDeRetorno` | Tipo de dado que a função devolve (opcional) |
| `{ ... }`       | Bloco de código executado                    |

## Exemplo: Função com retorno
```
 fun soma(a: Int, b: Int): Int {
    return a + b
}

```
## Função sem retorno (Unit)
```
fun mostrarMensagem() {
    println("Olá! Esta é uma função sem retorno.")
}
```
## Função com parâmetro opcional
```
fun saudacao(nome: String = "Visitante") {
    println("Bem-vindo, $nome!")
}

```
# 📘 Classes em Kotlin

## 🧠 O que é uma classe?

Em Kotlin (e em outras linguagens orientadas a objetos), uma **classe** é um modelo ou molde que descreve as **características (propriedades)** e **comportamentos (métodos)** de um objeto.

> 💬 Em resumo: **classe** é a forma, **objeto** é o conteúdo.

Por exemplo, podemos ter a classe `Carro` como um molde, e dela criar vários objetos como `carro1`, `carro2`, etc.

---

## Estrutura básica de uma classe

```kotlin
class Carro {
    var marca: String = ""
    var modelo: String = ""
    var ano: Int = 0

    fun ligar() {
        println("O carro $modelo está ligado!")
    }
}
```

## Criando e usando objetos
Para usar uma classe, criamos objetos dela (ou seja, instâncias):
```
fun main() {
    val carro1 = Carro()
    carro1.marca = "Fiat"
    carro1.modelo = "Uno"
    carro1.ano = 2010

    carro1.ligar()
}
```
## Construtores

O Kotlin facilita a criação de construtores, que são formas de inicializar objetos com valores logo ao criá-los.

```
class Carro(val marca: String, val modelo: String, var ano: Int) {
    fun exibirInfo() {
        println("Marca: $marca | Modelo: $modelo | Ano: $ano")
    }
}

fun main() {
    val carro = Carro("Honda", "Civic", 2020)
    carro.exibirInfo()
}

```
---

### open class — Permite Herança

Por padrão, as classes em Kotlin são “final”, ou seja, não podem ser herdadas.
Para permitir que outra classe herde dela, usamos o modificador open.
```
open class Animal(val nome: String) {
    fun dormir() {
        println("$nome está dormindo...")
    }

    open fun fazerSom() {
        println("$nome fez um som!")
    }
}

class Cachorro(nome: String) : Animal(nome) {
    override fun fazerSom() {
        println("$nome latiu: Au Au!")
    }
}

fun main() {
    val dog = Cachorro("Rex")
    dog.dormir()
    dog.fazerSom()
}

```
### Explicação:

open class Animal → permite que a classe seja herdada.

: Animal(nome) → indica que a classe Cachorro herda de Animal.

override fun → sobrescreve um método da classe pai.

### Herança e Polimorfismo

Quando uma classe herda outra, ela ganha acesso aos métodos e atributos da classe pai.
Podemos também modificar o comportamento desses métodos (isso é o polimorfismo).
```
open class Pessoa(val nome: String) {
    open fun apresentar() {
        println("Olá, meu nome é $nome.")
    }
}

class Professor(nome: String, val disciplina: String) : Pessoa(nome) {
    override fun apresentar() {
        println("Olá, sou o professor $nome e leciono $disciplina.")
    }
}

fun main() {
    val p1 = Pessoa("Maria")
    val p2 = Professor("João", "Kotlin")

    p1.apresentar()
    p2.apresentar()
}

```

## Encapsulamento

Encapsulamento significa proteger os dados de uma classe, controlando como eles podem ser acessados ou alterados.
Em Kotlin, usamos modificadores de visibilidade:

Modificador	Acesso permitido em...
public (padrão)	Qualquer lugar
private	Apenas dentro da própria classe
protected	Na classe e em subclasses
internal	Dentro do mesmo módulo/projeto

```
class ContaBancaria {
    private var saldo: Double = 0.0

    fun depositar(valor: Double) {
        if (valor > 0) {
            saldo += valor
            println("Depósito de R$ $valor realizado com sucesso.")
        }
    }

    fun verSaldo() {
        println("Saldo atual: R$ $saldo")
    }
}

fun main() {
    val conta = ContaBancaria()
    conta.depositar(100.0)
    conta.verSaldo()
    // conta.saldo = 999.0  ❌ ERRO: saldo é privado!
}
```
### data class — Classes de Dados

Usadas para armazenar informações, as data class já vêm com:

   toString() automático

   equals() e hashCode()

   copy() para duplicar objetos facilmente

   data class Pessoa(val nome: String, val idade: Int)
   
```
fun main() {
    val p1 = Pessoa("Ana", 20)
    val p2 = p1.copy(idade = 21)

    println(p1)         // Pessoa(nome=Ana, idade=20)
    println(p2)         // Pessoa(nome=Ana, idade=21)
}
```
### Objeto Único (object)

Em Kotlin, o object é usado para criar uma única instância (singleton) automaticamente.
Serve bem para utilitários, contadores ou configurações.
```
object Contador {
    var valor = 0

    fun incrementar() {
        valor++
        println("Contagem atual: $valor")
    }
}

fun main() {
    Contador.incrementar()
    Contador.incrementar()
}


```
### Classe Abstrata

Uma classe abstrata serve como modelo e não pode ser instanciada diretamente.
Ela pode conter métodos abstratos, que devem ser implementados nas subclasses.

```
abstract class Funcionario(val nome: String) {
    abstract fun calcularSalario(): Double

    fun apresentar() {
        println("Funcionário: $nome")
    }
}

class Professor(nome: String, val aulas: Int) : Funcionario(nome) {
    override fun calcularSalario(): Double {
        return aulas * 50.0
    }
}

fun main() {
    val prof = Professor("Carlos", 20)
    prof.apresentar()
    println("Salário: R$ ${prof.calcularSalario()}")
}
```

### Classe com Herança + Construtor + Encapsulamento

```
open class Pessoa(
    val nome: String,
    private var idade: Int
) {
    open fun apresentar() {
        println("Olá! Meu nome é $nome e tenho $idade anos.")
    }
}

class Aluno(nome: String, idade: Int, val matricula: String) : Pessoa(nome, idade) {
    override fun apresentar() {
        println("Sou o aluno $nome, matrícula $matricula.")
    }
}

fun main() {
    val aluno = Aluno("Lucas", 18, "2025A01")
    aluno.apresentar()
}

```
📘 Saída:
```
Sou o aluno Lucas, matrícula 2025A01.
```



## 📂 Lista de Atividades
- [Lista 1 – Variáveis, Operadores Matemáticos e if/else](https://docs.google.com/document/d/1pfy5TH6OVX3XXufT9q3VN0aSqXCmTJGxGbD22tK6Ixw/edit?usp=sharing) (inicio 16/09| fim: 18/09) 
- [Lista 2 – When, while e do while](https://docs.google.com/document/d/1X7piSX--u729lxASkoCxMtXNbnMEUwBYLeS39EWXcGU/edit?tab=t.0#heading=h.bmwx0c14zlpb) (inicio: 23/09 | fim: 25/09)
- [Lista 3 - Array](https://docs.google.com/document/d/1vNd9r-2BIz2kouJxbMfPuK3-DWaq65unVfrng82M3cQ/edit?usp=sharing)
- [Lista 4 - Funções](https://docs.google.com/document/d/1r2xgCZ9deXtuBg3t8I-8zjyoGCj8VR00xM1c2KdB3rY/edit?usp=sharing)
- [Lista 5 - Classes](https://docs.google.com/document/d/1jN7t75e5EZuHT2ayuwMAPcURD7JbfEcHQ5cOP_nzbCg/edit?usp=sharing)
