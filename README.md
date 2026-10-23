# LUMA POS - Sistema de Punto de Venta y Gestión Comercial Inteligente

Proyecto integrador correspondiente a la cátedra de **Práctica Profesionalizante 1 (PP1)** de la carrera **Técnico Superior en Desarrollo de Software** del **Instituto Superior Santo Domingo (ISSD)**.

## 📌 Descripción del Proyecto
LUMA POS es una solución integral diseñada para micro y pequeños comercios minoristas multirrubro (almacén, fiambrería, carnicería y minimarket). El sistema busca optimizar el cobro en mostrador mediante la integración de balanzas comerciales, mitigar mermas por vencimiento aplicando rotación FIFO y descuentos automáticos (Smart Sale), agilizar la actualización masiva de precios y centralizar la conciliación de caja y cuentas corrientes (fiados).

---

## 🛠️ Stack Tecnológico (Sprint 0)
* **Lenguaje:** Python 3.10+ (versión configurada: 3.13.2)
* **Framework Web:** Django 5+ (versión configurada: 6.1.2)
* **Frontend:** HTML5, Tailwind CSS, Alpine.js, HTMX
* **Base de Datos:** SQLite (desarrollo) / PostgreSQL (producción)
* **Control de Versiones:** Git & GitHub
* **IDE / Entorno:** PyCharm

---

## 🚀 Instalación y Puesta en Marcha

### 1. Clonar el repositorio
```bash
git clone https://github.com/Ludmimar/LumaPos.git
cd LumaPos
```

### 2. Crear y activar el entorno virtual
* **En Windows (Git Bash):**
  ```bash
  python -m venv .venv
  source .venv/Scripts/activate
  ```
* **En Windows (PowerShell):**
  ```powershell
  python -m venv .venv
  .venv\Scripts\Activate.ps1
  ```
* **En Linux / macOS:**
  ```bash
  python3 -m venv .venv
  source .venv/bin/activate
  ```

### 3. Instalar dependencias
```bash
pip install -r requirements.txt
```
*(o `pip install django` si estás configurando el entorno base inicial).*

### 4. Aplicar migraciones iniciales
```bash
python manage.py migrate
```

### 5. Iniciar el servidor de desarrollo
```bash
python manage.py runserver
```
El sistema quedará disponible en el navegador web en `http://127.0.0.1:8000/`.

---

## 📂 Estructura de Carpetas Propuesta
* `config/`: Configuración principal de Django (`settings.py`, `urls.py`, `wsgi.py`).
* `core/`: Componentes, vistas base y layouts compartidos.
* `ventas/`: Módulo de facturación, punto de venta (POS) y pesaje en balanza.
* `inventario/`: Control de existencias, lotes FIFO y alertas de caducidad.
* `caja/`: Apertura, arqueos, retiros y cierres de sesión (Reporte Z).
* `clientes/`: Gestión de cuentas corrientes y saldos deudores (fiados).
* `proveedores/`: Compras, remitos y pagos de mercadería.
* `tests/`: Pruebas automatizadas.

---

## 👤 Datos de la Estudiante
* **Estudiante:** Ludmila Anahi Martos
* **Docente:** Nadia Soledad Gallardo
* **Semestre:** 4to — **Año:** 2026