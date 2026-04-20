# PdM_TPfinal
Este repositorio contiene la documentación del TP final de la materia Programación de Microcontroladores (PdM) -  Protocolos de comunicación en S.E. (PCSE) del CESE

## Estructura
TPF/
├── Drivers/
│   ├── API/                   <-- Capa de Abstracción (PdM)
│   │   ├── Inc/
│   │   │   ├── API_delay.h    <-- Gestión de tiempos no bloqueantes
│   │   │   ├── API_lcd.h      <-- Funciones de alto nivel del display
│   │   │   ├── API_mpu6050.h  <-- Funciones de alto nivel de la IMU
│   │   │   ├── APILCD_port.h  <-- Interfaz de bajo nivel del LCD (PCSE)
│   │   │   └── MPU_port.h     <-- Interfaz de bajo nivel de la IMU (PCSE)
│   │   └── Src/
│   │       ├── API_delay.c    <-- Implementación de retardos no bloqueantes (PdM)
│   │       ├── API_lcd.c      <-- Lógica del LCD (PCSE)
│   │       ├── API_mpu6050.c  <-- Lógica de procesamiento de ángulos (PCSE)
│   │       ├── APILCD_port.c  <-- Driver I2C + Modo 4 bits (PdM)
│   │       └── MPU_port.c     <-- Driver I2C: Lectura/Escritura Registros(PCSE)
│   └── STM32F4xx_HAL_Driver/  <-- Capa de Hardware 
├── Core/
│   ├── Inc/
│   │   └── main.h             <-- Definiciones globales
│   └── Src/
│       └── main.c             <-- Implementación de la MEF (Tabla 1  PdM)
└── TPF.ioc            <-- Configuración de hardware (84MHz, I2C1, GPIO)



TPF/
├── Drivers/
│   ├── API/                   <-- Capa de Abstracción (PdM) [cite: 6, 22]
│   │   ├── Inc/
│   │   │   ├── API_delay.h    <-- Gestión de tiempos no bloqueantes [cite: 23, 109]
│   │   │   ├── API_lcd.h      <-- Funciones de alto nivel del display [cite: 309]
│   │   │   ├── API_mpu6050.h  <-- Funciones de alto nivel de la IMU
│   │   │   ├── APILCD_port.h  <-- Interfaz de bajo nivel del LCD (PCSE) [cite: 321]
│   │   │   └── MPU_port.h     <-- Interfaz de bajo nivel de la IMU (PCSE) [cite: 325]
│   │   └── Src/
│   │       ├── API_delay.c    <-- Implementación de retardos [cite: 34]
│   │       ├── API_lcd.c      <-- Lógica del LCD (PCSE) [cite: 309]
│   │       ├── API_mpu6050.c  <-- Lógica de procesamiento de ángulos
│   │       ├── APILCD_port.c  <-- Driver I2C + Modo 4 bits (PdM/PCSE) [cite: 241, 322]
│   │       └── MPU_port.c     <-- Driver I2C: Lectura/Escritura Registros (PCSE) [cite: 325]
│   └── STM32F4xx_HAL_Driver/  <-- Capa de Hardware (ST) [cite: 16]
├── Core/
│   ├── Inc/
│   │   └── main.h             <-- Definiciones globales
│   └── Src/
│       └── main.c             <-- Implementación de la MEF (Tabla 1 PdM) [cite: 80]
└── TPF.ioc                    <-- Configuración de hardware (84MHz, I2C1, GPIO) [cite: 113]
