---
title: "Qtheme"
date: "2025-09-25"
tags:
  - "python"
  - "qtile"
  - "archlinux"
  - "cli"
---

![preview](https://raw.githubusercontent.com/jsusmachaca/qtheme/master/preview/term.png)
![preview](https://raw.githubusercontent.com/jsusmachaca/qtheme/master/preview/bars.png)

**Qtheme** es una herramienta de línea de comandos (CLI) desarrollada en Python que facilita la gestión y personalización de temas en **Qtile** (gestor de ventanas) y **Kitty** (emulador de terminal).

---

# Instalación

```sh
git clone https://github.com/jsusmachaca/qtheme.git
cd qtheme
```

En Arch Linux:

```sh
makepkg -si
```

En otras distribuciones:

```sh
python setup.py build
python setup.py install
```

---

# Aplicación

## Qtile

Para listar los temas disponibles para Qtile y Kitty:

```sh
qtheme -ls
```

Salida:

![preview](https://raw.githubusercontent.com/jsusmachaca/qtheme/master/preview/list.png)

Para cambiar el tema de Qtile:

```sh
qtheme --theme [tema]
```

Para cambiar la posición de la barra:

```sh
qtheme --position [top/bottom]
```

Puedes combinar los parámetros:

```sh
qtheme -t nord -p t
```

---

## Kitty

Para cambiar el tema del terminal:

```sh
qtheme --terminal [tema]
```

Para cambiar la opacidad del terminal:

```sh
qtheme --terminal-opacity [valor-opacidad]
```

Para cambiar la fuente del terminal:

```sh
qtheme --terminal-font [familia-de-fuente]
```

---

## Qtile + Kitty

Puedes usar los parámetros juntos:

```sh
qtheme -t onedark -To 0.80 -kf "UbuntuMono Nerd Font"
```

También puedes usar parámetros para Qtile y Kitty combinados:

```sh
qtheme -t forest -p b -k onedark -ko 1 -kf "Hack Nerd Font"
```
