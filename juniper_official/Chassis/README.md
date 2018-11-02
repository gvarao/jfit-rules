# Chassis Management Healthbot KPIs
#
 
Contains readily consumable healthbot playbooks and rules which are specific to chassis key performance indicators(KPIs).
Chassis KPI rules collect the statistics from network devices, then analyze the data and act. Chassis KPI playbook is a set of
rules, where each rule is defined with a set of KPIs. Playbook contains chassis temperature, routing engine temperature, routing engine CPU temperature, FPC temperature, FAN health, PEM power usage, Zone power usage and overall system power usage rules. Rules are defined with default variable values, which can be changed while deploying the playbook.


## Usage

Apply the playbook to device-group under the playbooks section using healthbot GUI.
