# Azure-104
Curso dio Azure 103

Etapa 1) Iniciando com a criação.
**Nota importante maquina virtual é um modelo de infraestrutura como serviço. O que significa que a Microsoft só precisa deixar o ambiente funcionando.
Demais itens como configuração e backups e de responsabilidade do administrador.**
 1.1 primeiro passo criar um resource group isso permite que você possa como o proprio nome sugere um recurso dentro deste local.
 1.2 Ir em maquina virtuais e criar maquina virtual
  1.2.1 Basico
  Na primeira tela. será adicionado resource group que recem criamos. caso não haja tem um botão para criar nesse local
  O nome da Maquina virtual a zona a qual pertence. lembrando que procurar sempre alocar o o recurso o mais proximo possivel do usuario.
  As Zonas de disponiveis.
  O tipo de segurança nesse caso para o teste usamos o padrão.
  Escolher a Imagem do sistema operacional (windows server ou windows 11)
  após isso escolher o tamanho da maquina cirtual, lembrando sempre que isso altera o custo. (CPUs e RAM)
  Criar usuario e Senha para login
  1.2.2 Criar disco
  Escolher o tamanho o default é 127Gib
  O tipo de disco
  Deleter com a VM, para que o disco não fique orfão.
  Os recursos de rede NIC.
  1.2.3 Load Balance.
  Não foi usado nenhum, porém ele serve caso tenha 3 maquinas fazendo o mesmo processo, assim o load balance iria escolher a melhor disponivel.
  1.2.4 Gerenciamento.
  Existe algumas opções
  Entre elas o Backuo que para o cenario de teste não ativamos para produção muito importante o uso.
  1.2.5 Monitoramento
  No caso foi desabilitado o diagnostico. Porem outra feature recomendada para produção.
  1.2.6 Avançado
  Não foi usado nada.
  1.2.7 tags
  Inserido a TAG para rever depois centro de custo.
  1.2.8 Revição e Criação
  Apertar Criar.
1.3 Dentro o menu da maquina virtual > Tamanho.
é possivel trocar o tamanho com a maquina virtual ativa, porém fazer o processo causara que ela reinicie para absorver o novo parametro selecionado.
1.4 Dentro o menu da maquina virtual > Disco.
É possivel adicionar disco a maquina virtual e esse processo não reinicia a maquina.
Etapa 2) Desanexar Disco
Dentro o menu da maquina virtual > Disco.
Desanexar o disco, para poder usar em outra maquina virtual.
2.1.1 É possivel criar um Scale Set dentro deste menu você pensa em alta disponibilidade o mais recomendado é o automatico. Uma vex ativo e configurado ele pode aumentar a CPU para atender a demanda.
2.1.2 Tem a opção de disponibilidade que faz que a replicação da maquina seja feita em Hacks diferentes caso um hack desligue outro assuma. lembrando que a opção de domains são sempre impars

  
