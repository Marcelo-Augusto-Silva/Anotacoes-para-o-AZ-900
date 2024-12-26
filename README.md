# Anotaçoes para o AZ-900
 Anotaçoes para o AZ-900


Vanatagens da Computação em nuvem:
    - Alta disponibilidade 
    - Escalabilidade 
    - Agilidade
    - Distribuição Geografica 
    - Disaster Recovery

Por que a computação em nuvem normalmente é mais barata ?

    Baixo custo de operação
    Pay as you go = Pague pelo o que usar, voce so paga o que usar, se usa muito paga mais se usa menos, paga menos
    Escalabilidade = a nuvem pode escalar a potencia da maquina 


Modelo de Serviços de nuvem

    Iaas = Infraestrutura como serviço
    Paas = Plataforma como serviço
    Saas = Software como serviço

O que é Serverless computing ?

    Infraestrutura sem ser gerenciada, você não vai se preocupar com o Hardware.
    Você não se preocupa com a infraestrutura 


    Serverless Computing é um modelo de computação em nuvem em que você pode executar códigos e aplicativos sem se preocupar com a infraestrutura subjacente, como servidores, balanceamento de carga ou provisionamento de recursos. Apesar do nome "serverless" (sem servidor), isso não significa que não há servidores. Em vez disso, os servidores são gerenciados automaticamente pelo provedor de nuvem, permitindo que você se concentre apenas no código.


Tipos de Nuvem:

    On premisses = Dentro do seu datacenter

    Hybrid CLoud = Nuvem hibrida, dentro do seu data center e na nuvem

    Off premisses = Totalmente na nuvem 


Infraestrutura do Azure

    Dois componentes, infraestrutura fisica e os componentes de redes

    Mais de 160 Datacenters divididos em regioes


    Geografia 
        Regiao
            ZOna de disponibilidade

    
    Zona de disponibilidade são Datacenters fisicos separados em regios do azure.
    Cada Zona de disponibilidade é composto por um Datacenter ou mais
    Cada Zona de disponibilidade é independente de cada uma

     
    Pares de Regioes 

        Pares de Regiões (Region Pairs) são um conceito utilizado no Microsoft Azure para criar um vínculo entre duas regiões da nuvem dentro da mesma geografia, proporcionando alta disponibilidade, recuperação de desastres e conformidade legal. Cada região no Azure está emparelhada com outra região dentro da mesma geografia (quando possível), formando um "par de regiões". Isso permite uma série de vantagens em termos de redundância e continuidade dos serviços.

    Azure Marketplace

        É os produtos que a azure tem pronto 


    
    Azure pricing:

        link: https://azure.microsoft.com/en-us/pricing/

        Serve para calcular o valor 

        TCO - calcular os custos que voce tem, com os custos que voce vai ter na nuvem

        Pricing by product - Calcula o preço por produtos

        Pricing calculator - Voce monta a infra e ve quanto que vai ficar


    Tipos de pagamentos:

        VMs:
            Pay as you go = Paga pelo o que usar

            Instancias reservadas = Voce reserva a instancia por um periodo especifico, sai mais barato 

            Instancias Spot = Permite usar a capacidade ociosa das VMs,, o custo é muito mais barato, ELAS PODEM SER INTERROMPIDAS 




    Grupo de Recursos:

        Serve para organizar os recursos criados

    
    Billing Account = Conta do administrador 

    Subscripition = Inscriçoes 


    Tipos de Suporte;

        Basico

        Developer

        Standard 

        Professional Direct





    
    CLI


        az group create  --location westus --resource-group labazcli =  Esse comando cria um grupo de recurso pela CLI


        az group list | grep name = lista todos os grupos por nome 

        az vm create -n MyVm1 -g labazcli --image Ubuntu2204 --generate-ssh-keys = Cria uma Vm Ubuntu e já gera uma chave SSH


        az group delete --resource-group labazcli = Delete o grupo de recurso 



Anotações Módulo 2 do curso da Alura


    Serviços de COmputação envolvem não só VMs más tambem serviços de Container, serviços de K8s, Azure Functions entre outros 

    App Service, você sobe uma aplicação e a nuvem gerencia toda a infraestrutura para você 
    


    RDP = Remote Desktop, fica na porta 3389

    VMs scale sets serve para gerenciar a infraestrutura automaticamente


    App Service se caracteriza como PAAS



    Windows Virtual Desktop 

        Serve para servir as aplicaçoes do Office ou algum app sem precisar configurar uma maquina virtual, varios usuarios podem acessar ao mesmo tempo, permite multi sessão

        Se caracteriza como PAAS



    Azure functions:

        São funções que você deixa pronto e são disparadas por eventos,, opr exemplo:
            Uma função vai ser ativada se receber requisição de um URL especifica 

            link: https://learn.microsoft.com/pt-br/azure/azure-functions/functions-triggers-bindings?tabs=isolated-process%2Cnode-v4%2Cpython-v2&pivots=programming-language-csharp


        
    Azure VNet:

        O azure reserva cinco IPs dentro de cada sub rede.
            Endereço de Rede
            O gateway
            2 ips reservado para mapear os Ips de DNS
            Endereço de difusão da rede ou seja o de broadcasting 

            
        Existem restrições quanto ao uso de endereços IP dentro dessas sub-redes?
        Sim. O Azure reserva os quatro primeiros e o último endereço, em um total de cinco endereços IP em cada sub-rede.

        Por exemplo, o intervalo de endereços IP de 192.168.1.0/24 tem os seguintes endereços reservados:

        192.168.1.0: endereço de rede.
        192.168.1.1: reservado pelo Azure para o gateway padrão.
        192.168.1.2, 192.168.1.3: reservados pelo Azure para mapear os endereços IP do DNS do Azure para o espaço da rede virtual.
        192.168.1.255: endereço de transmissão de rede.

        link: https://learn.microsoft.com/pt-br/azure/virtual-network/virtual-networks-faq


    hostname -i = mostra o Ip da maquina virtual 

    Load Balancer trabalha na camada 4

    Application Gateway trabalha na camada 7


    VPN Gateway e Express Route 

        VPN Gateway permite conectar a sua rede local com a vnet da nuvem 

        Tambem permite conectar duas redes Vnet da Azure independente da regiao 

        Express Route é você contratar um link dedicado com algum parceiro da nuvem e assim não vai trafegar pela internet 


    Azure CDN = Azure Content Delivery network

        Deixa um cache de dados nos servidores, assim fica mais rapido de obter a informação.

        Exemplo: Você precisa acessar uma informaçao que so tem nos EUA, o CDN deixa informaçoes em cache nos servidores do Brasil assim fica mais rapido de obter as informaçoes


Anotações do curso 3 da Azure



    