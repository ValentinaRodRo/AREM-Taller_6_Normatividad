# 🧾 Notas – Parte 1: Checklist de Cumplimiento Normativo (GobData)

## 📘 Contexto del caso
**GobData** es una plataforma estatal de trámites ciudadanos en línea que gestiona información personal y datos sensibles (salud, antecedentes, identificación, direcciones, certificados digitales).  
Por la naturaleza de la información que procesa, está sujeta a la **Ley 1581 de 2012**, el **Decreto 1377 de 2013**, los lineamientos de la **Superintendencia de Industria y Comercio (SIC)**, y estándares internacionales como **ISO/IEC 27001** y el **GDPR europeo**.

El objetivo del checklist fue verificar el nivel de cumplimiento en materia de protección de datos personales, seguridad de la información y principios de privacidad por diseño.

---

## 🔍 Resumen general de cumplimiento

| Categoría | Nivel de Cumplimiento | Observación general |
|------------|------------------------|----------------------|
| Gobernanza y base legal | Parcial | Existen políticas y avisos, pero falta actualización de registros ante la SIC y cláusulas de terceros. |
| Consentimiento y principios | Parcial | Los mecanismos de consentimiento funcionan; faltan DPIA para datos sensibles. |
| Derechos del titular (Habeas Data) | Parcial | Hay acceso y actualización, pero no portabilidad ni supresión completa. |
| Seguridad de la información (ISO 27001) | Parcial | Buen control de accesos y trazabilidad, pero cifrado y continuidad necesitan mejoras. |
| Retención y eliminación | No cumple | No hay política formal de retención documental. |
| Terceros y transferencias | Parcial | Infraestructura nacional, pero contratos sin anexos de seguridad. |
| Privacidad por diseño | Parcial | Falta institucionalizar revisiones de privacidad y DPIA. |

---

## ⚠️ Hallazgos clave

1. **Política de retención inexistente**  
   No se define cuánto tiempo conservar los datos ni el método de eliminación o anonimización.  
   ➜ *Riesgo alto de incumplimiento con la Ley 1581 de 2012, Art. 11.*

2. **Evaluaciones de impacto (DPIA) no implementadas**  
   Los módulos que manejan datos sensibles (salud, antecedentes) no han sido evaluados formalmente.  
   ➜ *Recomendado por el GDPR Art. 35 y la Guía SIC sobre tratamiento de datos sensibles.*

3. **Cifrado incompleto en reposo**  
   Aunque se usa TLS 1.2+ en tránsito, el cifrado en bases de datos no es uniforme y carece de administración central de llaves (KMS).  
   ➜ *Relevante para ISO 27001 A.10 y GDPR Art. 32.*

4. **Contratos con terceros sin cláusulas de seguridad**  
   Se hallaron convenios sin definiciones claras de responsabilidades ni auditorías a subencargados.  
   ➜ *Ley 1581 Art. 25 y ISO 27001 A.15.*

5. **Derechos del titular parcialmente implementados**  
   El portal permite consultar y actualizar datos, pero no suprimirlos ni exportarlos.  
   ➜ *GDPR Art. 15–20; Ley 1581 Art. 8–15.*

---

## 🧭 Recomendaciones prioritarias (primeros 90 días)

1. **Definir y aprobar política de retención** con tablas de conservación por tipo de trámite.  
2. **Implementar cifrado en reposo** con gestión central de llaves (KMS) y rotación periódica.  
3. **Realizar DPIA** en los módulos de salud y antecedentes judiciales.  
4. **Actualizar contratos** con terceros incluyendo cláusulas de confidencialidad, subprocesadores y auditoría.  
5. **Crear procedimiento ARCO completo** (Acceso, Rectificación, Cancelación, Oposición) para el ciudadano.  
6. **Incluir checklist de privacidad por defecto** en el ciclo de desarrollo (SDLC).

---

## 🧩 Conclusión
El caso **GobData** presenta un cumplimiento **moderado (≈ 60 %)** en materia de protección de datos y seguridad.  
Se destacan avances en autenticación, trazabilidad y avisos de privacidad, pero aún existen brechas relevantes en **retención**, **evaluación de impacto** y **gestión de cifrado**.

El fortalecimiento de la gobernanza y la adopción de un **SGSI conforme a ISO/IEC 27001** permitirán mejorar la confianza ciudadana y el cumplimiento normativo a nivel nacional e internacional.

---

### 📚 Referencias legales y normativas
- **Ley 1581 de 2012** – Protección de Datos Personales (Colombia)  
- **Decreto 1377 de 2013** – Reglamenta parcialmente la Ley 1581  
- **Guía SIC** – Tratamiento de datos sensibles  
- **ISO/IEC 27001:2022** – Sistema de gestión de seguridad de la información  
- **GDPR UE 2016/679** – Reglamento General de Protección de Datos  
- **Circular MinTIC 01 de 2021** – Lineamientos de seguridad digital
