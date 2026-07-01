# 📊 Resumen Ejecutivo

## 🔴 Amenaza: Campaña de Phishing y Malware en Dominios .shop

**Fecha:** 2026-07-01  
**Autor:** Condor2026  
**Clasificación:** CRÍTICA  
**TLP:** CLEAR

---

### 🎯 ¿Qué hemos encontrado?

Hemos identificado una **red criminal activa** que utiliza:
- 1 IP maliciosa: `104.17.231.54` (Cloudflare)
- 100+ dominios `.shop` con nombres aleatorios
- Certificados SSL rotados para evadir detecciones
- Páginas de phishing que imitan a bancos y servicios

---

### 🚨 ¿Qué riesgo supone?

| Riesgo | Impacto |
|--------|---------|
| 🔴 **Robo de credenciales bancarias** | Vaciamiento de cuentas |
| 🔴 **Secuestro de sesiones** | Acceso no autorizado a cuentas |
| 🔴 **Instalación de malware** | RATs, info-stealers, troyanos |
| 🟡 **Phishing a gran escala** | Correos masivos con enlaces maliciosos |
| 🟡 **Ataques a gamers** | Distribución a través de Discord/Steam |

---

### 👤 ¿A quién afecta?

- **Usuarios de banca online** (principal objetivo)
- **Usuarios de Discord/Steam** (gamers)
- **Empleados** que reciben correos de phishing
- **Empresas** que utilizan servicios de Cloudflare (pueden tener falsos positivos)

---

### 🛡️ ¿Qué debemos hacer?

#### Acción Inmediata (AHORA MISMO)
- ✅ Bloquear `104.17.231.54` en el firewall
- ✅ Bloquear todos los dominios `.shop` listados
- ✅ Alertar a los usuarios sobre correos sospechosos
- ✅ Activar 2FA en todas las cuentas

#### Acción Preventiva (PRÓXIMOS DÍAS)
- 📌 Implementar reglas YARA/Suricata
- 📌 Monitorear logs de DNS en busca de estos dominios
- 📌 Actualizar sistemas y navegadores
- 📌 Realizar campañas de concienciación

#### Acción Estratégica (LARGO PLAZO)
- 🏛️ Reportar a las autoridades (INCIBE, Europol)
- 🏛️ Colaborar con otros investigadores
- 🏛️ Compartir IOCs con la comunidad

---

### 📈 Estadísticas Clave

| Métrica | Dato |
|---------|------|
| **Dominios maliciosos confirmados** | 25+ |
| **Dominios sospechosos** | 100+ |
| **Certificados SSL rotados** | 33+ |
| **Ventana de actividad** | 27-30 de junio de 2026 |
| **Vendors que detectan** | 12/91 (máximo) |

---

### ⚠️ Conclusión

Esta campaña es **alta y activa**. Los atacantes utilizan técnicas avanzadas de evasión (Fast-Flux DNS, DGA, rotación de certificados) y se enfocan en el robo de credenciales bancarias y sesiones. **La amenaza es real y requiere acción inmediata.**

---

### 🔗 Recursos

- 📂 Repositorio: [https://github.com/Condor2026/threat-intel-tprbalxs](https://github.com/Condor2026/threat-intel-tprbalxs)
- 📄 Informe completo: [README.md](https://github.com/Condor2026/threat-intel-tprbalxs/blob/main/README.md)
- 🔍 IOCs: [https://github.com/Condor2026/threat-intel-tprbalxs/tree/main/iocs](https://github.com/Condor2026/threat-intel-tprbalxs/tree/main/iocs)

---

**⚠️ NO ACCEDER A LOS DOMINIOS LISTADOS SIN MEDIDAS DE SEGURIDAD**

---

**Condor2026**  
*Investigador de Seguridad Independiente*  
*2026-07-01*
