# 🌐 Resumo - Componentes da Arquitetura do Microsoft Azure

Este repositório contém um resumo dos principais conceitos sobre a **arquitetura do Microsoft Azure**, abordando recursos fundamentais como regiões, grupos de recursos, pares de regiões, assinaturas, entre outros. Este material serve como apoio para revisão, estudos e futuras implementações na nuvem da Microsoft.

---

## 📦 Componentes de Arquitetura do Azure

A arquitetura do Azure é composta por vários elementos que juntos garantem **escalabilidade**, **disponibilidade**, **resiliência** e **gestão eficiente** de recursos em nuvem. Os principais componentes são:

- **Regiões**: Conjuntos de datacenters geograficamente localizados que oferecem serviços do Azure.
- **Zonas de disponibilidade**: Isolamentos físicos dentro de uma região para garantir alta disponibilidade.
- **Conjuntos de disponibilidade (Availability Sets)**: Distribuem VMs entre domínios de falha e de atualização para evitar indisponibilidade.
- **Grupos de recursos**: Containers lógicos que agrupam recursos relacionados, como VMs, redes e bancos de dados.

---

## 🌍 Pares de Região e Grupos de Recursos

- **Pares de regiões** são duas regiões vinculadas com o objetivo de replicação e recuperação de desastres. Essa relação garante:
  - Replicação assíncrona confiável
  - Prioridade em atualizações para evitar falhas simultâneas
  - Armazenamento georredundante seguro

- **Grupos de recursos**:
  - Servem para agrupar recursos que compartilham o mesmo ciclo de vida.
  - **Importante**: grupos de recursos **podem conter recursos localizados em diferentes regiões**.

---

## 🧾 Assinaturas do Azure e Grupos de Gerenciamento

- **Assinatura (Subscription)**: Unidade de cobrança que organiza e controla o uso dos recursos do Azure.
- **Grupos de gerenciamento (Management Groups)**: Utilizados para organizar múltiplas assinaturas e aplicar políticas de governança (RBAC, políticas de segurança, etc.).

---

## 🔁 Alta Disponibilidade e Replicação

- A **alta disponibilidade** é garantida por meio de:
  - Zonas e conjuntos de disponibilidade
  - Balanceamento de carga
  - Replicação entre regiões

- A **replicação de baixa latência** permite que aplicativos críticos tenham desempenho confiável e tolerância a falhas.

---

## 🗺️ Região do Azure

- Uma **região** é um conjunto de datacenters implantados dentro de uma área geográfica específica.
- Cada região é conectada por redes de **baixa latência e alta capacidade**.

---

## ⚙️ Conjuntos de Disponibilidade

- São compostos por:
  - **Domínios de falha**: isolam VMs entre racks físicos diferentes.
  - **Domínios de atualização**: garantem que atualizações de sistema ocorram de forma escalonada, evitando indisponibilidade simultânea.

---

📝 **Observação**: Este conteúdo é parte do desafio prático de arquitetura de nuvem Microsoft Azure, proposto na plataforma DIO.

