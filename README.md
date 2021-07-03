# appium

#Przygotowanie CLI gmsaas

$sudo apt install python3-pip

$pip3 install gmsaas

#zalogowanie się na konto w cloud.geny.io

$ gmsaas auth login [EMAILUZYTYDOKONTAGENYMOTION@EMAIL.COM]

#uruchamianie zadalne instancji

$ gmsaas instances start <recipe_uuid> <name>

#Zatrzymanie zdalne instancji aktualne działających
  
$ gmsaas instances list -q | xargs -n1 gmsaas instances stop --no-wait

#zatrzymanie dzialania dla konkretnej instancji
  
$ gmsaas instances stop <instance_uuid>

#Wyświetlenie aktualnie działających "instancji"
  
$ gmsaas instances list

#wypisz konfiguracje androidów z genymotio
  
$ gmsaas recipes list
