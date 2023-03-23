import java.util.Scanner;
import java.time.LocalDateTime;
public class atividadefametro {
public static void main(String[] args) {
	Scanner input = new Scanner(System.in);
	LocalDateTime now = LocalDateTime.now();
	
	int meslocal = now.getMonthValue();
	int dialocal = now.getDayOfMonth();
	int horalocal = now.getHour();
	int minutolocal = now.getMinute();
	
	System.out.println("Digite o numero do mês que foi marcado o agendamento");
	int mes = input.nextInt();
	 
	while (mes < meslocal) {
		System.out.println("Este mês já passou, tente novamente");
		mes = input.nextInt();
	}
	boolean dia_valido = false;
	int dia = 0;
	
	String nomeMes = "";
    switch(mes) {
      case 1:
        nomeMes = "Jan";

        while (!dia_valido) {
          System.out.print("Digite o dia do agendamento");
          dia = input.nextInt();

          while (dia < dialocal) {
  			System.out.println("Este dia já passou, tente novamente");
  			mes = input.nextInt();
  		}
          while (dia < 0) {
  			System.out.println("Invalido, tente novamente");
  			mes = input.nextInt();
  		}
          if (dia >= 1 && dia <= 31) {
            dia_valido = true;
          } else {
            System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
          }
        }  break;
        
       case 2:
    	   nomeMes = "Fev";
    	while (!dia_valido) {
    	  System.out.print("Digite o dia do agendamento");
    	  dia = input.nextInt();

    	  while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
    	  while (dia < 0) {
    			System.out.println("Invalido, tente novamente");
    			mes = input.nextInt();
    		}
    	   if (dia >= 1 && dia <= 31) {
    	     dia_valido = true;
    	   } else {
    	     System.out.println("Dia inválido. Insira um valor entre 1 e 28.");
    	   }
    	 }  break;
    	 
       case 3:
    	   nomeMes = "Mar";
       	while (!dia_valido) {
       	  System.out.print("Digite o dia do agendamento");
       	  dia = input.nextInt();

       	while (dia < dialocal) {
			System.out.println("Este dia já passou, tente novamente");
			mes = input.nextInt();
		}
       	while (dia < 0) {
  			System.out.println("Invalido, tente novamente");
  			mes = input.nextInt();
  		}
       	   if (dia >= 1 && dia <= 31) {
       	     dia_valido = true;
       	   } else {
       	     System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
       	   }
       	 }  break;
       	 
       case 4:
    	   nomeMes = "Abr";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 30.");
          	   }
          	 }  break;
          	 
       case 5:
    	   nomeMes = "Mai";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
          	   }
          	 }  break;
          	 
       case 6:
    	   nomeMes = "Jun";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();
          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 30.");
          	   }
          	 }  break;
          	 
       case 7:
    	   nomeMes = "Jul";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
          	   }
          	 }  break;
          	 
       case 8:
    	   nomeMes = "Ago";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();
          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 30.");
          	   }
          	 }  break;
          	 
       case 9:
    	   nomeMes = "Set";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();
          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
          	   }
          	 }  break;
          	 
       case 10:
    	   nomeMes = "Out";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 30.");
          	   }
          	 }  break;
          	 
       case 11:
    	   nomeMes = "Nov";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 31.");
          	   }
          	 }  break;
          	 
       case 12:
    	   nomeMes = "Dez";
          	while (!dia_valido) {
          	  System.out.print("Digite o dia do agendamento");
          	  dia = input.nextInt();

          	while (dia < dialocal) {
    			System.out.println("Este dia já passou, tente novamente");
    			mes = input.nextInt();
    		}
          	while (dia < 0) {
      			System.out.println("Invalido, tente novamente");
      			mes = input.nextInt();
      		}
          	   if (dia >= 1 && dia <= 31) {
          	     dia_valido = true;
          	   } else {
          	     System.out.println("Dia inválido. Insira um valor entre 1 e 30.");
          	   }
          	 }  break;
   }
	while (mes < 1 || mes > 12) {
		System.out.println("Mês invalido, digite novamente");
		mes = input.nextInt();
	}
	
	System.out.println("Digite a hora marcada do agendamento");
	int hr = input.nextInt();
	
	while (hr < 0 || hr > 23) {
		System.out.println("Hora invalida, digite novamente");
		hr = input.nextInt();
	}
	System.out.println("Digite o minuto");
	int min = input.nextInt();
	
	while (min < 0 || min > 59) {
		System.out.println("Minuto invalido, digite novamente");
		min = input.nextInt();
	}
	
	int resuMes = meslocal - mes;
	int resuDia = dialocal - dia;
	int resuHora = horalocal - hr;
	int resuMin = minutolocal - min;
	
	if (resuMes < 10 || resuDia < 10 || resuHora < 10 || resuMin < 10) {
	    System.out.println("Faltam 0" + resuMes + " meses " + " 0" + resuDia + " dias " + " 0" + resuHora + " horas " + " 0" + resuMin + " minutos");
	} else if (resuMes < 10 || resuDia < 10 || resuHora < 10) {
	    System.out.println("Faltam 0" + resuMes + " meses " + " 0" + resuDia + " dias " + " 0" + resuHora + " horas " + resuMin + " minutos");
	} else if (resuMes < 10 || resuDia < 10) {
	    System.out.println("Faltam 0" + resuMes + " meses " + " 0" + resuDia + " dias " + resuHora + " horas " + resuMin + " minutos");
	} else if (resuMes < 10) {
	    System.out.println("Faltam 0" + resuMes + " meses " + resuDia + " dias " + resuHora + " horas " + resuMin + " minutos");
	} else {
	    System.out.println("Faltam " + resuMes + " meses " + resuDia + " dias " + resuHora + " horas " + resuMin + " minutos");
	}
    
}
}
//EIMM∴