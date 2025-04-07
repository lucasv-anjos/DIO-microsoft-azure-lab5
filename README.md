# 🖥️ Considerações Importantes ao Criar uma VM no Microsoft Azure

Criar uma máquina virtual (VM) no Azure envolve diversas decisões que impactam desempenho, custo, segurança e escalabilidade. Abaixo estão as principais considerações:

---

## 📍 1. Escolha da Região

- Selecione uma **região próxima aos usuários finais** para reduzir a latência.
- Verifique a **disponibilidade de recursos e serviços** na região desejada.
- Considere a **compliance local** (ex: exigências de armazenamento de dados no país).

---

## 📐 2. Tamanho da VM

- Escolha o tipo de VM com base na carga de trabalho.
- Avalie:
  - Número de vCPUs
  - Quantidade de memória RAM
  - Capacidade de armazenamento temporário

---

## 💾 3. Tipo de Disco e Armazenamento

- **Disco do SO**: SSD padrão ou premium.
- **Discos de dados** adicionais, se necessário.
- **Armazenamento gerenciado**: oferece alta disponibilidade e facilidade de gerenciamento.
- **Snapshots** e **backups** são recomendados para recuperação.

---

## 🔐 4. Sistema Operacional e Imagem

- Escolha entre entre as opções de imagens disponiveis.
- Pode-se usar imagens personalizadas para a criação da VM.

---

## 🌐 5. Rede e Segurança

- **Criação de VNet (rede virtual)** para isolar e controlar o tráfego.
- Configuração de **sub-redes**, **endereçamento IP**, e **grupos de segurança de rede (NSG)**.
- Considere:
  - Firewalls
  - VPNs
  - Regras de entrada/saída

---

## 🛡️ 6. Gerenciamento de Identidade e Acesso

- Use **Azure Active Directory** para autenticação e controle de acesso.
- Implemente **Managed Identities** para evitar armazenar credenciais no código.
- Atribua **RBAC (controle de acesso baseado em função)** para limitar permissões.

---

## 💸 7. Custos e Orçamento

- Analise o custo estimado antes da criação.
- Considere:
  - Tempo de execução (ligado vs desligado)
  - Tipo de disco
  - Tráfego de rede
  - Use a [**Calculadora de Preços do Azure**](https://azure.microsoft.com/pt-br/pricing/calculator/) para simulações:  

---

## 🔄 8. Alta Disponibilidade e Backup

- Use **Availability Sets** ou **Availability Zones** para redundância.
- Configure **backup automático** com Azure Backup.
- Habilite **monitoramento com Azure Monitor e Log Analytics**.

---

## ✅ 9. Tags e Organização

- Use **tags** para organizar, monitorar custos e aplicar políticas de governança.
- Exemplo: `Environment=Production`, `Owner=EquipeTI`

---
