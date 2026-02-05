# ***Exercicios Kotlin 1 à 25***

## ***Exercicios 1***
```kotlin
fun main() {
    val num1 = readln().toInt()
    val num2 = readln().toInt()
    
    println("Resultado da subtração dos numeros é ${num1 - num2}")
}
```
## ***Exercicios 2***
```kotlin
fun main() {
    val nome = readln()
    val sobrenome = readln()
    
    println("Seu nome completo é $nome $sobrenome")
}
```

## ***Exercicios 3***
```kotlin
fun main() {
    val num1 = readln().toDouble()
    val num2 = readln().toDouble()
    
    println("Resultado da adição dos numeros é ${num1 + num2}")
    println("Resultado da subtração dos numeros é ${num1 - num2}")
    println("Resultado da mutiplicação dos numeros é ${num1 * num2}")
    println("Resultado da divisão dos numeros é ${num1 / num2}")
}
```

## ***Exercicios 4***
```kotlin
import kotlin.math.pow

fun main() {
    val lado = readln().toDouble()
    var resultado = lado.pow(2)
    
    println("O quadrado com lado $lado é $resultado")
    
}
```

## ***Exercicios 5***
```kotlin
fun main(){
    var altura = readln().toDouble()
    var largura = readln().toDouble()
    
    var areaTriangulo = (altura * largura) / 2
    println("A area do triangulo é $areaTriangulo")
}
```

## ***Exercicios 6***
```kotlin
import kotlin.math.pow
fun main() {
    println("Digite seu peso em kilos")
    val peso = readln().toDouble()
    println("Digite sua altura em metros")
    val altura = readln().toDouble()
    
    var imc = peso / altura.pow(2)
    
    if(imc < 18.5){
        println("Abaixo do peso")
    } else if(imc >= 18.5 && imc < 24.9){
        println("Peso normal")
    } else if(imc >= 24.9 && imc < 29.9){
        println("Sobrepeso")
    } else {
        println("Obesidade")
    }
    println(imc)
}
```

## ***Exercicios 7***
```kotlin
fun main(){
    var idadeEmDias = readln().toInt()
    
    if(idadeEmDias > 30){
    var meses = (idadeEmDias / 30).toInt()
    var diasRestantes = idadeEmDias % 30
        if(meses > 12){
        var anos = (meses / 12).toInt()
        var mesesRestantes = meses % 12
            if(anos > 0){
        println("Você é $anos ano(s) $mesesRestantes mês(es) e $diasRestantes dia(s) de idade")
        }
        } else {
            println("Você é $meses meses e $diasRestantes dia(s) de idade")
        }
    } else {
        println("Você é $idadeEmDias dia(s) de idade")
    }
    
}
```

## ***Exercicios 8***
```kotlin
fun main(){
    var nota1 = readln().toDouble()
    var nota2 = readln().toDouble()
    var nota3 = readln().toDouble()
    
    var media = (nota1 + nota2 + nota3) / 3 
    println("A média é $media")
}
```

## ***Exercicios 9***
```kotlin
fun main() {
    val segundos = readln().toInt()

    var horas = segundos / 3600
    var minutos = (segundos % 3600) / 60
    var segundosRestantes = segundos % 60

    println("O evento tem duração de $horas hora(s), $minutos minuto(s) e $segundosRestantes segundo(s).")
}
```

## ***Exercicios 10***
```kotlin
import kotlin.math.pow
import kotlin.math.sqrt

fun main() {
    println("Valor x1")
    var x1 = readln().toDouble()
    println("Valor x2")
    var x2 = readln().toDouble()
    println("Valor y1")
    var y1 = readln().toDouble()
    println("Valor y2")
    var y2 = readln().toDouble()
    
    var distancia = sqrt((x2 - x1).pow(2) + (y2 - y1).pow(2)) 
    
    println("Distancia é $distancia")
}
```

## ***Exercicios 11***
```kotlin
```

## ***Exercicios 12***
```kotlin
```

## ***Exercicios 13***
```kotlin
```

## ***Exercicios 14***
```kotlin
```

## ***Exercicios 15***
```kotlin
```

## ***Exercicios 16***
```kotlin
```

## ***Exercicios 17***
```kotlin
```

## ***Exercicios 18***
```kotlin
```

## ***Exercicios 19***
```kotlin
```

## ***Exercicios 20***
```kotlin
```

## ***Exercicios 21***
```kotlin
```

## ***Exercicios 22***
```kotlin
```

## ***Exercicios 23***
```kotlin
```

## ***Exercicios 24***
```kotlin
```

## ***Exercicios 25***
```kotlin
```

## ***Exercicios 1***
```kotlin
```
