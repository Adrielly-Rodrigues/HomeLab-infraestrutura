🖥️ Infraestrutura Windows Server 2019 com Active Directory, DNS e DHCP

📋 Descrição do Projeto
Este projeto teve como objetivo implementar uma infraestrutura de rede corporativa utilizando Windows Server 2019 em ambiente virtualizado através do Oracle VirtualBox.
Durante o desenvolvimento foram configurados e integrados os serviços de Active Directory Domain Services (AD DS), DNS e DHCP, criando um ambiente de domínio funcional para gerenciamento centralizado de usuários, computadores e recursos da rede.
O projeto também contemplou a criação de Unidades Organizacionais (OUs), usuários, escopos DHCP, resolução de nomes via DNS e testes de comunicação entre clientes e servidor.

🎯 Objetivos
Configurar um servidor Windows Server 2019.
Implementar um Controlador de Domínio (Domain Controller).
Configurar o serviço DNS.
Configurar o serviço DHCP.
Criar usuários e estruturas organizacionais.
Integrar clientes Windows ao domínio.
Validar a comunicação da rede.

🛠️ Tecnologias Utilizadas
Windows Server 2019 Standard
Windows 10 Cliente
Active Directory Domain Services (AD DS)
DNS Server
DHCP Server
Oracle VirtualBox
IPv4
TCP/IP

🌐 Configuração do Servidor
Servidor
Nome: SRV-REV
Domínio: REVAD.LOCAL

IP: 10.10.10.10
Máscara: 255.255.255.0
Gateway: 10.10.10.1
DNS: 10.10.10.10
O servidor foi configurado com endereço IP estático para garantir estabilidade aos serviços de rede.

🏢 Active Directory Domain Services (AD DS)
Foi realizada a instalação e configuração do Active Directory Domain Services, promovendo o servidor como Controlador de Domínio.
Domínio criado
REVAD.LOCAL

Benefícios
Gerenciamento centralizado de usuários.
Gerenciamento de computadores.
Controle de autenticação.
Administração de recursos da rede.
📂 Estrutura Organizacional (OUs)
Durante as atividades práticas do SENAC, foram criadas diversas Unidades Organizacionais (Organizational Units - OUs) dentro do domínio REVAD.LOCAL, simulando a estrutura administrativa de uma empresa real.
Essa organização permite separar usuários, grupos, computadores e recursos por setor, facilitando o gerenciamento e aplicação de políticas de segurança.
REVAD.LOCAL

│

└── SENAC

    │
    
    ├── SAND

    │
    
    └── SMIG
        │
        ├── Almoxarifado
        ├── Auditoria
        ├── Comercial
        ├── Compras
        ├── Computadores
        ├── Contabilidade
        ├── Diretoria
        ├── Diversos
        ├── Filantropia
        ├── Financeiro
        ├── Geral
        ├── Grupos
        ├── Jovem Aprendiz
        ├── Jurídico
        ├── Logística
        ├── Marketing
        ├── Produção
        ├── Qualidade
        ├── Recepção
        ├── Recursos Humanos
        ├── SAC
        ├── Servidores
        └── Usuários

👥 Gerenciamento de Usuários
Foram criadas contas de usuários para autenticação no domínio.

Usuários cadastrados
Maria Aparecida de Souza
Joana Candido
Robson Medeiro
Suporte Smig
User Printer

Configurações aplicadas
Senha inicial criada pelo administrador.
Obrigatoriedade de alteração da senha no primeiro acesso.
Organização dos usuários em OUs específicas.
Administração centralizada pelo Active Directory.

🌎 Configuração do DNS
Foi instalado e configurado o serviço DNS integrado ao Active Directory.
Funções do DNS
Resolução de nomes da rede.
Localização do controlador de domínio.
Suporte ao processo de autenticação.
Comunicação entre servidor e clientes.

📡 Configuração do DHCP
Foi instalado e configurado o serviço DHCP para distribuição automática de endereços IP.
Escopo criado

DHCP-REVAD
Recursos configurados
Faixa de distribuição de endereços IPv4.
Máscara de rede.
Gateway padrão.
DNS da rede.
Exclusão de endereços reservados.
Controle de concessões ativas.

📋 Validação do DHCP
O servidor DHCP distribuiu automaticamente endereços IP aos clientes da rede.
Concessões Ativas
10.10.10.146
10.10.10.147
As concessões puderam ser visualizadas diretamente no console DHCP do servidor.

🖥️ Integração Cliente-Servidor
Uma máquina Windows 10 foi configurada para receber parâmetros de rede automaticamente via DHCP.
Configuração recebida
Endereço IPv4: 10.10.10.147
Máscara:
255.255.255.0
Servidor DHCP:
10.10.10.10
Servidor DNS:
10.10.10.10
Isso demonstra o correto funcionamento dos serviços DHCP e DNS.

✅ Testes de Conectividade
Teste de Resolução DNS
Comando executado:
ping REVAD.LOCAL
Resultado:
Disparando REVAD.LOCAL [10.10.10.10]
Pacotes enviados: 4
Pacotes recebidos: 4
Perdidos: 0
Mínimo = 0 ms
Máximo = 0 ms
Média = 0 ms
O resultado confirmou que o DNS está resolvendo corretamente o nome do domínio para o endereço IP do servidor.

Teste de Comunicação com o Servidor
Comando executado:
ping 10.10.10.10
Resultado:
Pacotes enviados: 4
Pacotes recebidos: 4
Perdidos: 0
Mínimo = 0 ms
Máximo = 0 ms
Média = 0 ms
O teste confirmou comunicação total entre cliente e servidor.

✅ Resultados Obtidos
Implantação de um Controlador de Domínio funcional.
Configuração do Active Directory.
Configuração do DNS integrado ao domínio.
Configuração do DHCP para distribuição automática de IP.
Criação de estrutura organizacional através de OUs.
Cadastro e gerenciamento de usuários.
Integração de clientes Windows ao ambiente.
Validação da resolução de nomes.
Validação da distribuição automática de endereços IP.
Comunicação entre cliente e servidor com 0% de perda de pacotes.

📚 Conhecimentos Desenvolvidos
Administração de Windows Server 2019
Active Directory
DNS
DHCP
Gerenciamento de Usuários
Estruturação de OUs
Redes TCP/IP
Serviços Microsoft
Virtualização com Oracle VirtualBox
Infraestrutura de Redes
Administração de Domínio
Troubleshooting de Redes

🏆 Conclusão
Ao final do projeto foi implantada uma infraestrutura corporativa completa em ambiente virtualizado, contemplando autenticação centralizada por Active Directory, resolução de nomes via DNS, distribuição automática de endereços IP por DHCP e gerenciamento de usuários e computadores através de Unidades Organizacionais.
Os testes realizados comprovaram o correto funcionamento da comunicação entre cliente e servidor, bem como a integração entre todos os serviços configurados, simulando um ambiente empresarial real baseado em Windows Server 2019.
