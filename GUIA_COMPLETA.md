# 🎯 Registro de Asistencias - GUÍA COMPLETA

## 🚨 PROBLEMA ACTUAL: "Failed to fetch" en Vercel
**Tu proyecto:** https://ministerio-de-educaci-n.vercel.app/

## ⚡ SOLUCIÓN INMEDIATA (2 minutos):

### 1️⃣ CONFIGURAR CORS EN SUPABASE:
```
🔗 Ve a: https://supabase.com/dashboard/project/pjcokjzxzgefpdmbkuop/settings/api
📋 En "CORS Configuration", agrega:

https://ministerio-de-educaci-n.vercel.app
https://*.vercel.app
https://carlos-manuel-ponce.github.io
```

### 2️⃣ PROBAR:
- Ve a: https://ministerio-de-educaci-n.vercel.app/acreditacion.html
- Busca un DNI
- Abre Developer Tools (F12) para ver errores

## 📊 Base de Datos Implementada:
```sql
CREATE TABLE asistencia (
    region, establecimiento, cargo, aspirante,
    dni UNIQUE, asiento UNIQUE (1-209),
    presente BOOLEAN, fecha_asistencia
);
```

## 🎯 Funcionalidad:
- ✅ Búsqueda por DNI
- ✅ Muestra: región → establecimiento → cargo → aspirante → dni → asiento
- ✅ Modal de confirmación
- ✅ Registro de asistencia

## 🌐 URLs:
- **Vercel:** https://ministerio-de-educaci-n.vercel.app/acreditacion.html
- **GitHub:** https://carlos-manuel-ponce.github.io/Ministerio-de-Educaci-n/acreditacion.html
