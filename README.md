Sistemas anti-cheat a nivel de Kernel
Los anticheat utilizan limitaciones de la protección en modo de usuario donde utiliza controladores del kernel  y supervisa en tiempo real todos los procesos incluso los hilos. 
-	Operan con tres capas compuesta de jernel.
-	Se movio al kernel los anti-cheat porque las trampas en modo kernel manipulan directamente la memoria del juego y evadían la detección en modo usuario.
-	Para responder a esto, el anti-cheat se movió al nivel kernel, donde realiza la supervisión con el mismo nivel de privilegio.
-	Los anti-cheat responden con bloqueo de drivers, detección de hipervisores y defensa DMA basada en IOMMU.
-	Gracias a estas funciones, puede detectar cualquier manipulación en la memoria, inyecciones de código o incluso drivers que se pueden usar para engañar al juego.
-	 Precisamente en el mundo de los videojuegos donde existe una competitividad altísima, e incluso la reputación de las organizaciones está en juego, la industria defiende que esta protección es imprescindible para mantener la limpieza en los torneos.

Que procesos monitorean todos estos bloqueos.
-	registerCallBacks: Controla accesos a handles y bloquea el acceso a memoria desde procesos externos.
-	PsSetCreateProcessNotifyRoutineEx: bloquea la creación de procesos de trampas. 
-	PsSetLoadImageNotifyRoutine: detecta la carga de DLL no permitidas
-	CmRegisterCallbackEx: Monitorea cambios en el registro. 

Ricochet
La iniciativa Ricochet Anti-Cheat es un enfoque multifacético para combatir las trampas, que incluye nuevas herramientas del lado del servidor que controlan los análisis para identificar las trampas, procesos de investigación mejorados para acabar con los tramposos, actualizaciones para reforzar la seguridad de las cuentas, y mucho más. Las funciones de seguridad de Ricochet Anti-Cheat se lanzarán junto con Call of Duty.

Se identificará haciendo un sistema de detección donde correrá con el juego funcionando donde no corre si el juego no está activo.

También se creo un sistema de detección de movimiento donde analiza patrones de curvas, drift incluso el stick.
Vanguard

Ejecuta el sistema anti-cheat donde se ejecuta a nivel de arranque del ordenador incluso cuando el juego no está abierto, porque consume demasiado manteniendo los recursos abiertos incluso sin jugar por eso hay quejas de expertos de Ciberseguridad y jugadores.
Últimamente se hacen pasar por unidades de memoria modificando el firmware para que lo reconozca como una unidad de memoria y así inyectar lenguaje para trampas.
Exige que el secure boot este activado para que no se modifiquen cosas en el arranque (boot) también TPM 2.0 (trusted platform Module). El TPM verifica que el firmware  y bootloader no fueron modificados en el arranque. 
EasyAnticheat: 
 Monitorizan los archivos mientras está activo el juego, donde no reside en memoria permanentemente, juegos como: fortnite, rocket leagu y Apex.
Mismo nivel de privilegios que vanguard durante la partida, pero no tiene acceso al kernel por completo.

Fallo de CrowdStrike de 2024
Una única actualización de contenidos de Crowdstrike, una empresa de ciberseguridad que provoco la caída de 8,5 millones de sistemas donde genero disrupciones en los sistemas operativos durante días a miles de organizaciones en el mundo.
CrowdStrike es una empresa estadounidense destacada en el campo de la ciberseguridad. Se distingue por sus soluciones avanzadas en protección en la nube, seguridad de redes y servicios de respuesta a ciberataques. Su plataforma Falcon, que emplea inteligencia artificial y aprendizaje automático, permite detectar y mitigar ciberamenazas en tiempo real.
 Desde su fundación en 2011, CrowdStrike se ha consolidado como una de las soluciones más destacadas.
Provoco caídas de 5.000 millones de dólares, se calcula que el incidente de Crowdstrike costo a las aseguradoras 1.500 millones por la perdida de cobertura o interrupción de negocio.
El incidente afectó a los hosts de Windows que ejecutaban la versión 7.11 y superiores del sensor y estaban en línea entre el 19 de julio de 2024, 04:09 UTC y 05:27 UTC y recibieron la actualización. Los sistemas Apple macOS y Linux no se vieron afectados.

Origen:
Todo fue porque forzaron actualizaciones que no estaban aprobadas por los clientes.
Donde la actualización se basaba en el software antivirus para proteger los dispositivos con Microsoft de Windows de ataques maliciosos. 
Impactos:
Pérdida de productividad: Los empleados no podían trabajar en sus equipos, lo que afectó negativamente el ritmo de trabajo y las operaciones comerciales.
Daños en los sistemas: En algunos casos, la falla pudo haber ocasionado daños en los sistemas operativos, requiriendo reparaciones o reinstalaciones.
Vulnerabilidad a ciberataques: Con la protección de endpoints comprometida, las empresas se exponían a un mayor riesgo de ciberataques.
    Soluciones: 
La compañía tardo una hora y 20 minutos para crear un parche para solucionarlo, donde la naturaleza del fallo hizo difícil su despliegue, las maquinas afectadas entraban en bucle de carga donde impedía descargar actualizaciones necesarias para arreglar el problema.

 
Fuentes: 
https://ciberia.usal.es/es/noticias/fallo-global-en-software-de-crowdstrike-provoca-caos-informatico-en-millones-de-sistemas
https://es.news.hada.io/topic?id=27539
https://hardzone.es/noticias/juegos/anti-cheat-invasivos-nivel-kernel-problemas-privacidad-jugar-online/



