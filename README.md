# AprendaCSharp
*HOLA MUNDO*
//Los comentarios son definidos apartir de doble slash
//using sirve para invocar librerias utiliando nombres cortos
//las librearias deben estar referenciadas a nivel fisico
using System;
//Los proyectos de consola se componen de un namespace el cual contiene la clase de metodo
//que hara correr el programa 
//por lo cual se le conoce como entry point method
namespace HolaMundo
{
//los bloques se delimitan con curlybrackets{}
//las lineas terminan en ;
class program
static void main ()string[]args)
{
console.writeline("hola Mundo,ahora en c#!");
console.readline();
}
}
}


*CONVERSIONES*
using System;

namespace conversiones
class progam
{
static void main(string[]args)
{
//En c# las varibales son declaradas enunciando el tipo de dato seguido de el nombre de la variable y opcionalmente de un valor de inicio
string numero ="1234"
//Se muestra como representacion string(Tosting())
//del tipo de dato(gettyoe())
//de la variable(numero)
console.writeline(numero.gettype().tostring());
//se debe coonvertir a int y se muestra el tipo
int intnumero = convert.to int32(numero);
console.writeliner(intNumero.gettype().tostring());
//string.format este comando permite hacer micro substituciones
console.writeline(string.format("El nuero es (0)",
intnumero));
console.readline();
}
}
}



*ALEATORIO*
using system
{
class program
{
//la letra F se conoce como valor float
//si esta fuera de un metodo se le conoce como variable de clase
stratic public float numero1 = 24.5F;
static void main(string[]args)
{
//la declaracion dentro de un metodo hace que la variable sea local
random numAleatorio = new random();
numero2 = (float)numAleatorio.next(1,11);
console.writeline(string.format(
"La suma de {0} y {1} es {2}",
numero1, numero2, numero1 + numero2));
console.readline();
}
}
}

*ENTRADA*
using System;

namespace entrada 
{
class program
{
//a continuacion se declararan dos variables, una para preguntar la informacion y otra para recibir el valor, si es que es posible.
string valor;
int receptora=0;
Console.Write("Escribe algo");
valor =console.ReadLine();
//Se quiere comprobar si el valor capturado puede pasar a int
if (int.TryParse(valor, out receptora))
{
//si fue posible la conversion, el valor convertido se alacenara en la variable int de tranajo, y muestralo.
Console.WriteLine(
String.Format("Dato entero {0}. Muy bien!",
receptora));
}
else
{
//Si la conversion no fue exitosa, se manda un mensaje para notificarlo.
Console.WriteLine("Dato no es entero. Intentar de nuevo.");
}
//Pausa
Console.WriteLine ("");
Console.WriteLine ("Presiona INTRO para continuar");
Console.WriteLine ();
}
}
}

*NOMBRE*
using system;
using system.tex;
namespace Nombre
static void main(string[]args)
{
string nombre
string apellido
console.write("captura de nombre:");
nobre=console.readline();
//las variables se asigan su version en mayusculas
nombre = nomnre.toupper();
//stringbuilder permite evitar el fenomeno de las concatenas 
//se declara objeto stringbulder y se le asigna una nueva instancia de la clase
stringbulder nombrecompleto = new stringbuider()nombre);
nombrecompleto.append("");
nombrecompleto.append(apellido);
console.writeline(nombrecompleto);
//pausa
console.writeline("");
console.writeliner("presiona INTROpara continuar");
console.readkey;
}
}
}

*TABLA*
using system;

namespace Tabla
{

class Program
{
static void Main(string[] args)
{
//Los datos que se capturan como string es cuando son numericos, se define //a variable para el valor capturado y otro para el valor en el tipo que // ocupa 
string_numero;
int umero;
//Se pregunta el dato como string, y sse convierte a su equivalente //numerico.
  Console.Write("Dame un numero del 1 al 9: ");
  _numero=Console.ReadLine();
  numero=Convert.ToInt32(_numero);
  
  /Se genera un ciclo de numero conocido de iteraciones.
  for (int i=1; i <=10;i++)
  {
  Console.WriteLine (
  String.Format("{0}x{1}={2}",
  numero,i,numero*i));
  }
  /Pausa.
Console.WriteLine ("");
Console.WriteLine ("Presiona INTRO para continuar")
Console.ReadKey();
}
}
}

*TABLAS*
using System;

namespace Tablas
{

class Program
{
static vid main(string[]args)
{
for(int i =1; 1<= 10; i++)
{
console.writeline("");
console.writeline(string.format("tabla del (0);",i));
console.writeline("");
//las variables de secuencia permiten ser combinables cuando 
//un for esta dentro de otro for
for int j = 1; <= 10; j++)
{
console.writeline(
string.format("(0) x (1) = (2)",
i,j,i*j));
}
}
//pausa
console.writeline(");
console.writeline("presiona INTRO para continuar");
console.readkey();
}
}
}


*COMPARA*
using system
namespace compara
{
static void main(string[]args)
{
//Una vez presentados los datos de string se deberan converitr a INT y se almacenaran en //2 variables de trabajo
string_numero2,_numero2;
console.write("numero 1");
_numero1 = console.readline();
console.write(numero 2; ");
_numero2 = console.readline();
nunero1 = comvert.toint32(_numero1);
numero2 = convert.toint32(_numero2);
//un if dentro del otro ambor¿s con una salida por falso
if(numero1) == numero2)
{console.writeline(
string.foreat(
"nnumeros preporcionados (0) y (1). (2)",
numero1, numero2, "Los numeros son iguales"));
}
else
{
if (numero1>numero2)
{console.writeline(
string.format(
"numeros proporcionados (0) y (1). (2),
numero1, numero2, "los numeros son iguales"));
}
else
console.writeline(
string.format(
"numeros proporcionados (0) y (1).(2)",
numero1,numero2,"el mayor es el segundo"));
}
}
//pausa
console.writeline("");
console.writeline("presiona INTO para continuar");
console.readkey();
}
}


*ACUMULADO*

using System;
using system.collections.generic;
using system.linq;
using system.text;
usisng system.threading.tasks;

namespace Acumulado
{
class program
{
stativ void Main(string[] args)
{
string_numero;
int numero;
int acumulado=0;
Console.WriteLine("Capture los enteros a acumular.");
Console.WriteLine("Dejar vacio y dar INTRO, para salir");
Console.WriteLine(**);
//cuando se usa un ciclo while infinito, no concluye sino hasta que de manera explicita se ejecuta un break.
while(true)
{
Console.WriteLine("Dame un numero entero: ");
_numero=Console.ReadLine();
if(_numero **"")
{
break;
}
else
{
if(int.TryParse(_numero, out numero))
{
acumulado+=numero;
Console.WriteLine(String.format("Monto acumulado:{0},acumulado));
}
else
{
Console.WriteLine("El dato proporcionado no es un numero entero.");
Console.WriteLine("Intenta de nuevo");
}
}
}
//Pausa
console.writeline("");
console.writeline("presiona INTRO para continuar");
console.readkey
}
}
}

*Multiplo*
using system;

namespace Multiplo
(
class program
(
static void Main(string[] args)
(
string_numero;
int numero;
bool esMultiplo3, esMultiplo5, esMultiplo7;

try
(

Console.Write("Dame un numero entero:");
_numero=Console.ReadLine();
numero=Convert.ToInt32(_numero);
//Si un numero tiene un residual de cero con respecto a un numero, es que es un multiplo.
esMultiplo3= ((numero % 3)==0);
esMultiplo5= ((numero % 5)==0);
esMultiplo7= ((numero % 7)==0);
//Si es multiplo de 3 y de 5 al mismo tiempo, o si es multiplo de 7, correcto.
if((esMultiplo3 & esMultiplo5) | esMultiplo7)
(
Console.WriterLine("Incorrecto");
)
)
carch (Exepction =)
(
Console.WriteLine("");
Console.WriteLine("Presiona INTRO para continuar");
Console.WriteLine();
)
)
)
)
