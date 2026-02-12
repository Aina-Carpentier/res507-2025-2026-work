![schemaIsolation](schema-isolation.png)

**Where does isolation happen?**  
L’isolation a lieu entre le user et les pods, il ne peut pas communiquer avec l’app sans passer par le service et pas avec la db sans passer par l’app

**What restarts automatically?**

Tout ce qui est dans le déploiement, le pod contenant les 2 containers

**What does Kubernetes *not* manage?**

Kubernetes ne gère pas directement le stockage physique (disque dur, cloud)

![containersVsVms](containers-vs-vms.png)

**When would you prefer a VM over a container?**

Une VM a son propre OS qui tourne, permettant un usage illimité tandis qu’un container est un simple (potentiel ensemble de) processus

**When would you combine both?**

On peut combiner les 2 lorsque l’on veut isoler nos containers dans 2 systèmes différents entre eux fortement et pour des raisons de cybersécurité.
