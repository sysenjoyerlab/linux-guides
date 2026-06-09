# Guía de Elección: ¿Qué distribución de Linux elegir?

Para saber qué distribución queremos debemos saber para qué la queremos. Puedes encontrar más información de cada distribución en su respectiva carpeta dentro de este repositorio.

## Conceptos clave
Antes de elegir, es fundamental entender que no todas las distribuciones operan bajo los mismos principios. Estas seis dicotomías definen la experiencia del usuario:

*   **Ciclo de actualización:** 
    *   *Rolling Release:* Actualizaciones continuas, sin versiones mayores. Software siempre moderno, pero requiere mayor atención al actualizar.
    *   *Fixed Release:* Versiones cerradas (ej. Debian 12). Máxima estabilidad y predictibilidad; software más conservador.
*   **Sistema de inicio (Init):**
    *   *Con Systemd:* El estándar actual. Automatizado y centralizado. Ideal para facilidad y compatibilidad universal.
    *   *Sin Systemd:* Opciones como OpenRC o runit. Para quienes buscan simplicidad UNIX y transparencia.
*   **Gestión de paquetes:**
    *   *Binarios:* Descargas programas ya compilados (rápido y sencillo).
    *   *Fuentes:* Compilas el software en tu máquina (adaptación total, requiere más tiempo).
    *   *Universales:* (Flatpak/Snap) Aislados del sistema para evitar problemas de dependencias.
*   **Idealismo del software (Ética):**
    *   *Puristas:* Solo software 100% libre.
    *   *Pragmáticas:* Incluyen drivers propietarios para asegurar que el hardware funcione a la primera.
*   **Estructura de Administración:**
    *   *"Opinionated" (Opinadas):* Los desarrolladores deciden por ti para darte una experiencia consistente.
    *   *"DIY" (Do It Yourself):* Tú eres el arquitecto; construyes el sistema desde los cimientos.
*   **Ciclo de Estabilidad:**
    *   *Estabilidad de "Roca":* Prioriza que el sistema no cambie (ideal para servidores).
    *   *Estabilidad de "Vanguardia":* Prioriza tener los últimos parches y mejoras (ideal para desarrollo).

---

## 1. Para principiantes (Facilidad de uso)
Estas distribuciones son el mejor punto de partida para ir tomando contacto con la terminal. Priorizamos la estabilidad, facilidad de uso y un entorno gráfico pulido.

*   **Ubuntu:** Extremadamente sencillo, su interfaz gráfica es muy completa y apenas requiere usar la terminal.
*   **Pop!OS:** Excelente compatibilidad con tarjetas gráficas Nvidia e incluye Tiling Window Manager (gestor de ventanas tipo mosaico.
*   **Linux Mint:** Probablemente la opción más natural para quienes vienen de Windows. Ofrece un entorno de escritorio (Cinnamon) muy pulido e intuitivo.

## 2. Usuarios avanzados o con ganas de aprender
Cuando buscas sacar el máximo partido a tu sistema y entender cómo funciona:

*   **Arch Linux:** Muy recomendada con fines educativos. Al ser *Rolling Release*, requiere estar atento a la *ArchWiki* y realizar buenas prácticas (backups). Su documentación es, sencillamente, la mejor del ecosistema.
*   **Gentoo Linux:** Su ventaja son las `useflags`, que permiten definir qué funciones incluir al compilar el software. Construyes un sistema adaptado a tu hardware.
*   **Slackware:** Basada en los principios de UNIX tradicional, prescinde de automatismos modernos y gestión automática de dependencias. La elección perfecta si buscas aprender Linux sin capas de abstracción y evitar *systemd*.

## 3. Ciberseguridad
Puedes instalar un SO ya preparado o modificar uno base. Yo recomiendo modificar uno base para reducir la **superficie de ataque**.

*   **Kali Linux (Debian-based):** El estándar de la industria; la mayoría de cursos y guías están enfocados en esta distribución.
*   **BlackArch (Arch-based):** Cuenta con un repositorio enorme (AUR) de herramientas, con las ventajas de ser *rolling release* y tener acceso a la *ArchWiki* (aunque esta Wiki es ampliamente utilizada para otros sistemas operativos no Arch).
*   **Parrot:** Destaca por su versatilidad. Pensado tanto para auditorías de seguridad como para uso diario y desarrollo.

## 4. Seguridad y Privacidad
Distribuciones enfocadas radicalmente en el anonimato y la protección.

*   **Qubes:** Utiliza un hipervisor (Xen) para aislar cada tarea (navegación, correo, trabajo) en máquinas virtuales llamadas "qubes". Si una parte es comprometida, el resto permanece intacto.
*   **Tails:** Diseñado para iniciarse desde un USB. Todo el tráfico pasa por Tor y, al apagarse, borra todo rastro en la RAM.
*   **Whonix:** Utiliza dos máquinas virtuales: una actúa como puerta de enlace (gateway) hacia Tor y la otra como estación de trabajo, evitando fugas de identidad.

## 5. Servidores
Aquí buscamos estabilidad, seguridad y mantenimiento predecible.

*   **Debian:** El estándar de facto. Configuración lógica, comunidad enorme y la base de muchos otros sistemas.
*   **OpenBSD:** Técnicamente no es Linux (es UNIX), pero es obligatorio nombrarlo. Enfoque radical en la seguridad y código auditable. El sistema con menos fallos remotos de la historia.

---
> *Recuerda: no hay una “mejor” distribución, solo hay herramientas que se ajustan mejor o peor a tus necesidades actuales.*

**¿Qué sigue?** Puedes consultar las guías de instalación o los apartados de “Entornos de escritorio y Window Managers”.
