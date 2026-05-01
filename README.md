# 🔐 Calculadora CHMOD Linux

Una calculadora web moderna y estática para generar permisos Linux en formato **octal**, **simbólico** y comandos `chmod` reales.

Diseñada con una interfaz oscura, limpia y visualmente atractiva inspirada en paneles técnicos estilo terminal / glassmorphism.

---

## 🌐 Demo

> Sube este proyecto a GitHub Pages, Netlify o cualquier hosting estático.

---

## ✨ Características

✅ Conversión automática de permisos Linux
✅ Generación de permisos en formato **octal** (`755`, `644`, `4755`, etc.)
✅ Representación **simbólica** (`rwxr-xr-x`)
✅ Comando real `chmod` en letras:

```bash
chmod u=rwx,g=rx,o=rx archivo
```

✅ Comando `chmod` en octal:

```bash
chmod 755 archivo
```

✅ Soporte para bits especiales:

* `4000` → **SUID**
* `2000` → **SGID**
* `1000` → **Sticky Bit**

✅ Copiar resultados al portapapeles
✅ Responsive (móvil / tablet / escritorio)
✅ 100% HTML + CSS + JavaScript (sin frameworks)

---

## 📸 Vista previa

Interfaz dividida en:

### Panel izquierdo

* Bits especiales
* Usuario
* Grupo
* Otros

### Panel derecho

* Resultado octal
* Resultado simbólico
* Comando chmod numérico
* Comando chmod simbólico

---

## 📚 Ejemplos

| Permiso | Resultado |
| ------- | --------- |
| 755     | rwxr-xr-x |
| 644     | rw-r--r-- |
| 700     | rwx------ |
| 4755    | rwsr-xr-x |
| 1777    | rwxrwxrwt |

---

## 🔧 Bits Especiales

### 🔹 SUID (`4000`)

Permite ejecutar archivos con privilegios del propietario.

Ejemplo:

```bash
chmod 4755 archivo
```

---

### 🔹 SGID (`2000`)

Ejecuta con permisos del grupo o hereda grupo en carpetas.

Ejemplo:

```bash
chmod 2775 carpeta
```

---

### 🔹 Sticky Bit (`1000`)

Solo el propietario puede borrar archivos dentro del directorio.

Ejemplo:

```bash
chmod 1777 /tmp
```

---

## 🚀 Instalación

Solo descarga los archivos:

```bash
git clone https://github.com/D1se0/chmod-calculator.git
```

Y abre:

```bash
index.html
```

---

## 📁 Estructura

```bash
/
├── index.html
├── HackNerdFont-Regular.ttf
└── README.md
```

---

## 🛠 Tecnologías

* HTML5
* CSS3
* JavaScript Vanilla
* Font Awesome

---

## 💡 Uso ideal

Perfecto para:

* Administradores Linux
* Sysadmins
* DevOps
* Estudiantes de ciberseguridad
* Usuarios que aprenden chmod

---

## 🌍 Publicar en GitHub Pages

1. Sube el proyecto a GitHub
2. Ve a **Settings**
3. Entra en **Pages**
4. Branch: `main`
5. Root: `/`

Tu web quedará online.

---

## 📜 Licencia

MIT License

---

## 👨‍💻 Autor

Creado para facilitar el uso de permisos Linux de forma visual y rápida.
