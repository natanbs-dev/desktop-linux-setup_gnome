# BATERIA

# listando primeiramente para ver os tipos de bateria do dispositivo
``ls /sys/class/power_supply/``

# limitando em 80 a carga da bateria
``echo 80 | sudo tee /sys/class/power_supply/BAT0/charge_control_end_threshold``

# SWAPPINESS

# definindo a swappiness em 10 sabendo que o cachyos define, por padrão, 150:
``sudo sysctl vm.swappiness=10``

# verificar
``cat /proc/sys/vm/swappiness``
