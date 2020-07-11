# hello-word
Sou analista, e estou em uma fase de criação.

# Importação
import schedule
import time

def FazerTarefaImportante():
    print('Gerando grana...')
# schedule.cada.tempo.fazer
schedule.every(10).seconds.do(FazerTarefaImportante())

while time:
    schedule.run_pending()
    time.sleep(1)
