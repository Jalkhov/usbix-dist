# Changelog

Todas las versiones notables de USBix. Formato basado en *Keep a Changelog*.

## 0.1.3

- Corregido: la descarga de la actualización fallaba porque GitHub responde con
  una **redirección (302)** que no se seguía. Ahora se siguen las redirecciones.
- Nuevo: la actualización se descarga **en segundo plano con barra de progreso**
  (tamaño y porcentaje) y opción de **cancelar**.
- Nuevo: diálogo de actualización con **novedades**, estados (descargando, lista,
  error) y botón **"Instalar y cerrar"**.
- Nuevo: tras una actualización silenciosa, USBix se **vuelve a abrir** en la bandeja.
- Corregido: ya no se duplica el aviso de "Nueva versión disponible".

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
