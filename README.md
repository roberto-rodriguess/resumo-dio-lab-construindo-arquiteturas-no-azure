# resumo-dio-lab-construindo-arquiteturas-no-azure

Neste laboratório prático para a certificação AZ-900, foram explorados conceitos fundamentais do Azure e a criação de recursos básicos na plataforma.

### Infraestrutura Global do Azure

A Microsoft Azure possui mais de 60 regiões ao redor do mundo, que podem ser visualizadas através do site [azure.microsoft.com](http://azure.microsoft.com/) ou [datacenters.microsoft.com](http://datacenters.microsoft.com/). Pontos importantes:

- O globo interativo permite explorar todas as regiões disponíveis
- No Brasil, existem duas regiões: Brasil South (São Paulo) e Brasil Southeast (Rio de Janeiro)
- Brasil South replica dados para os Estados Unidos
- Brasil Southeast é reservada para clientes brasileiros que requerem disaster recovery com considerações de LGPD
- O site oferece um tour virtual pelos datacenters da Microsoft

### Criação de Grupos de Recursos

Um grupo de recursos é uma coleção de recursos que compartilham o mesmo ciclo de vida, permissões e políticas. Durante a demonstração:

- Foi criado um grupo de recursos chamado "AZ900-Lab-Jill" na região East US 2
- As tags/marcações são opcionais, mas úteis para organização de custos e atribuição de centro de custos
- O permissionamento deve seguir o princípio do menor privilégio possível
- É possível configurar bloqueios para evitar exclusões acidentais ou maliciosas
- O Log de Atividades registra todas as ações realizadas no grupo de recursos

### Criação de Rede Virtual

Foi demonstrada a criação de uma rede virtual (VNet):

- A VNet foi criada na região Brasil South, enquanto o grupo de recursos estava na East US 2
- Recursos podem estar em regiões diferentes do seu grupo de recursos
- O visualizador de recursos mostra graficamente todos os recursos no grupo
- É possível baixar templates para automatização e implantação via código
