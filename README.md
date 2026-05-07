# ⚔️ Mu Online Classic - Server Infrastructure

Infraestructura moderna para un servidor de **Mu Online Season Classic**, basada en el emulador nativo **OpenMU** y desplegada mediante **Docker & Easypanel**.

## 🚀 Despliegue Rápido (Easypanel)

1. Conecta este repositorio a tu proyecto en **Easypanel**.
2. Asegúrate de tener una instancia de **PostgreSQL 17** corriendo.
3. Configura las variables de entorno detalladas en `.env.example`.

## 📂 Estructura del Proyecto

```text
├── configs/            # Configuraciones del juego (Exp, Drop, Shops)
├── data/               # Volúmenes persistentes de la base de datos
├── .github/workflows/  # Automatización de despliegue
├── docker-compose.yml  # Definición de servicios (Stack)
└── .env.example        # Plantilla de variables de entorno
```

## 🛠️ Comandos de Administración

### Ver logs del servidor
```bash
docker logs -f mu-server
```

### Reiniciar el servidor
```bash
docker-compose restart mu-server
```

## 🔒 Seguridad
- No olvides cambiar las contraseñas por defecto en producción.
- Los puertos expuestos son: `44405` (Connect), `55901` (Game), `1234` (Admin Panel).

---
*Powered by Antigravity AI Engine*
