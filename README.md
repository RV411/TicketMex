# TicketMex


### USUARIO

```mermaid

flowchart TB
    subgraph PRIMERO
    Ingresar_a_la_pagina-->Ver_Categorias
    end
    subgraph PRIMERO
    Ingresar_a_la_pagina-->Registrarse
    end
    subgraph PRIMERO
    Ingresar_a_la_pagina-->Ingresar
    end
    Registrarse-->Teclear_Datos
    Ingresar-->Teclear_Datos
    subgraph SEGUNDO
    Ver_Categorias-->Ver_Eventos
    end
    subgraph SEGUNDO
    Ver_Eventos-->Mostrar_Pagina
    end
    Mostrar_Pagina-->Seleccionar_Evento
    Seleccionar_Evento-->Registrarse
    Seleccionar_Evento-->Ingresar
    Acceder_a_la_página-->Seleccionar_Evento
    subgraph TERCERO
    Teclear_Datos-->Acceder_a_la_página
    end
    subgraph CUARTO
    Seleccionar_Evento
    end
    
```

### ADMINISTRADOR

```mermaid

flowchart TB
    subgraph PRIMERO
    Ingresar_a_la_pagina-->Ingresar
    end
    Ingresar-->Teclear_Datos
    subgraph SEGUNDO
    Teclear_Datos-->Acceder_a_la_página_de_administrador
    end
    Acceder_a_la_página_de_administrador-->Administrar_Eventos
    subgraph TERCERO
    Administrar_Eventos-->Crear_Evento
    end
    subgraph TERCERO
    Administrar_Eventos-->Actualizar_Evento
    end
    subgraph TERCERO
    Administrar_Eventos-->Eliminar_Evento
    end    
```
