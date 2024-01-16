# SWIIIJulcamoroBrandonAlquiler
Identificación de Subdominios
# Gestión de alquileres 
Permite  los usuarios realizar reservas de vehículos, rastrear el estado y la disponibilidad de la flota de vehículos. Generar y gestionar contratos de alquiler
Tipo de dominio: Es un core Domain porque representa el proceso de alquiler de los vehículos que mejora la experiencia del usuario en us visita. Esto le genera ventaja competitiva
# Gestión de pagos
Porcesa pagos de los clientes de forma segura. Genera facturas y recibos para cada transacción
Tipo de dominio: Es un core domain porque representa una parte fundamental del proceso de adquisición de vehículos.
# Gestión de vehículos
Gestiona la flota de vehículos, incluyendo detalle de  mantenimiento, características y disponibilidad. Registrar y rastrear el historial de servicio de cada vehículo.
Tipo de dominio: El subdominio de Gestión vehículos es un Support Domain ya que permite garantizar que los productos estén disponibles para los clientes. Sin embargo, no es esencial para el funcionamiento del negocio
# Gestión de clientes   
Mantiene la información actualizada de los clientes, incluyendo perfiles y preferencias. Facilita la creación de cuentas de usuario para los turistas.
Tipo de dominio: El subdominio Clientes es un Support Domain, ya que su función principal consiste en complementar el proceso de alquiler de vehículos. Aunque no es el núcleo central, desempeña un papel estratégico en el fortalecimiento de la relación entre el cliente y el negocio.
# Seguridad 
Implementar un sistema robusto de autenticación y autorización para garantizar la seguridad de los datos. Establecer políticas de seguridad que apliquen a todos los aspectos del sistema.
Tipo de Dominio:  El subdominio seguridad es un Generic Domain porque contiene autenticación y autorización que podría ser reutilizados en otros proyectos y adaptarse a las necesidades específicas de cada negocio.

## Patrones Utilizados
# Gestión de Clientes y Seguridad
    Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales y como se incluye al contexto Seguridad entonces, para acceder a este contexto. El contexto Clientes debe pasar por la capa ACL para entender al contexto Seguridad.
# Seguridad y Gestión de pagos 
    Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales y como se incluye al contexto Seguridad entonces, en ambos contextos se guardan datos confidenciales.
# Gestión pagos y Gestión clientes
    Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales en los contextos pagos y clientes.
# Gestión de vehículos y gestión de pagos
    Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales en el contexto pago
# Gestión de Pagos y Gestión de Alquileres
     Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales en este caso en el contexto pagos.
# Seguridad y Gestión de Alquileres
     Utilizamos la capa ACL porque se pide que se garantice la protección de datos confidenciales en el contexto seguridad con respecto a alquileres
# Gestión de Vehículos y Gestión de Clientes
    Se utiliza un patrón conformista porque el contexto vehículo no tiene motivación para traducir su lenguaje ubicuo al contexto Gestión Clientes pues se trata de cosas distintas
# Gestión de Alquileres y Gestión de Vehículos
    Utilizamos una asociación porque se espera que haya una buena comunicación entre ellos y para eso el partner ship permite tener objetivos alineados y trabajar conjuntamente en múltiples reuniones.

