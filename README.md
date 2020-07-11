# hello-word
Sou analista, e estou em uma fase de criação.

# Importação
import schedule
import time

# Definir tarefa impoprtante
def TarefaImportante():
    print('Gerando grana...')
# schedule.cada.tempo.fazer
schedule.every(10).seconds.do(TarefaImportante)

while time:
    schedule.run_pending()
    time.sleep(1)
