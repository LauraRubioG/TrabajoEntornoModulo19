# Informe de Práctica Git - Grupo [Marta Gonzalez, Laura Rubio y Paula Rivas] Modulo 19

## 1. Integrantes y Reparto de Tareas

* **[Laura Rubio]:**
    * Configuración inicial del repositorio local y remoto.
    * Creación de la rama `feature/laura-rubio`.
    * Modificación del archivo `index.html`. (generación de conflicto intencionado).
    * Resolución del conflicto mediante merge manual.
    * Integración de cambios en `main` (Fast-forward).
    * Mejora del historial de commits usando `git commit --amend`.
    * Uso del comando `git stash` para guardar cambios temporales.
    * Resolución final de conflictos al integrar en `main`.
    * Documentación del proyecto (`GIT_LOG.md`).
    

* **[Marta González]:**
    * Creación de la rama `feature/marta-gonzalez`.
    * Modificación del archivo `index.html` (generación de conflicto intencionado).
    * Resolución del conflicto mediante merge manual.
    * Integración de cambios en `main` (Fast-forward).
    * Mejora del historial de commits usando `git commit --amend`.
    * Uso del comando `git stash` para guardar cambios temporales.
    * Resolución final de conflictos al integrar en `main`.
    * Documentación del proyecto (`GIT_LOG.md`).

* **[Paula Rivas]:**
    * Creación de la rama `feature/paula rivas`.
    * Modificación del archivo `index.html`. (generación de conflicto intencionado).
    * Resolución del conflicto mediante merge manual.
    * Integración de cambios en `main` (Fast-forward).
    * Mejora del historial de commits usando `git commit --amend`.
    * Uso del comando `git stash` para guardar cambios temporales.
    * Resolución final de conflictos al integrar en `main`.
    * Documentación del proyecto (`GIT_LOG.md`).

---

## 2. Descripción de los Conflictos

Durante la práctica se generaron conflictos intencionados para practicar su resolución:

### Conflicto 1: Edición simultánea de HTML
* **Archivos afectados:** `index.html`
* **Causa:** Las integrantes Laura, Marta y Paula intentaron fusionar su rama con `main`, pero Marta ya había modificado las líneas en el parrafo `<p>`.
* **Resolución:** Paula y Laura realizacon un `git pull` para traer los cambios remotos. VS Code detectó el conflicto. Una edito las líneas eliminando las marcas `<<<< HEAD` y `>>>>`, y otra uso los camando merge, add y push  para resolver el conflicto, decidiendo mantener ambos cambios en el archivo

### Conflicto 2: Edición simultánea de HTML
* **Archivos afectados:** `index.html`
* **Causa:** Las integrantes Laura, Marta y Paula volvieron a fusionar su rama con `main`, pero Paula ya había modificado las líneas en el parrafo `<p>`.
* **Resolución:** Marta y Laura realizacon un `git pull` para traer los cambios remotos. VS Code detectó el conflicto. En este caso ambas usaron los camando merge, add y push  para resolver el conflicto, decidiendo mantener ambos cambios en el archivo


---

## 3. Comandos Git Relevantes

Lista de los comandos más utilizados durante el flujo de trabajo:

* **Gestión de ramas:**
    * `git checkout -b feature/nombre`: Para crear y cambiar a una nueva rama.
    * `git checkout main`: Para volver a la rama principal.

* **Sincronización:**
    * `git push origin feature/nombre`: Para subir la rama personal a GitHub.
    * `git pull origin main`: Fundamental para actualizar el repositorio local antes de fusionar.

* **Integración y Conflictos:**
    * `git merge feature/nombre`: Para integrar los cambios de una rama.
    * `git status`: Usado constantemente para verificar archivos modificados o en conflicto.

* **Avanzados:**
    * `git commit --amend`: Utilizado para corregir el mensaje del último commit y mejorar el historial.
    * `git stash`: Utilizado para guardar cambios en progreso sin hacer commit.