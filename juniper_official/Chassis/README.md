# Chassis management healthbot key performance indicators
#
** Synopsis **
 
This folder contains multiple healthbot rules and playbooks which checks the health of chassis and notifies when anomalies are found.
 
** Rule Index **
 
Rule1 : chassis-fan-health.rule –  Monitors the fan state changes and notifies anomalies.
Sensor type : iAgent
Input variables : N/A
Dependency file(s) : chassis-fan.yml
 
Rule2 : chassis-temperature.rule –  Detects the chassis temperature threshold breaches and notifies anomalies.
sensor type: open-config
Input variables : chassis_temperature_high_threshold(default value 55), chassis_temperature_low_threshold(default value 45)
Dependency file(s): No
 
Rule3 : fpc-temperature.rule – Detects the FPC temperature threshold breaches and notifies anomalies.
sensor type: open-config
Input variables : FPC_Slot_No(default value 0-9), FPC_Temperature_Higher_Threshold(default value 55), FPC_Temperature_Lower_Threshold(default value 45)
Dependency file(s) : No
 
Rule4 : pem-power-usage.rule –  Detects the PEM power usage threshold breaches and notifies anomalies.
sensor type: open-config
Input variables : pem_power_usage_threshold(default value 888888880)
Dependency file(s) : used-percentage.py
 
Rule5 : re-cpu-temperature.rule – Detects the RE CPU temperature threshold breaches and notifies anomalies.
sensor type: open-config
Input variables : RE_CPU_Temperature_Higher_Threshold(default value 55), RE_CPU_Temperature_Lower_Threshold(default value 45), RE_Slot_No(default value 0-1)
Dependency file(s) : No
 
Rule6 : system-power-usage.rule – Detects the system power usage threshold breaches and notifies anomalies.
sensor type: open-config
Input variables : system_power_usage_threshold(default value 20)
Dependency file(s) : used-percentage.py
 
Rule7 : zone-power-usage.rule – Detects the zone power usage threshold breaches and notifies anomalies
sensor type: iAgent
Input variables : zone_power_usage_threshold(default value 80)
Dependency file(s) : used-percentage.py
 
 
Playbook – chassis-kpis.playbook – Playbook contains multiple rules which checks the health of chassis and notifies when anomalies are found.
This playbook contains following rules:-
chassis.fan/check-fan-health
chassis.temperatures/check-fpc-temperature
chassis.power/check-pem-power-usage
chassis.power/check-system-power-usage
chassis.power/check-zone-power-usage
chassis.temperatures/check-chassis-temperature
chassis.temperatures/check-re-cpu-temperature
chassis.temperatures/check-re-temperature
