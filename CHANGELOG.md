# Changelog

Todas las versiones notables de USBix. Formato basado en *Keep a Changelog*.

## 0.1.2

- Añadido: **notas de versión** (novedades) que la app muestra antes de actualizar.
- Añadido: changelog y notas en el repositorio de distribución.
- Mejora: el manifest firmado incluye las notas, así que vienen autenticadas.

## 0.1.1

- Corregido: la comprobación de actualizaciones **fallaba en Windows 7** (tipo de
  proxy de WinHTTP inexistente en ese sistema).
- Corregido: el resultado de la comprobación no se mostraba en `Ajustes`.
- Mejora: versión centralizada en el archivo `VERSION`.

## 0.1.0

- Primera versión: detección de virus de USB (autorun, `.lnk`, doble extensión,
  ADS, ejecutables empaquetados), desinfección con cuarentena, restauración de
  atributos, vacunación con ACLs, auditoría de persistencia, blindaje de escritura
  y canal de actualizaciones firmado (Ed25519).
