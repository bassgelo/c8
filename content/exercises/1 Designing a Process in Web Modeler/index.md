---
title: '1 Designing a process'
weight: 2
---

## Background

In this exercise you are asked to design a process using BPMN and DMN. The scenario description can be found in the next section. To model it use the Camunda 8 Web Modeler https://modeler.cloud.camunda.io/.

### Task: Model the following process.

We are designing a process to manage the quarantine of persons infected with HZV - the "Hypothetical Zombie Virus". Statistically, 5% of people who are infected with the Zombie Virus turn into actual undead Zombies, with an insatiable craving to eat human brains. The other 95% experience mild symptoms - mostly an extreme craving for ice cream.

In order to stop the spread of the undead and the collapse of modern civilisation, you have been tasked with designing and automating a quarantine process using Camunda Platform 8.

The virus has a different effect in different age groups. People aged 30 and under recover faster, and they can be cleared of the danger of turning into Zombies in 5-7 days. People over 30 can turn into Zombies anywhere up to 10 days.

In order to keep society running, it's an acceptable risk to release people under 31 years of age from quarantine at the lower bound of their risk period (5 days), if they work in a "critical infrastructure" role (like a power plant) - we're balancing the collapse of civilization from brain-eating Zombies or a collapse from a runaway nuclear power plant here.

When someone tests positive for the HZV the Health Department is informed. They immediately contact the infected person and notify them to quarantine, and for how long, then check on them regularly - every two days. If the person turns into a Zombie during the quarantine period, the quarantine process ends, and another process is started.

When the quarantine period ends without the person turning into a Zombie, the Health Department issues a digital recovery certificate and sends it to the person. This certificate can be used to get a 10% discount at participating ice-cream retailers.

With all of this information in hand, it's up to you to create the best possible quarantine process using Camunda 8 Web Modeler, keeping the various contingency plans and timelines in mind.

Need a hint? One solution can be found in the git repo link.

You may like to refer to the https://docs.camunda.io/docs/components/modeler/bpmn/bpmn-primer/ and the docs for https://docs.camunda.io/docs/components/modeler/dmn/ in the Camunda 8 documentation.