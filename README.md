#meow;

package Калькулятор;
import java.util.Scanner;

public class Test {
static Scanner = new Scanner(System.in);

public static void main( String[] args {
int num1 = getInt ();
int num2 = getInt (); 
char operation = getOperation();

}
public static int getInt() {
System.out.print("Введите число");


if (scanner.hasNextInt()) {
num1 = Scanner.nextInt();
} else {
sustem.out.println("Это не число...")
}
scanner.next();
num1 = getInt();
}
return num1;
}
public static char getOperation ()  {
System.out.print("Деление или умножение? Сложение или вычитание? Признавайся!");
char Operation;
if (scanner.hasNext())  {
operation =  scanner.next().charAt (0);
} else { 
System.out.println ("Это что-то не то...");
shanner.next();
operation - getOperation();
}
return operation;
}
public static int calc (int num 1, int num2, char.Operation) {
int result;
switch (operation) { 
case '+' :
result = num1 + num2;
break;

case '-';
result = num1 - num2;
break;

case '*';
result = num1 * num2;
break;

case '/';
result = num1 / num2;
break;

case '**'
result = num1 ** num2;
break;

default: 
System.out.println("Совсем не то...");

result = calc(num1, num2, getOperation());
}
return result; 
}

}
