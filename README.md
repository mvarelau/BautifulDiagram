# BautifulDiagram
Elija un problema de la vida real (sistema de gestión de biblioteca, negocio de compra-venta, automóvil, etc) que se pueda modelar a través de objetos y clases. Plantee las relaciones de clases, composiciones, propiedades y comportamientos del sistema en uno mas diagramas tipo UML.
Yo escogí el trasporte masivo.
```mermaid
classDiagram
    Bus <|-- Troncal
    Bus <|-- Urbano
    Bus <|-- Alimentador
    Bus <|-- Complementario 
    Bus <|-- Especial
    class Bus{
        +Transmilenio
        +Color()
    }
    class Troncal{
     
      +Ruta(Se debe describir con varias palabras)
    
    }
    class Urbano{
    
      +Ruta()
    }
    class Alimentador{
      
      +Ruta()
    }
    class Complementario{
        
        +Ruta()
    }
    class Especial{
      
      +Ruta()
    
    }
    class Estación{
        +Ubicación
        +Nombre()
    }
    class MedioTransporte{
        +Tipo
        +Público?
    }
    Estación <-- Usuario: llega 
    Bus <-- Estación
    MedioTransporte --*Bus
```
``
