# Healthbot LLDP KPIs
#
 
Contains readily consumable healthbot playbooks and rules which are specific to LLDP neighbor key performance indicators(KPIs). LLDP KPI rules collect the statistics from network devices, then analyze the data and act. LLDP KPI playbook is a set of rules, where each rule is defined with a set of KPIs. Playbook contains lldp session state, lldp statistics i.e. frame discards, frame in errors, frame out erros, tlv discards and unknown tlv rules. Rules are defined with default variable values, which can be changed while deploying the playbook.


## Usage

Apply the playbook to device-group under the playbooks section using the healthbot GUI.
