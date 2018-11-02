# Healthbot default KPIs
Contains readily consumable healthbot playbooks and rules which are specific to chassis, linecard, system, interface and protocols key performance indicators(KPIs). KPI rules collect the statistics from network devices, then analyze the data and act.

The KPI playbook is a set of rules, where each rule is defined with a set of KPIs.

Playbooks for chassis, linecard, system, interface and protocols(bgp, lldp, rib) are available in respective folders.

Rules are defined with default variable values, which can be changed while deploying the playbook.

## Usage
Apply the playbook to device-group under the playbooks section using the HealthBot GUI.
