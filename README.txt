StudentHub es una plataforma para gestionar servicios académicos universitario

## Preguntas de reflexión
1. ¿Diferencia entre git add y git commit?
git add mueve un cambio del working directory al staging area (lo "prepara" para el commit, pero aún no queda guardado en el historial). git commit toma lo que está en staging y lo guarda permanentemente en el historial del repositorio, con un mensaje.

2. ¿Diferencia entre git push y git pull?
git push envía tus commits locales al repositorio remoto (GitHub). git pull trae los commits que hay en el remoto y no tienes localmente, y los integra en tu rama actual.

3. ¿Diferencia entre un repositorio local y uno remoto?
El local vive en tu propia máquina y puedes trabajar sin conexión a internet. El remoto (como GitHub) es una copia centralizada, accesible por todo el equipo, que sirve como punto de sincronización entre colaboradores.

4. ¿Qué problema resuelve una rama?
Permite desarrollar cambios en paralelo sin afectar el código estable de main, aislando el trabajo en progreso hasta que esté listo para integrarse.

5. ¿Diferencia entre git merge y git rebase?
merge combina dos ramas creando un nuevo "commit de fusión" que preserva el historial tal como ocurrió (con las dos líneas). rebase reescribe los commits de una rama para que parezcan haberse creado sobre la punta actual de otra rama, dejando un historial lineal, sin commit de fusión.

6. ¿Por qué ocurre un conflicto?
Cuando dos ramas modifican las mismas líneas de un archivo (o una modifica y otra elimina el mismo contenido) de forma distinta, Git no puede decidir automáticamente cuál versión conservar.

7. ¿Quién debe decidir cómo resolver un conflicto?
La persona (o el equipo) que entiende la intención de ambos cambios — normalmente quien escribió el código en conflicto, o ambos en conjunto — nunca se debe resolver "a ciegas" borrando contenido sin revisar.

8. ¿Qué problema resuelve un Pull Request?
Formaliza y visibiliza la integración de cambios a una rama importante (como main), permitiendo discusión, revisión y control de calidad antes de fusionar.

9. ¿Por qué es recomendable revisar un PR antes de integrarlo?
Para detectar errores, mejorar la calidad del código, mantener consistencia con el resto del proyecto y compartir conocimiento entre el equipo, evitando que un solo error llegue a main sin ser visto por nadie más.

10. ¿Qué ventaja tiene trabajar en una rama en lugar de modificar main directamente?
main se mantiene siempre estable y desplegable; los cambios experimentales o en desarrollo quedan aislados y pueden probarse, revisarse o incluso descartarse sin poner en riesgo el código principal.