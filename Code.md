import java.util.Scanner;
public class CalculadoraAgendamentos {
public static void main(String[] args) {
	Scanner input = new Scanner(System.in);
	System.out.println("Digite o horário do agendamento");
	int hr = input.nextInt();
	
	while (hr < 0 || hr > 23) {
		System.out.println("Hora invalida, digite novamente");
		hr = input.nextInt();
	}
	System.out.println("Digite os minutos");
	int min = input.nextInt();
	
	while (min < 0 || min > 59) {
		System.out.println("Minuto invalido, digite novamente");
		min = input.nextInt();
	}
	System.out.println("Digite os segundos");
	int sec = input.nextInt();
	
	while (sec < 0 || sec > 59) {
		System.out.println("Segundos invalidos, digite novamente");
		sec = input.nextInt();
	}
    if (hr < 10 & min < 10 & sec < 10) {
    	System.out.println("O horário do agendamento foi: " + "0" + hr + "hr" + "0"+ min + "min" + "0" + sec + "seg");
    }
    else {
    	System.out.println("O horário do agendamento foi: " + "0" + hr + "hrs" + min + "min" + sec + "seg");
    }
}
}
