# Grupo 9 Ejercicio Guiado: Seguridad Integrada con DevSecOps

## Paso 2

## ¿Qué dependencias tienen vulnerabilidades?

    - connect:2.6.0
    - cookie:0.0.4
    - express:3.0.0
    - fresh:0.1.0
    - jquery.js
    - mime:1.2.6
    - qs:0.5.1
    - send:0.0.4

## ¿Qué versiones se sugiere actualizar?

    - connect:2.6.0 : A la más actualizada o desactivar methodOverride
    - cookie:0.0.4: Actualizar a 0.7.0
    - express:3.0.0: Actualizar a 3.11 o superior
    - fresh:0.1.0: Actualizar a 0.5.2 o superior
    - jquery.js: quitar
    - mime:1.2.6: Actualizar 2.0.3 o superior
    - qs:0.5.1: Actualizar a 6.0.4, 6.1.2, 6.2.3, 6.3.2 o superior
    - send:0.0.4: Actualizar a 0.11.1 o superior

## Paso 3

## ¿Cuántas vulnerabilidades detecta Trivy?

safenotes-app (debian 10.13)
Total: 7647

## ¿Cuál es su nivel de severidad?

Total: 7647 (UNKNOWN: 12, LOW: 1385, MEDIUM: 4674, HIGH: 1536, CRITICAL: 40)

## Paso 4

## ¿Se detectaron posibles ataques XSS, headers inseguros o vulnerabilidades CSRF?

Se detecto lo siguiente:
Cabecera Content Security Policy (CSP) no configurada
Falta de cabecera Anti-Clickjacking
El servidor divulga información mediante un campo(s) de encabezado de respuesta HTTP ''''X-Powered-By''''
Falta encabezado X-Content-Type-Options

## Preguntas finales

## ¿Qué aprendiste sobre la diferencia entre SAST, DAST y SCA?

Static Application Security Testing (SAST): Identifica vulnerabilidades sin ejecutar el código.
Dynamic Application Security Testing (DAST): Identifica vulnerabilidades en tiempo de ejecución.
Software Composition Analysis (SCA): Analiza las dependecias del software.

## ¿Qué herramientas fueron más fáciles de implementar?

 Dependency Check y Trivy se ejecutaron sin problemas. ZAP requirio configuración de proxy y una excepción de seguridad en macos.

## ¿Cómo DevSecOps mejora la seguridad sin frenar el desarrollo?

Al integrar la seguridad en cada etapa del desarrollo es posible resolver los problemas en etapas tempranas del desarrollo, lo que permite no atrasar las entregas.

## ¿Qué parte del proceso automatizarías completamente en una empresa?

Tanto SAST, DAST y SCA es posible agregarlas a los procesos de forma automática.
