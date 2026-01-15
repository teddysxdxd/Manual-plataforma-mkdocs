# PEP Cargos - Persona natural

Este paso permite capturar los datos relacionados a personas expuestas políticamente (PEP). El ingreso de datos es opcional, pero una vez creado un registro de cargos ocupados, la persona se clasifica como PEP. Serán habilitados otros pasos del flujo relacionados a personas naturales clasificadas como PEP, como la participación en empresas, parentescos y todos los datos relacionados con el cónyuge. 

![Formulario PEP Cargos](../assets/images/pep_cargos_1.png)

| Campo | Descripción | Condición |
| :--- | :--- | :--- |
| **Institución** | Nombre de la institución en donde la persona PEP ocupó un cargo público. Al ingresar algún texto, el sistema sugiere el listado de instituciones existentes con ese nombre. | Obligatorio si es una persona PEP. |
| **Cargo Ocupado** | Cargo que fue ocupado por la persona PEP en esa institución. Al ingresar algún texto, el sistema sugiere el listado de cargos existentes con ese nombre. | Obligatorio al ingresar la institución. |
| **País donde ocupó el cargo** | País en donde la persona PEP ocupó el cargo en la institución. | Obligatorio al ingresar la institución. |
| **Período en que ocupó el cargo** | Permite seleccionar el período de gobierno en el que la persona PEP ocupo el cargo. | Obligatorio al ingresar la institución. |

En este paso es realizada la creación del cliente y se asigna el estado correspondiente, dependiendo si es una persona PEP se asigna el estado pendiente de aprobación y cuando no es PEP se asigna el estado de prospección.

Después de agregar los registros de cargos ocupados por la persona PEP, se debe utilizar el botón Siguiente para continuar con el próximo paso y capturar datos relacionados a PEP. 

Al agregar el primer cargo público durante el flujo de creación de clientes, el sistema realiza la creación de cliente y asigna el estado del cliente para identificar que esta pendiente de aprobación por ser PEP.

Si no es creado ningún cargo público a la persona, al utilizar el botón Siguiente el sistema crea el cliente con estado de prospección para que pueda continuar con los demás pasos.

---

[← Volver a página anterior](crear-cliente-natural.md)