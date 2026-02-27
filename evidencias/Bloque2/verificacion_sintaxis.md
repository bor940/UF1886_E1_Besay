# 2.2 Verificación sintáctica

Módulo: Personalización de formato de ventas  
Archivo de manifiesto detectado: manifest  
Nombre esperado por Odoo: __manifest__.py  

---

## 1) Sintaxis Python

### 1.1 Comprobación del nombre del archivo (requisito Odoo)

__Objetivo:__ verificar que el manifiesto tiene el nombre requerido por Odoo para que el módulo sea reconocido.

__Comando ejecutado:__
```bash

ls -la

drwxrwxr-x 3 bor bor 4096 Feb 25 12:39 .
drwxrwxr-x 3 bor bor 4096 Feb 25 12:21 ..
-rw-rw-r-- 1 bor bor    0 Feb 25 12:36 __init__.py
-rw-rw-r-- 1 bor bor  333 Feb 25 12:39 __manifest__.py
drwxrwxr-x 2 bor bor 4096 Feb 26 09:21 views


```

```code
contenido manifiest

{
    "license": "LGPL-3",
    "name":"Personalización de formato de ventas",
    "data":[
        "views/sale_report.xml",
    ],
    "depends":[
        "sale",
    ]
}

```

## 1) Validacion XML

__Objetivo:__ comprobar que el referenciado en el manifiesto esta bien formado

__Artributo referenciado__

-views/sale_report.xml

### 1.1 Verificar la evidencia del archivo

__Comando ejecutado__

```bash

```

__Salida obtenida__

```bash

```

### 1.2 Validacion archivo XML (bien formado)

```bash
xmllint --noout views/sale_report.xml
echo $?
```

__Salida obtenida__
```bash


```

__Resultado__
- Codigo de retorno
- Interpretacion:
    - 0 -> XML bien formado
    - Error -> Indicar mensaje exacto
