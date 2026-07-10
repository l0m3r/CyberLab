# 🧪 CyberLab by l0m3r

## 1. 📋 О проекте
*Краткое описание целей лаборатории.*
- 🎯 **Цель:** повышение компетенций в сфере кибербезопасности, Red и Blue Team, CTF.
- 📌 **Статус:** в разработке.

---

## 2. 🏗️ Архитектура и сеть

### 2.1. 🌐 Сетевая схема (Network Diagram)
*Визуальное представление (можно вставить картинку или описать текстом).*
<img width="1940" height="1200" alt="CyberLab" src="https://github.com/user-attachments/assets/0bb9b076-a21a-4f5a-a72a-36ca4c772d2a" />

- 🔥 **DMZ-зона:** (IP диапазон) — Веб-серверы, прокси.
- 🏢 **Внутренняя сеть (Corporate):** (IP диапазон) — Рабочие станции, файловые сервера, AD.
- 🛡️ **Сеть управления (Management):** (IP диапазон) — Для доступа администраторов (через Jump Box).
- ⚔️ **Сеть атакующих (Attackers):** (IP диапазон) — Kali Linux, C2-сервера.

### 2.2. 🔗 Логическая схема взаимодействия
*Как сервисы общаются друг с другом.*
- 🎯 Цепочка атаки (Kill Chain) для конкретного сценария (например: Внешний вход -> Фишинг -> Повышение привилегий -> Exfil).
- 🧭 Схема маршрутизации (NAT, Port Forwarding).

### 2.3. 🪤 Список уязвимых сервисов (Intentional Vulnerabilities)
*Что специально настроено для взлома.*
- 💻 **SMB** — EternalBlue (MS17-010) на Win 7.
- 🌍 **Web** — SQLi / XSS на порту 8080.
- 🏛️ **AD** — Отсутствие патча ZeroLogon.

---

## 3. 🖥️ Характеристики сервера (Server Specifications)
*На каком железе/виртуализации всё работает.*

- **Хост-машина:**
  - 🐧 **OS:** Ubuntu Server 22.04 LTS / ESXi 7.0 / Proxmox.
  - ⚡ **CPU:** Intel Xeon Gold 6240 (x ядер выделено).
  - 🧠 **RAM:** 128 GB (Выделено под лабораторию: 64 GB).
  - 💾 **Storage:** NVMe SSD 2 TB (RAID 1).
  - 🌐 **Сеть:** 1 Gbps Ethernet (или 10 Gbps).

- **Виртуализация:**
  - 🧩 **Hypervisor:** VMware ESXi / KVM (Libvirt) / VirtualBox (Headless).
  - 🔌 **Тип сети:** Мост (Bridge) или Изолированная VLAN.

---

## 4. 🧰 Используемое ПО (Software Stack)
*Что установлено на хосте и внутри виртуальных машин.*

- **На хосте (Оркестрация):**
  - 🤖 Ansible / Terraform — для разворачивания ВМ.
  - 🐳 Docker / Podman — для контейнеризированных сервисов (SIEM, ELK).
  - 🔍 OpenVAS / Nessus — сканеры уязвимостей (установленные статично).
- **Внутри целевых машин (Targets):**
  - 🪟 **ОС:** Windows 10 / Server 2019, Ubuntu 20.04, Kali Linux.
  - 🧨 **Уязвимые приложения:** Apache Struts 2, Tomcat, Wordpress 4.x.
- **Инструменты мониторинга:**
  - 📊 Wazuh (EDR) / Splunk / Grafana (для визуализации логов атак).

---

## 5. 🚀 Инструкция по быстрому запуску (Quick Start / Deployment)

### 5.1. 📦 Требования (Prerequisites)
- Установленный Vagrant / VMware Workstation.
- Доступ к репозиторию (SSH ключи).

### 5.2. ⚡ Запуск окружения
```bash
git clone https://github.com/yourlab/cyberlab.git
cd cyberlab
vagrant up --provision# CyberLab 
Описание лаборатории и основых настроек. Используется для повышения компетенций в сфере кибербезопасности.

## :microscope: Описание лаборатории

Лаборатория создна на основе:
- **CPU:** 10 x Intel(R) Xeon(R) CPU E5-2666 v3 @ 2.90GHz (1 Socket)
- **RAM:** 32 GB
- **SSD:** 128 GB
- **SSD:** 500 GB
- **HDD:** 500 GB

В качестве гипервизора используется [proxmox_ve_9.2](https://www.proxmox.com/).

## :pencil: Логическая схема



