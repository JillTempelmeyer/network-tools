---
copyright:
  years: 1994, 2017
lastupdated: "2017-12-01"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# Perguntas Mais Freqüentes

## Como posso atualizar as informações de propriedade para os meus IPs? (SWIP)

O Shared WhoIs Project (SWIP) do ARIN permite que você forneça informações de propriedade para endereços IP em sua conta. Essa ferramenta funciona com o sistema {{site.data.keyword.BluSoftlayer_notm}} WHOIS reverso. Recomenda-se usar as duas ferramentas porque nem todas as ferramentas do WHOIS usam o nosso sistema WHOIS reverso para localizar o proprietário de um bloco de IPs (uma sub-rede). Apenas sub-redes com 8 endereços IP ou mais (sub-redes com uma máscara de sub-rede menor que 30) podem usar o sistema SWIP.

Você pode efetuar SWIP em uma sub-rede acessando **Rede pública-> SWIP** no portal do cliente e selecionando **Swip de sub-rede** próximo ao intervalo da meta.

Na página SWIP é possível executar as tarefas a seguir:

 * **Swip de sub-rede:** enviar uma solicitação ao ARIN para atualizar suas informações de IP com seus dados do WHOIS reverso.<br/>
 * **Atualizar sub-rede:** atualizar o ARIN, se você mudar seus dados do WHOIS reverso.<br/>
 * **Limpar sub-rede:** remover suas informações do ARIN e substituí-las por informações padrão do IBM Cloud.

Também é possível ver o estado de uma Solicitação de SWIP lendo a coluna Status na página SWIP:

 * **Sem SWIP:** a solicitação de SWIP para esta sub-rede ainda não foi fornecida. Os dados de WHOIS listarão {{site.data.keyword.BluSoftlayer_notm}} como o proprietário da sub-rede.
 * **Solicitação esperando ARIN...:** uma solicitação foi enviada, mas estamos esperando uma resposta. Respostas podem levar até três dias.
 * **Limpeza esperando ARIN...:** assim como uma solicitação SWIP, a limpeza das informações do WHOIS pode levar até 3 dias para ser concluída.
 * **IBM processando manualmente...:** às vezes, uma solicitação de SWIP não pode ser processada automaticamente. Nesse caso, o erro é relatado ao {{site.data.keyword.BluSoftlayer_notm}} e devemos corrigir manualmente a transação.
 
