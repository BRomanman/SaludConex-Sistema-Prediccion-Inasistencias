# Dataset sintético original

Archivo: `SaludConex_Datos_Sinteticos_50000.csv`

## Resumen

- Registros: 50.000.
- Variables: 18.
- Periodo de `Fecha_Atencion`: 2024-01-01 a 2026-10-31.
- Valores vacíos detectados en la revisión: 0.
- IDs de reserva únicos: 50.000.
- Edades registradas: 1 a 89 años.

## Distribución de `Resultado_Reserva`

| Valor | Registros | Porcentaje |
|---|---:|---:|
| Asistio | 38.562 | 77,12 % |
| Inasistencia | 8.450 | 16,90 % |
| Cancelada | 2.988 | 5,98 % |

Las cancelaciones se excluyen del conjunto utilizado para el modelamiento, quedando 47.012 registros.

## Diccionario de datos

| Columna | Descripción |
|---|---|
| `ID_Reserva` | Identificador sintético de la reserva. |
| `ID_Paciente_Anonimizado` | Identificador sintético anonimizado del paciente. |
| `Edad` | Edad registrada para la reserva. |
| `Comuna` | Comuna asociada al registro. |
| `Centro_Medico` | Centro médico asociado. |
| `Especialidad` | Especialidad de la consulta. |
| `Profesional_ID` | Identificador del profesional. |
| `Fecha_Solicitud` | Fecha en que se solicitó la reserva. |
| `Fecha_Atencion` | Fecha programada para la atención. |
| `Horario_Atencion` | Bloque horario de la atención. |
| `Dias_Anticipacion` | Días entre la solicitud y la atención. |
| `Asistencias_Previas` | Conteo sintético de asistencias previas. |
| `Cancelaciones_Previas` | Conteo sintético de cancelaciones previas. |
| `Inasistencias_Previas` | Conteo sintético de inasistencias previas. |
| `Tipo_Previsión` | Tipo de previsión. |
| `Modalidad_Atencion` | Modalidad de la atención. |
| `Confirmacion_Recordatorio` | Estado de confirmación del recordatorio. |
| `Resultado_Reserva` | Resultado de la reserva: asistencia, inasistencia o cancelación. |

**Uso:** dataset de entrada para el notebook. `Resultado_Reserva` es la variable objetivo/resultado y no debe utilizarse como variable predictora.
