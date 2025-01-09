# Anotações para o AZ-900

---

## Vantagens da Computação em Nuvem
- Alta disponibilidade  
- Escalabilidade  
- Agilidade  
- Distribuição geográfica  
- Recuperação de desastres (Disaster Recovery)  

## Por que a computação em nuvem é mais barata?
- **Baixo custo de operação**  
- **Pay as you go**: Pague pelo que usar, ajustando custos ao consumo.  
- **Escalabilidade**: A nuvem ajusta automaticamente a potência necessária para suas necessidades.  

---

## Modelos de Serviços de Nuvem
1. **IaaS (Infraestrutura como Serviço)**  
2. **PaaS (Plataforma como Serviço)**  
3. **SaaS (Software como Serviço)**  

---

## O que é Serverless Computing?
- Modelo de computação em que o provedor gerencia automaticamente a infraestrutura necessária.  
- Você foca apenas no código, sem se preocupar com hardware, servidores ou balanceamento de carga.  
- **Exemplo**: Funções ativadas por eventos.  

---

## Tipos de Nuvem
1. **On-premises**: Datacenter local.  
2. **Hybrid Cloud**: Combinação de datacenter local e nuvem.  
3. **Off-premises**: Totalmente na nuvem.  

---

## Infraestrutura do Azure
- **Componentes**: Infraestrutura física e redes.  
- Mais de 160 datacenters divididos por regiões.  
- Estrutura hierárquica:  
  - Geografia → Região → Zona de Disponibilidade.  

### Zona de Disponibilidade
- Datacenters independentes dentro de uma região.  
- Cada zona possui no mínimo um datacenter.  

### Pares de Regiões
- Conexões redundantes entre regiões na mesma geografia, proporcionando alta disponibilidade e recuperação de desastres.  

---

## Azure Marketplace
- Catálogo de produtos e soluções prontos para uso na Azure.  

---

## Azure Pricing
- **TCO**: Calcula custos atuais e futuros na nuvem.  
- **Pricing by Product**: Estima preço por serviço.  
- **Pricing Calculator**: Monta a infraestrutura e avalia os custos.  

### Tipos de pagamento para VMs:
1. **Pay as you go**: Pague conforme o uso.  
2. **Instâncias Reservadas**: Contratação por períodos específicos, mais barato.  
3. **Instâncias Spot**: Usam capacidade ociosa, com custo reduzido, mas podem ser interrompidas.  

---

## Grupos de Recursos e Contas
- **Grupo de Recursos**: Organização dos recursos criados.  
- **Billing Account**: Conta administrativa.  
- **Subscription**: Inscrição ou assinatura de serviços.  

---

## Tipos de Suporte
1. Básico  
2. Developer  
3. Standard  
4. Professional Direct  

---

## CLI Comandos Básicos
- Criar um grupo de recursos:  
  ```bash
  az group create --location westus --resource-group labazcli



Azure Functions: Executa códigos disparados por eventos.
Azure VNet: Reserva 5 IPs por sub-rede.
Load Balancer: Camada 4.
Application Gateway: Camada 7.
VPN Gateway: Conecta redes locais com a Azure.
Express Route: Link dedicado sem passar pela internet.
Azure CDN: Reduz latência armazenando dados em cache regional.



Azure Functions: Executa códigos disparados por eventos.
Azure VNet: Reserva 5 IPs por sub-rede.
Load Balancer: Camada 4.
Application Gateway: Camada 7.
VPN Gateway: Conecta redes locais com a Azure.
Express Route: Link dedicado sem passar pela internet.
Azure CDN: Reduz latência armazenando dados em cache regional.
