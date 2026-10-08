Sistemas anti-cheat a nivel de Kernel
Los anticheat utilizan limitaciones de la protección en modo de usuario donde utiliza controladores del kernel  y supervisa en tiempo real todos los procesos incluso los hilos. 
-	Operan con tres capas compuesta de jernel.
-	Se movio al kernel los anti-cheat porque las trampas en modo kernel manipulan directamente la memoria del juego y evadían la detección en modo usuario.
-	Para responder a esto, el anti-cheat se movió al nivel kernel, donde realiza la supervisión con el mismo nivel de privilegio.
-	Los anti-cheat responden con bloqueo de drivers, detección de hipervisores y defensa DMA basada en IOMMU.

Que procesos monitorean todos estos bloqueos.
-	registerCallBacks: Controla accesos a handles y bloquea el acceso a memoria desde procesos externos.
-	PsSetCreateProcessNotifyRoutineEx: bloquea la creación de procesos de trampas. 
-	PsSetLoadImageNotifyRoutine: detecta la carga de DLL no permitidas
-	CmRegisterCallbackEx: Monitorea cambios en el registro. 

Vanguard

Ejecuta el sistema anti-cheat donde se ejecuta a nivel de arranque del ordenador incluso cuando el juego no está abierto, porque consume demasiado manteniendo los recursos abiertos incluso sin jugar por eso hay quejas de expertos de Ciberseguridad y jugadores.
Últimamente se hacen pasar por unidades de memoria modificando el firmware para que lo reconozca como una unidad de memoria y así inyectar lenguaje para trampas.
EasyAnticheat: 
 Monitorizan los archivos mientras está activo el juego, donde no reside en memoria permanentemente, juegos como: fortnite, rocket leagu y Apex.
Mismo nivel de privilegios que vanguard durante la partida, pero no tiene acceso al kernel por completo.

Fallo de CrowdStrike de 2024
Una única actualización de contenidos de Crowdstrike, una empresa de siberseguriad que provoco la caída de 8,5 millones de sistemas donde genero disrupciones en los sistemas operativos durante días a miles de organizaciones en el mundo.
Provoco caídas de 5.000 millones de dólares, se calcula que el incidente de Crowdstrike costo a las aseguradoras 1.500 millones por la perdida de cobertura o interrupción de negocio.
Todo fue porque forzaron actualizaciones que no estaban aprobadas por los clientes.
Donde la actualización se basaba en el software antivirus para proteger los dispositivos con Microsoft de windwos de ataques maliciosos. 
Impactos:
Pérdida de productividad: Los empleados no podían trabajar en sus equipos, lo que afectó negativamente el ritmo de trabajo y las operaciones comerciales.
Daños en los sistemas: En algunos casos, la falla pudo haber ocasionado daños en los sistemas operativos, requiriendo reparaciones o reinstalaciones.
Vulnerabilidad a ciberataques: Con la protección de endpoints comprometida, las empresas se exponían a un mayor riesgo de ciberataques.
    Soluciones: 
La compañía tardo una hora y 20 minutos para crear un parche para solucionarlo, donde la naturaleza del fallo hizo difícil su despliegue, las maquinas afectadas entraban en bucle de carga donde impedía descargar actualizaciones necesarias para arreglar el problema.
