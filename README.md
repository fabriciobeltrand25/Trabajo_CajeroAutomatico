# Cajero Automatico Proyecto Programacion Web 2

**Grupo #7**

**Integrantes:**

- **Fabricio Antonio Romero** — #202410080063  
- **Erik Francisco Pineda** — #202310011128  
- **Rony Enrique Barahona** — #202410060998  

---

## Tarea Segundo Parcial

---

# Tecnologías utilizadas

- Java  
- JSF (Jakarta Faces)  
- PrimeFaces  
- Maven  
- Tomcat

---

# Funcionalidades del sistema

El sistema cuenta con las siguientes operaciones:

### Depósitos
Permite ingresar dinero a una cuenta válida.

### Retiros
Solo se permite si el saldo es suficiente.

### Consulta de saldo
Muestra el saldo actual del cliente.

---



# Archivo de datos

En el proyecto se encuentra el archivo **TXT** de datos con los datos de los clientes y los pines.

Ejemplo:

Formato

```
Cuenta, PIN, MONTO
1001,1234,5000
1002,1111,3000
1003,2222,1500
1004,3333,8000
1005,4444,2000
```

---

# Instalación del proyecto

A continuación se muestran los pasos básicos para ejecutar el proyecto en el IDE **IntelliJ**.

---

## Paso 1: Importar el proyecto (Clonar URL de Github)

https://github.com/fabriciobeltrand25/Trabajo_CajeroAutomatico

No es necesario crear el proyecto desde cero.

1. Abre tu IDE (**IntelliJ**).
2. Selecciona **Open** si se clonó el repositorio desde **Github Desktop**.
3. Si no, selecciona **Clone Repository** y clona directamente el proyecto.
4. **Importante:** seleccionar el archivo **pom.xml**.

El IDE reconocerá automáticamente que es un proyecto **Maven** y descargará todas las dependencias necesarias.  

Si no lo hace:

- Dar click derecho en el **pom.xml**
- Seleccionar **Add as Maven Project**

---

## Paso 2: Actualizar dependencias Maven

En algunos casos el IDE no descarga las dependencias automáticamente.

Para solucionarlo:

1. Ir a la pestaña **Maven** (normalmente en el lado derecho del IDE).
2. Presionar el botón **Reload** (icono de flechas circulares).
3. Esperar a que termine la descarga.

Esto instalará las librerías necesarias.

---

## Paso 3: Ejecutar el servidor

Para ejecutar la aplicación web usaremos el servidor de aplicaciones **Tomcat**.

Pasos generales:

1. Ir a **Add Configuration**
2. Presionar **+**
3. Seleccionar **Tomcat Server → Local**
4. Definir la ruta de donde está instalado el **Tomcat**
5. Seleccionar el **JDK**
6. En la pestaña **Deployment**
7. Presionar **+**
8. Seleccionar **Artifact** : Cajero.AutomatiocoJsf : war exploded
9. Elegir el que dice:

Finalmente:

Presionar el botón **Run / Play** para iniciar el servidor.

---

# Uso del sistema

Al iniciar la aplicación aparecerá el menú principal con tres opciones:

- Depositar  
- Retirar  
- Consultar  

Cada operación solicita:

- Número de cuenta  
- PIN de seguridad  

El sistema validará la información y mostrará el resultado de la operación.

---

# Notas

- Los datos de clientes se cargan desde un archivo **Clientes.txt**, que se encuentra en la carpeta de **Resources**.
- Las operaciones actualizan el saldo del cliente en memoria.
- La interfaz fue construida usando **PrimeFaces** para mejorar la presentación visual.
