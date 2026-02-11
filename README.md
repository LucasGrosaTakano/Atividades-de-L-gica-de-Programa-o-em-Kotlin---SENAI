---

# Lista de Exercícios — Lógica de Programação em Kotlin (Parte 1)

Este documento contém exercícios de lógica de programação desenvolvidos em Kotlin, com a descrição do desafio, o código solução e um resumo breve.

---

## Exercício 1 — Diferença entre dois números

### Descrição do desafio

Ler dois números e calcular a diferença entre eles, mostrando o resultado na tela.

### Código solução

```kotlin
fun main(){
    println("insira valor de A")
    var a = readln().toDouble()

    println("insira valor de B")
    var b = readln().toDouble()

    println("a diferença entre $a e $b é de: ${a - b}")
}
```

### Resumo breve

O programa lê dois valores e imprime a subtração `a - b`.

---

## Exercício 2 — Nome completo

### Descrição do desafio

Ler nome e sobrenome e mostrar o nome completo na tela.

### Código solução

```kotlin
fun main(){
    println("insira seu nome")
    var nome = readln().toString()

    println("insira seu sobrenome")
    var sobre = readln().toString()

    println("Olá! $nome $sobre!")
}
```

### Resumo breve

O programa lê duas strings e imprime o nome completo.

---

## Exercício 3 — Operações básicas

### Descrição do desafio

Ler dois números e mostrar os resultados de soma, subtração, multiplicação e divisão.

### Código solução

```kotlin
fun main(){
    println("insira o valor de A")
    var a = readln().toDouble()

    println("insira valor de B")
    var b = readln().toDouble()

    println("A soma dos dois valores é: ${a + b}, a subtração é ${a - b}, multiplicação é ${a*b} e divisão é ${a/b}")
}
```

### Resumo breve

O programa realiza as quatro operações matemáticas com os dois valores digitados.

---

## Exercício 4 — Área do quadrado (retângulo)

### Descrição do desafio

Calcular a área a partir do comprimento e largura informados.

### Código solução

```kotlin
fun main(){
    println("insira o valor do comprimento")
    var a = readln().toDouble()

    println("insira valor da largura")
    var b = readln().toDouble()

    println("a area do seu quadrado é de: ${a*b}")
}
```

### Resumo breve

O programa calcula a área usando `comprimento * largura`.

---

## Exercício 5 — Área do triângulo

### Descrição do desafio

Calcular a área do triângulo usando base e altura.

### Código solução

```kotlin
fun main(){
    println("insira o valor da base do triangulo")
    var a = readln().toDouble()

    println("insira valor da altura do triangulo")
    var b = readln().toDouble()

    println("a area do seu triangulo é: ${(a*b)/2} ")
}
```

### Resumo breve

O programa usa a fórmula `(base * altura) / 2`.

---

## Exercício 6 — IMC

### Descrição do desafio

Ler altura e peso, calcular IMC e mostrar a classificação.

### Código solução

```kotlin
fun main() {
    println("insira o valor de altura")
    val altura = readln().toFloat()

    println("insira o valor do peso")
    val peso = readln().toFloat()

    var resultado = Calculo(altura, peso)

    if (resultado < 18.5){
        println("Abaixo do peso")
    }else if (resultado >= 18.5 && resultado <= 24.9){
        println("Peso Normal")
    }else if (resultado >= 25 && resultado <= 29.9){
        println("Sobrepeso (Acima do peso desejado)")
    }else{
        println("Obesidade")
    }
}

fun Calculo(altura : Float, peso: Float): Float{
    return peso / (altura*altura)
}
```

### Resumo breve

O programa calcula o IMC e usa `if/else` para exibir a faixa correta.

---

## Exercício 7 — Idade em dias, meses e anos

### Descrição do desafio

Ler idade em anos e mostrar equivalente em dias, meses e anos.

### Código solução

```kotlin
fun main(){
    println("digite sua idade")
    var idade = readln().toDouble()

    println("sua idade expressa em dias é: ${idade * 365.25}, em meses ${idade * 12} e em anos $idade ")
}
```

### Resumo breve

O programa converte a idade para meses e dias usando multiplicação.

---

## Exercício 8 — Média de 3 notas

### Descrição do desafio

Ler 3 notas e calcular a média final.

### Código solução

```kotlin
fun main(){
    println("insira o valor da nota 1")
    var nota1 = readln().toDouble()

    println("insira o valor da nota 2")
    var nota2 = readln().toDouble()

    println("insira o valor da nota 3")
    var nota3 = readln().toDouble()

    println("o valor da média de notas é ${(nota1 + nota2 + nota3) / 3}")
}
```

### Resumo breve

O programa soma as 3 notas e divide por 3.

---

## Exercício 9 — Duração de evento em horas, minutos e segundos

### Descrição do desafio

Ler um tempo em segundos e converter para horas, minutos e segundos.

### Código solução

```kotlin
fun main(){
    println("digite o tempo do evento em segundos: ")
    var tempo = readln().toInt()

    var horas = tempo/3600
    var minutos = (tempo%3600) / 60
    var segundos = tempo%60

    println("a duração do evento é de $horas horas, $minutos minutos e $segundos segundos")
}
```

### Resumo breve

O programa usa divisão e resto (`%`) para converter o tempo.

---

