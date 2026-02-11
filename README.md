# Atividades-de-L-gica-de-Programa-o-em-Kotlin---SENAI

// ---- Lista 02 ---- //
// ---- Calculo De IMC ---- //

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
