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
    var not1 = readln().toDouble()
    var not2 = readln().toDouble()
    var not3 = readln().toDouble()
    
    var media = (not1 + not2 + not3) / 3 
    println("A média é $media")
}
```

## ***Exercicios 9***
```kotlin
fun main() {
    var segundos = readln().toInt()

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
import kotlin.math.pow

fun main(){
    var A = 0
    var B = 0
    var C = 0
    while(true){
    A = readln().toInt()
    B = readln().toInt()
    C = readln().toInt()
    if(A > 0 && B > 0 && C > 0){
        break
    } else {
        println("Todos os numeros devem ser positivos")
    }
    }
    val R = ((A + B).toDouble()).pow(2)
    val S = ((B + C).toDouble()).pow(2)
    val D = (R + S)/ 2

    
    println(D)
}
```

## ***Exercicios 12***
```kotlin
import kotlin.math.pow

fun main(){
    var custoFabrica = readln().toFloat()
    var percentagemDistribuidor = custoFabrica * 0.28
    var imposto = custoFabrica * 0.45
    var total = custoFabrica + imposto + percentagemDistribuidor
    
    println(total)
}
```

## ***Exercicios 13***
```kotlin
fun main(){
    var a = readln().toDouble()
    var b = readln().toDouble()
    var c = readln().toDouble()
    var d = readln().toDouble()
    var e = readln().toDouble()
    var f = readln().toDouble()
    
    var x = ((c * e) - (b * f)) / ((a * e) - (b * d))
    
    var y = ((a * f) - (c * d)) / ((a * e) - (b * d))
    
    println("O x = $x e o y = $y")
}
```

## ***Exercicios 14***
```kotlin
fun main(){
    var salario = readln().toDouble()
    var novoSalario = salario * 1.25
    
    println(novoSalario)
}
```

## ***Exercicios 15***
```kotlin
fun main(){
    var salario = readln().toDouble()
    var percentual = readln().toDouble()
    var novoSalario = salario * (1 + percentual / 100)
    
    println(novoSalario)
}
```

## ***Exercicios 16***
```kotlin
fun main() {
    println("Ano de Nascimento")
    var anoNascimento = readln().toInt()
    println("Mes de Nascimento")
    var mesNascimento = readln().toInt()
    println("Dia de Nascimento")
    var diaNascimento = readln().toInt()
    println("Ano atual")
    var anoAtual = readln().toInt()
    println("Mes atual")
    var mesAtual = readln().toInt()
    println("Dia atual")
    var diaAtual = readln().toInt()

    var diferencaDia = 0
    var diferencaMes = 0
    var diferencaAno = 0

    if (anoNascimento == anoAtual) {
        diferencaAno = 0  
    } else {
        diferencaAno = anoAtual - anoNascimento
    }

    if (mesNascimento > mesAtual && anoNascimento != anoAtual) {
        diferencaMes = mesNascimento - mesAtual
        diferencaAno--
        diferencaMes = 12 - diferencaMes
    } else if (mesNascimento > mesAtual && anoNascimento == anoAtual) {
        diferencaMes = mesNascimento - mesAtual
        diferencaMes = 12 - diferencaMes 
    } else {
        diferencaMes = mesAtual - mesNascimento
    }

    if (diaNascimento > diaAtual && mesNascimento >= mesAtual) {
        diferencaDia = diaNascimento - diaAtual
        diferencaMes--
        diferencaDia = 30 - diferencaDia
    } else if (diaNascimento > diaAtual && mesNascimento < mesAtual) {
        diferencaDia = diaNascimento - diaAtual
        diferencaDia = 30 - diferencaDia
    } else {
        diferencaDia = diaAtual - diaNascimento
    }

    if (diferencaDia == 30) {
        diferencaDia = 0
    }
    println("Você tem $diferencaAno ano(s), $diferencaMes mes(es) e $diferencaDia dia(s)")
}
```

## ***Exercicios 17***
```kotlin
fun main(){
    var sacoRacao = readln().toDouble()
    var racaoParaGato = readln().toInt()
    
    var gastoTotal = (sacoRacao * 1000) - ((racaoParaGato * 2) * 5)
    
    println("O gasto total foi $gastoTotal")
}
```

## ***Exercicios 18***
```kotlin
fun main(){
    var A = readln().toInt()
    var B = readln().toInt()
    var temp = B
    println("Antes")
    println("Valor A = $A")
    println("Valor B = $B")
    B = A
    A = temp
    println("Depois")
    println("Valor A = $A")
    println("Valor B = $B")
}
```

## ***Exercicios 19***
```kotlin
fun main(){
    var comprimento = readln().toInt()
    var largura = readln().toInt()
    var altura = readln().toInt()
    
    var volume = comprimento * altura * largura
    
    println(volume)
}
```

## ***Exercicios 20***
```kotlin
import kotlin.math.pow

fun main(){
    var A = readln().toDouble()
    var B = readln().toDouble()
    
    var quadrado = (A - B).pow(2)
    
    println(quadrado)
}
```

## ***Exercicios 21***
```kotlin
fun main() {
    var valorDolar = readln().toDouble()
    var cotacaoDolar = readln().toDouble()
    
    var valorReal = valorDolar * cotacaoDolar
    
    println(valorReal)
    
}
```

## ***Exercicios 22***
```kotlin
import kotlin.math.pow

fun main() {
    var A = readln().toDouble()
    var B = readln().toDouble()
    var C = readln().toDouble()
    
    var quadradoResultado = (A + B + C).pow(2)
    
    println(quadradoResultado)
}
```

## ***Exercicios 23***
```kotlin
fun main() {
   var val1 = readln().toDouble()
   var val2 = readln().toDouble()
   var adi = val1 + val2
   var sub = val1 - val2
   var mul = val1 * val2
   var div = val1 / val2
   
   println("Adição: $val1 + $val2 = $adi")
   println("Subtração: $val1 - $val2 = $sub")
   println("Mutiplicação: $val1 * $val2 = $mul")
   println("Divisão: $val1 / $val2 = $div")
   
}
```

## ***Exercicios 24***
```kotlin
import kotlin.math.pow

fun main() {
    var raio = readln().toDouble()
    val pi = 3.1459
    var volume = (4/3) * pi * raio.pow(3)
    
    println(volume)
}
```

## ***Exercicios 25***
```kotlin
fun main() {
    var num = readln().toInt()
    var sucessor = num + 1
    var antecessor = num - 1

    println("Sucessor = $sucessor. Antecessor = $antecessor")
}
```
