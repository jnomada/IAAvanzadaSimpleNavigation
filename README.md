# Descripción
# IA Avanzada Simple Navigation
### Cambios en el proyecto

- He duplicado various de los cubos (que ya tienen collider) para crear una "puertecita" pequeña por donde pasará el nuevo agente cuando le conviene para llegar al distino de forma más rápida. Estos van debajo del padre "Gates".
- He creado un Agente nuevo llamado "DwarfAgent", al cual he añadido el componente **Nav Mesh Agent**.
- Luego he creado un nuevo **Agent Type** llamado "Dwarf" y le he dado un radio y altura de 0.34, step height de 0.3. Este lo he asignado como Agent Type en el NavMesh Agent.
- En el **Obstacle Avoidance** he puesto el **Radius** y **Height** a 0.34. La velocidad del **Steering** a 6.
- En el **Geometry** he añadido un nuevo **NavMesh Surface** con el Agente Type puesto en "Dwarf". A los tres Navmesh Surface los he "bakeado" para que sepa cada agente por donde puede caminar (recalcular) ya que he cambiado un poco la estructura del escenario.
- Al nuevo agente le he adjuntado el mismo script que los ya existentes para que vaya al punto que marca el rayo al hacer clic del ratón.

[Vínculo al repositorio en Github](https://github.com/jnomada/IAAvanzadaSimpleNavigation)
