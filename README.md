# hello-word
Sou analista, e estou em uma fase de criação.

# Importar bibliotecas
import schedule
import time

# Configurações
def sudo_placement(): 
    print("Get ready for Sudo Placement at Geeksforgeeks") 
  
def good_luck(): 
    print("Good Luck for Test") 
  
def work(): 
    print("Study and work hard") 
  
def bedtime(): 
    print("It is bed time go rest") 
      
def geeks(): 
    print("Shaurya says Geeksforgeeks") 
  
# Agendamento de tarefas (scheduling) 
#   Após min
schedule.every(10).minutes.do(geeks) 
# Após Horas 
schedule.every().hour.do(geeks) 
# Após dias 
schedule.every().day.at("00:00").do(bedtime) 
# Após intervelos de tempo em minutos 
schedule.every(5).to(10).minutes.do(work) 
# Dias da semana  
schedule.every().monday.do(good_luck) 
# Dis da semana com horas determinada 
schedule.every().tuesday.at("18:00").do(sudo_placement) 

# While com loop de agendamento que confinua funcionando todo tempo enquanto for verdadeiro
while True: 
    schedule.run_pending() 
    time.sleep(1) 
