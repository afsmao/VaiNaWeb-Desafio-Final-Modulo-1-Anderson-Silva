# Proposta Técnica para Cliente: Arquitetura de Rede Corporativa com Foco em Segurança e Segmentação

## 1. Sumário Executivo
Esta proposta técnica visa atender à solicitação de um cliente fictício para o projeto de uma nova rede corporativa, com foco em segurança e segmentação. O objetivo é fornecer uma solução robusta que garanta a proteção dos ativos da empresa, ao mesmo tempo que assegura a eficiência e a escalabilidade da rede. A proposta detalha o escopo, metodologia, justificativas técnicas, e o plano de ação inicial para implementação.

## 2. Objetivo
Projetar uma rede corporativa segura e segmentada, capaz de atender às necessidades do cliente fictício em termos de usuários, setores e escritórios, promovendo maior controle e proteção dos ativos, além de facilitar a gestão de tráfego e recursos.

## 3. Escopo
- **Número de usuários**: 500.
- **Setores**: Recursos Humanos, Financeiro, TI, Marketing e Vendas.
- **Escritórios**: Matriz e três filiais.
- **Infraestrutura**: Servidores corporativos, estações de trabalho, dispositivos móveis e IoT.
- **Segurança**: Implementação de segmentação de rede, firewall, VPN e sistemas de monitoramento de tráfego.

## 4. Metodologia
A metodologia segue os seguintes passos:
1. Levantamento de requisitos junto ao cliente.
2. Planejamento de arquitetura lógica da rede.
3. Prototipagem em ambiente de simulação (Docker).
4. Documentação técnica detalhada.
5. Validação junto ao cliente.
6. Implementação em etapas com monitoramento contínuo.

## 5. Diagrama Lógico com Segmentação
O diagrama lógico da rede é estruturado em cinco segmentos principais:
- **Segmento 1**: Servidores corporativos (DNS, DHCP, Banco de Dados e Aplicações).
- **Segmento 2**: Estações de trabalho de usuários.
- **Segmento 3**: Dispositivos móveis e IoT.
- **Segmento 4**: Escritórios remotos conectados via VPN.
- **Segmento 5**: Área de DMZ para serviços externos (web e e-mail).

**Referência:** Veja o diagrama lógico detalhado no arquivo `diagrama_logico.md`.

## 6. Diagnóstico
### Principais Vulnerabilidades Identificadas:
1. Falta de segmentação entre setores, permitindo tráfego desnecessário e aumentando riscos de propagação de ameaças.
2. Ausência de monitoramento de tráfego em tempo real.
3. Dispositivos IoT sem proteção adequada.
4. VPN não implementada para escritórios remotos.

## 7. Recomendações
### Segmentação de Rede:
- Utilizar VLANs para separar tráfego entre setores e filiais.
- Configurar regras de firewall para controlar acesso entre segmentos.

### Proteção de Perímetro:
- Implementar firewalls de próxima geração.
- Configurar VPN para conexão segura entre matriz e filiais.

### Monitoramento:
- Adotar ferramentas de monitoramento de tráfego como Wireshark e sistemas SIEM.

### Proteção de IoT:
- Isolar dispositivos IoT em uma VLAN específica e aplicar políticas de segurança rigorosas.

## 8. Plano de Ação (Modelo 80/20)
### Fase 1: Implementação Inicial (80%)
- Configuração de VLANs e regras de firewall.
- Implementação de VPN para escritórios remotos.
- Prototipagem em ambiente Docker para validação de arquitetura.

### Fase 2: Melhorias Adicionais (20%)
- Configuração de sistemas de monitoramento (SIEM).
- Treinamento de equipe para gestão da nova infraestrutura.
- Revisão e ajustes conforme feedback do cliente.

## 9. Conclusão
Com esta proposta técnica, o cliente terá uma rede corporativa moderna, segura e segmentada, capaz de suportar o crescimento da empresa e garantir a proteção de seus ativos. A implementação será realizada em fases, com validação contínua para assegurar que os objetivos sejam plenamente atingidos.

## 10. Anexos
- [Diagrama lógico da rede](diagrama_logico.md)
- [Exemplo de regras de firewall](regras_firewall.md)

---

**Prazo de entrega**: 28 de julho de 2025, 23:59.
