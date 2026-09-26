# Changelog

Todas las versiones notables de USBix.

El formato sigue [Keep a Changelog](https://keepachangelog.com/es/1.1.0/). Cada
versión agrupa sus cambios en secciones **en este orden fijo**: `Añadido`,
`Cambiado`, `Corregido`, `Eliminado` (se omiten las que queden vacías).

## 0.1.3 - 2026-09-25

### Añadido

- Descarga de la actualización **en segundo plano**, con barra de progreso
  (tamaño y porcentaje) y botón de **cancelar**.
- Diálogo de actualización con las **novedades** y estados claros (descargando,
  lista, error), con el botón **"Instalar y cerrar"**.
- Tras una actualización silenciosa, USBix se **vuelve a abrir** en la bandeja.

### Corregido

- La descarga de la actualización fallaba porque GitHub responde con una
  **redirección (302)** que no se seguía.
- Ya no se duplica el aviso de "Nueva versión disponible".

## 0.1.2 - 2026-09-25

### Añadido

- **Notas de versión** (novedades) que la app muestra antes de actualizar.
- Changelog y notas en el repositorio de distribución.

### Cambiado

- El manifest firmado incluye las notas, así que llegan **autenticadas**.

## 0.1.1 - 2026-09-25

### Cambiado

- Versión centralizada en el archivo `VERSION`.

### Corregido

- La comprobación de actualizaciones **fallaba en Windows 7** (tipo de proxy de
  WinHTTP inexistente en ese sistema).
- El resultado de la comprobación no se mostraba en `Ajustes`.

## 0.1.0 - 2026-09-25

### Añadido

- Primera versión: detección de virus de USB (autorun, `.lnk`, doble extensión,
  ADS, ejecutables empaquetados), desinfección con cuarentena, restauración de
  atributos, vacunación con ACLs, auditoría de persistencia, blindaje de escritura
  y canal de actualizaciones firmado (Ed25519).
