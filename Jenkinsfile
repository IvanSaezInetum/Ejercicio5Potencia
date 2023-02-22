def num1 = 4
def num2 = 5
pipeline {
    agent any
    stages {
        stage('Calculadora') {
            steps {
                script {
                     def suma = num1 + num2
                def potencia = suma**2
                def info = "La suma de " + num1 + " + " + num2 + " es " + suma + " y la potencia de la suma es " + potencia
                
                writeFile(file: "salida.txt", text: info)
                def read = readFile(file: "salida.txt")
                println read
                }
               
            }
        }
    }
    
}
