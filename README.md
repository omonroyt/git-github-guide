# 📚 Guía Personal de Git y GitHub

> Mi repositorio de estudio para repasar todo lo que he aprendido sobre **Git** y **GitHub**.

---

## 📌 Índice

1. [¿Qué es Git y GitHub?](#-qué-es-git-y-github)
2. [Configuración inicial](#-configuración-inicial)
3. [Flujo de trabajo básico con Git](#-flujo-de-trabajo-básico-con-git)
4. [Comandos básicos de Git](#-comandos-básicos-de-git)
5. [Trabajo con ramas](#-trabajo-con-ramas)
6. [Trabajo con GitHub (remotos)](#-trabajo-con-github-remotos)
7. [Comandos útiles extra](#-comandos-útiles-extra)
8. [Notas personales y ejemplos](#-notas-personales-y-ejemplos)
9. [Recursos recomendados](#-recursos-recomendados)

---

## 🧠 ¿Qué es Git y GitHub?

**Git** es un sistema de control de versiones distribuido.  
**GitHub** es una plataforma en la nube que hospeda repositorios Git y facilita colaborar.

- Git = herramienta en tu computadora.
- GitHub = lugar donde alojas/repositorios y colaboras.

---

## ⚙️ Configuración inicial

### 1️⃣ Configurar usuario y correo

```bash
git config --global user.name "Tu Nombre"
git config --global user.email "tu_correo@example.com"
```
Ver configuración:
```bash
git config --list
```
Definir rama principal como ***main*** (práctica moderna):
```bash
git config --global init.defaultBranch main
```
---
### 2️⃣ Crear una llave SSH

```bash
ssh-keygen -t ed25519
```
Ver contraseña generada:
```bash
cd ~/.ssh/id_ed25519.pub
...
```
Iniciar una conexión SSH hacia GitHub:
```bash
ssh -T git@github.com

...(write:) yes
```
`Hi user! You've successfully authenticated, but Github...`
### 3️⃣ Crear una nueva llave SSH en GitHub.
![NewSSHKEY](./images/newsshkey.png)
