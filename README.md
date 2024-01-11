# Ejercicios-examen

Exercici1.
~~~
public static void main(String[] args) {
        // TODO code application logic here
        Scanner sc = new Scanner(System.in);
        System.out.println("Escribe un numero decimal");
        int num = sc.nextInt();
        decimalBinari(num);
    }
    static void decimalBinari(int numero){
        while (numero != 0){
            int binario = numero % 2;
            numero /= 2;
            System.out.println(binario);
        }
    }
}

Exercici3.

funcion boolean esParell(int numero){
	if (numero % 2 == 0){
		return true;
	} else{
		return false;
	}
}





Exercici4.

funcion void primersNombresParells(int n){
	for(int i = 0; i <= n; i++){
		if(i % 2 == 0){
			println(i);
		}
	}
}



Exercici5.

funcion int menu(){
	println("Tria una de les següents opcions:");
	println("1. Decimal a binari");
	println("2. Binari a decimal");
	println("3. És parell?");
	println("4. Calcular parells de 0 fins a n");
	println("0. Sortir");
	return input;
}



Exercici6.

main(){
	int userinput = menu();
	switch(userinput){
		case 1:
			println("Escribe un numero entero decimal");
			int op = input;
			decimalBinari(op);
			userinput = menu();
		case 2:
			println("Escribe un numero entero binario");
			op = input;
			binariDecimal(op);
			userinput = menu();
		case 3:
			println("Escribe un numero para saber si es par o inpar");
			op = input;
			esParell(op);
			userinput = menu();
		case 4:
			println("Escribe un numero para conocer sus pares desde 0 hasta el mismo");
			op = input;
			primersNombresParells(op);
			userinput = menu();
		case 0:
			println("Adiós");
			break;
		default:
			println("Opción inválida")
			userinput = menu();
}


Exercici7.

funcion double volumCilindre(double radi, double longitud){
	if(radi <= 0 || longitud <=0){
		println("Datos incorrectos");
	} else{
		return PI * radi * radi * longitud;
	}
}

funcion double volumPrismaRectangular(double costat1, double costat2, double costat3){
	if(costat1 <= 0 || costat2 <=0 || costat3 <= 0){
		println("Datos incorrectos");
	} else{
		return costat1 * costat2 * costat3;
	}
}


Exercici8.

main(){
	println("Què has de transportar? 1. Liquids 2. Sòlids");
	int opcion = input;
	while(opcion != 1 || opcion !=2){
		println("No és una opció vàlida");
		opcion = input;
	}
	if(== 1){
		println("Quants centímetres de radi te la cisterna?")
		double radi = input;
		println("Quants centímetres de longitud te la cisterna?")
		double longitud = input;
		double volum = volumCilindre(radi, longitud);
		
	}
	if(== 2){
		println("Quants centímetres te les arestes?")
		double costat1 = input;
		double costat2 = input;
		double costat3 = input;
		volum = volumPrismaRectangular(costat1, costat2, costat3);
		
	}
	println("Quants metres cúbics hem de transportar?");
	double mcubics = input;
	double capacidad = volum/1000000;
	println(capacidad);
	println(volum);
	println(mcubics/capacidad);
}
~~~
