# Regras de Firewall

## Configuração de Regras para Segmentação de Rede
### Regras Básicas:
1. **Segmento 1 (Servidores)**:
   - Permitir acesso interno apenas a partir do Segmento 2 (Estações de Trabalho).
   - Bloquear acesso direto de dispositivos IoT.

2. **Segmento 2 (Estações de Trabalho)**:
   - Permitir comunicação com Segmento 1 (Servidores) e Segmento 5 (DMZ).
   - Bloquear tráfego não autorizado para Segmento 3 (IoT).

3. **Segmento 3 (IoT)**:
   - Isolamento total da rede principal.
   - Permitir acesso apenas ao Segmento 1 para serviços específicos.

4. **Segmento 4 (VPN)**:
   - Permitir acesso remoto à matriz e servidores corporativos.
   - Monitorar todo o tráfego via VPN.

5. **Segmento 5 (DMZ)**:
   - Permitir acesso externo controlado para serviços web e e-mail.
   - Bloquear acesso direto a outros segmentos internos.

### Ferramentas para Configuração:
- Firewall de próxima geração (exemplo: Palo Alto, Fortinet).
- Políticas de segurança refinadas com base em SIEM.

**Observação**: Ajustes poderão ser realizados conforme feedback do cliente.
