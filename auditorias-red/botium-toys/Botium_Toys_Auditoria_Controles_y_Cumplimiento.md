# Botium Toys — Lista de comprobación de controles y conformidad

_Fecha:_ 2025-08-18

> Esta lista se completó en base al informe de alcance, objetivos y evaluación de riesgos de Botium Toys y al documento de categorías de controles.

## 1) Controles — ¿Existen hoy?

| Control | ¿Existe? | Evidencia breve |
|---|---|---|
| Mínimo privilegio (Least Privilege) | No | Todos los empleados pueden acceder a datos internos y posiblemente a datos de tarjetas y PII/SPII. |
| Planes de recuperación ante desastres (DRP) | No | No existen planes de recuperación ante desastres. |
| Políticas de contraseñas | Sí (débil) | Existe una política, pero no cumple requisitos mínimos actuales. |
| Separación de funciones (SoD) | No | No se ha implementado la separación de funciones. |
| Firewall | Sí | Firewall activo con reglas definidas. |
| Sistema de detección de intrusiones (IDS) | No | No se ha instalado un IDS. |
| Copias de seguridad (Backups) | No | No hay copias de seguridad de datos críticos. |
| Antivirus | Sí | Antivirus instalado y monitorizado por TI. |
| Monitoreo/mantenimiento manual de sistemas legacy | Sí (mejorable) | Se realiza, pero sin una planificación periódica clara. |
| Cifrado | No | No se utiliza cifrado para proteger datos de tarjetas. |
| Gestor de contraseñas | No | No existe un sistema centralizado de gestión de contraseñas. |
| Cerraduras físicas (oficinas/tienda/almacén) | Sí | Instaladas y operativas. |
| CCTV | Sí | Vigilancia CCTV actualizada. |
| Detección y prevención de incendios | Sí | Sistemas de alarma y prevención funcionando. |

## 2) Cumplimiento — Mejores prácticas

### PCI DSS
| Práctica | ¿Cumple hoy? |
|---|---|
| Solo usuarios autorizados acceden a datos de tarjeta | No |
| Datos de tarjeta se almacenan/procesan/transmiten de forma segura | No |
| Se implementa cifrado en los puntos de transacción y datos | No |
| Políticas seguras de gestión de contraseñas | No |

### GDPR
| Práctica | ¿Cumple hoy? |
|---|---|
| Los datos de clientes de la UE se mantienen privados/seguros | No |
| Plan para notificar a clientes de la UE en ≤72 h ante brecha | Sí |
| Datos correctamente clasificados e inventariados | No |
| Se hacen cumplir políticas/procedimientos de privacidad | Sí |

### SOC 1 / SOC 2
| Práctica | ¿Cumple hoy? |
|---|---|
| Políticas de control de acceso de usuarios establecidas | No |
| PII/SPII es confidencial/privada | No |
| Integridad de datos (consistencia, completitud, validación) | Sí |
| Disponibilidad de datos para usuarios autorizados | Sí |

## 3) Recomendaciones priorizadas

| Recomendación | Prioridad objetivo |
|---|---|
| Implementar control de Mínimo Privilegio y Separación de Funciones. | Inmediato (0–30 días) |
| Desplegar cifrado para datos en reposo y en tránsito, especialmente datos de tarjeta (PCI). | Inmediato (0–30 días) |
| Implantar un gestor de contraseñas y reforzar la política (longitud, complejidad, MFA donde aplique). | 0–30 días |
| Diseñar, documentar y probar un Plan de Recuperación ante Desastres; establecer copias de seguridad regulares y pruebas de restauración. | 0–60 días |
| Implementar un IDS y, si es posible, integración SIEM para alertado centralizado. | 30–60 días |
| Formalizar calendario de mantenimiento para sistemas legacy con procedimientos de intervención. | 30–60 días |
| Completar inventario y clasificación de datos/activos; mapear flujos de datos sensibles. | 0–45 días |
| Restringir el acceso a datos de tarjeta a personal estrictamente necesario; segmentar/red de datos de tarjeta. | 0–45 días |
| Revisar y documentar políticas de acceso de usuarios (altas/bajas/cambios, revisiones periódicas). | 0–45 días |
| Formación de concienciación en privacidad y seguridad para todo el personal. | 0–60 días |

---
_Elaborado por: Auditoría interna (actividad formativa)._