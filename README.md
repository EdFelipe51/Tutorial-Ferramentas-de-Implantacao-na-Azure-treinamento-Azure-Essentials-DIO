# Tutorial-Ferramentas-de-Implantacao-na-Azure-treinamento-Azure-Essentials-DIO
Contéudo do Treinamento Ferramentas de Implantacao na Azure Microsoft Azure Essentials DIO 

1 - O que são as ferramentas de linha de comando do Azure?
    
    As ferramentas de linha de comando do Azure automatizam operações de rotina, padronizam failovers de banco de dados e      efetuam pull de informações que fornecem insights avançados. Além de oferecerem a capacidade de escalar suas tarefas       no Azure, as ferramentas de linha de comando facilitam o compartilhamento de um script, que é muito mais fácil do que      uma página wiki extensa com capturas de tela demoradas. Nem sempre é necessário usar uma ferramenta de linha de            comando do Azure, mas saber como usar essas ferramentas é muito útil.

2 - Qual é a diferença entre cloud power shell, bash, CLI e power shell?

    2.1 - A CLI do Azure (interface de linha de comando do Azure) é um conjunto de comandos usado para criar e gerenciar             recursos do Azure

    2.2 - O Azure Cloud Shell é uma ferramenta poderosa que permite executar comandos do Azure diretamente no navegador,             sem a necessidade de instalar o Azure CLI ou o Azure PowerShell em sua máquina local.

    2.3 - O Bash é um interpretador de linha de comando para sistemas Unix e Linux. Ele atua como uma interface entre a              pessoa usuária e o sistema operacional, permitindo a execução de comandos e scripts para realizar várias                   atividades. De maneira geral, a interação acontece com o uso de comandos de texto.

    2.4 - PowerShell é um programa de automação de tarefas e gerenciamento de configuração da Microsoft, consiste em um              shell de linha de comando e a linguagem de script associada. arefas administrativas são geralmente executadas              por meio de cmdlets (pronuncia-se command-lets ), que são classes .NET especializadas que implementam uma                  operação específica. Elas funcionam acessando dados em diferentes armazenamentos de dados, como o sistema de               arquivos ou o Registro do Windows, que são disponibilizados ao PowerShell por meio de provedores .                         Desenvolvedores terceirizados podem adicionar cmdlets e provedores ao PowerShell. Os cmdlets podem ser usados ​​             por scripts, que podem, por sua vez, ser empacotados em módulos. Os cmdlets funcionam em conjunto com a API .NET    

3 - A CLI do Azure e o Azure PowerShell são ferramentas de linha de comando que permitem criar e gerenciar recursos do         Azure. Ambos são multiplataforma, instaláveis no Windows, no macOS e no Linux.

          3.1 - CLI do Azure

                Interface de linha de comando multiplataforma, instalável no Windows, macOS, Linux

                É executada no Windows PowerShell, Cmd ou Bash e outros shells do Unix.

          3.2 - PowerShell do Azure

                Módulo do PowerShell multiplataforma, executado no Windows, macOS, Linux

                Requer Windows PowerShell ou PowerShell    

4 - Ambientes de shell diferentes

    Windows PowerShell, PowerShell, Cmd e Bash são ambientes de shell. Seu ambiente de shell não apenas determina quais        ferramentas você pode usar, mas também altera sua experiência de linha de comando.

    Por exemplo, para o caractere de continuação de linha, o Bash usa a barra invertida \ enquanto que o Windows               PowerShell usa o acento grave `.As diferenças no ambiente de shell não alteram como a CLI do Azure e o Azure               PowerShell funcionam. No entanto, alteram sua experiência de linha de comando.

    A CLI do Azure tem um instalador que torna seus comandos executáveis em todos os quatro ambientes de shell.

    O Azure PowerShell é um conjunto de cmdlets empacotados como um módulo do PowerShell chamado Az; não um executável. O      Windows PowerShell ou o PowerShell devem ser usados para instalar o módulo Az.

    O Windows PowerShell é o shell de script padrão que vem pré-instalado com a maioria dos sistemas operacionais Windows.     O PowerShell é uma instalação autônoma que usa o .NET Core como seu runtime, permitindo que ele seja instalado no          macOS, Linux e Windows.

Obs.: Pontos principais:

O AzureRM é um módulo do PowerShell que ainda é indicado para administração do Azure com o PowerShell. No entanto, ele foi substituído pelo Azure PowerShell e sua data oficial de desativação é 29 de fevereiro de 2024.
Se você estiver usando o AzureRM, poderá migrar o Azure PowerShell do AzureRM para o Az.

5 - Azure Resource Manager 

    Simplifica o gerenciamento de recursos de aplicativo

    5.1 - Implantar recursos de aplicativos:

          O Azure Resource Manager permite que você implante repetidamente seu aplicativo e tenha confiança de que os                recursos sejam implantados em um estado consistente. Você define a infraestrutura e as dependências do                     aplicativo em um modelo declarativo único. Esse modelo é flexível suficiente para usar em todos seus ambientes,            como os ambientes de teste, de preparo ou de produção. Se você criar uma solução no Azure Marketplace, a solução           incluirá automaticamente um modelo que pode ser usado para seu aplicativo.

    5.2 - Organizar os recursos:

          O Azure Resource Manager facilita o gerenciamento e a visualização de recursos no seu aplicativo. Você não                 precisa mais implantar partes do aplicativo separadamente e fixá-las manualmente. Você coloca os recursos com um           ciclo de vida comum em um grupo de recursos que pode ser implantado ou excluído em uma única ação. É possível              ver quais recursos estão vinculados por uma dependência. É possível aplicar marcas a recursos para categorizá-             los para tarefas de gerenciamento, como cobrança.

    5.3 - Controlar acesso a recursos:
    
          Com o Azure Resource Manager, você pode controlar quem da organização pode executar ações nos recursos. É                  possível gerenciar permissões definindo funções e adicionando usuários ou grupos às funções. Para recursos                 críticos, é possível aplicar um bloqueio explícito que evita que os usuários excluam ou modifiquem o recurso. O            Azure Resource Manager cria logs de todas as ações do usuário para que você possa fazer auditorias. Para cada              ação, o log de auditoria contém informações sobre usuário, hora, eventos e status.  

6 - Azure Arc:

    É uma solução de gerenciamento multinuvem e híbrido que permite integrar computadores locais, o Amazon Web Services        (AWS) e o Google Cloud Platform (GCP) ao Azure. 

    O Azure Arc tem diversas funcionalidades, incluindo: 

        Gerenciar servidores físicos do Windows e do Linux, e máquinas virtuais hospedadas fora do Azure 

        Configurar e anexar clusters de Kubernetes em execução em qualquer lugar 
        
        Executar serviços de dados do Azure no local, na borda e em nuvens públicas 
        
        Estender os serviços do Azure para as instâncias do SQL Server hospedadas fora do Azure 
        
        Provisionar, redimensionar, excluir e gerenciar máquinas virtuais 
        
        Validar que os Windows Servers só podem ser acessados pela conta do AAD (Azure Active Directory) atualmente                Microsoft Entra ID ME-ID. 
        
        O Azure Arc pode ajudar a reduzir a complexidade e o custo operacional, especialmente em ambientes grandes,                diversificados e distribuídos.

     O Azure Arc oferece suporte a servidores em execução em qualquer lugar — no local e em qualquer nuvem. Isso inclui         servidores Windows e Linux, físicos e virtuais, ingressados no domínio e não ingressados no domínio.

7 - Azure Bicep

    O Azure Bicep é uma linguagem específica de domínio (DSL) que serve para implantar recursos do Azure. Ele é usado para     criar ambientes na infraestrutura em nuvem, definindo e implantando recursos como máquinas virtuais, contas de             armazenamento e redes virtuais. O Bicep possibilita ao usuário utilizar linhas de programação, para crriar ambientes,      recursos dentro do azure, através de scripts e linhas de comandos 
    
    O Azure Bicep oferece várias vantagens, incluindo: Sintaxe concisa, Segurança de tipos confiável, Suporte para             reutilização de código, Suporte para todos os tipos de recursos e versões de API.

    Caso tenha interesse em conhecer alguns template de BICEP, Azure, acessar o link abaixo:
    
    https://azure.github.io/bicep/
    
    


