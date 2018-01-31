# <img src=../../img/logo.png height=25 style:"float:left"> Recepção

Para iniciar uma recepção, abra a tela de detalhes de um agendamento e clique em iniciar recepção.
Depois disso, a recepção de pacientes tem 4 etapas:
1. [Cadastro](#cadastro)
2. [Foto](#foto)
3. [Cobrança](#cobrança)
4. [Confirmação](#confirmacao)
5. [Impressão impressão](#impressao)




##1. Cadastro {#cadastro}
No cadastro, deve ser feita a validação de dados do paciente, além de cadastro dos dados de convênio.
É necessário que o paciente tenha um CPF único e válido e que tenha ao menos um telefone cadastrado.
O cadastro dos dados de convênio também é feito aqui.

<div class="left-float-framme framme70">
	<img src="../../img/recepcao/cadastro.gif">
</div>

<div class="right-float-framme framme28">
	<ul>
		<li>Abra a recepção de um atendimento</li>
		<li>Verifique e edite os dados de cadastro do paciente</li>
		<li>Dados inválidos devolverão erro com indicação de qual campo deve ser alterado</li>
	</ul>
</div>

<div style="clear: left; margin-bottom: 20px"></div>



##2. Foto {#foto}

**Seção aparece apenas para organizações que contrataram a funcionalidade de reconhecimento facial**

Para tirar foto do paciente, clique no botão verde com o símbolo de câmera. 
Se for a primeira foto do paciente, ela se tornará a base de todos os outros reconhecimentos faciais.
A partir da segunda foto, a análise retornará positiva caso o percentual de reconhecimento facial seja maior que 80%.
Para determinados convênios de saúde o reconhecimento facial servirá como assinatura eletrônica, eliminando a necessidade de impressão da guia do convênio.


<div class="left-float-framme framme70">
	<img src="../../img/recepcao/foto.gif">
</div>

<div class="right-float-framme framme28">
	<ul>
		<li>Garanta alinhamento da face do paciente</li>
		<li>Tire a foto</li>
		<li>Aguarde resultado do reconhecimento facial</li>
	</ul>
</div>

<div style="clear: left; margin-bottom: 20px"></div>

> **Possíveis Problemas**
>  * Não consigo acessar a câmera - na primeira vez que a câmera for utilizada no eDoc seu navegador pedirá autorização para utilizar o aparelho. Dê autorização completa ao navegador para que a camera passe a funcionar no eDoc.
>  * Paciente não foi reconhecido - Daremos um aviso se o paciente não for reconhecido. Confira um documento com foto do paciente para garantir que não há fraude. Caso não haja fraude, permita o atendimento. A foto, o percentual de reconhecimento e o usuário que permitiu o atendimento de um usuário não reconhecido ficarão gravados para análise posterior.



##3. Cobrança {#cobranca}
A cobrança pode assumir 3 formas, dependendo do método de pagamento e do procedimento que o paciente realizará. São eles:
	a) [Atendimento Particular, todos os procedimento](#particular)
	b) [Atendimento por Convênio, Guia de Consulta](#convenio_consulta)
	c) [Atendimento por Convênio, Guia de SP-SADT](#convenio_spsadt)


### Particular, todos os convênios {#particular}
O atendimento particular reque apenas a seleção do procedimento que será realizado, e da quantidade que será realizada.
Por exemplo, no caso de uma consulta, a quantidade realizada será igual a 1. No caso de uma escleroterapia de veias, em geral 5 aplicações são feitas e cobradas na mesma sessão, e a quantidade será 5.
O preço é calculado automaticamente a partir dos contratos, mas caso se deseje dar um desconto, também é possível alterá-lo aqui.

<div class="left-float-framme framme70">
	<img src="../../img/recepcao/cobranca1.gif">
</div>

<div class="right-float-framme framme28">
	<ul>
		<li>Selecione o convênio particular</li>
		<li>Selecione o procedimento que será realizado</li>
		<li>Aponte se o atendimento é um retorno</li>
		<li>Selecione o método de pagamento</li>
		<li>Confira quantidade executada e preço</li>
	</ul>
</div>

<div style="clear: left; margin-bottom: 20px"></div>


> **Importante**
>  * Não será possível voltar e alterar os dados a partir do momento que se finaliza a cobrança - essa é uma medida de segurança para garantir que dados de entrada de caixa não sejam adulterados.


### Convênio, guia de consulta {#convenio_consulta}
Se o atendimento realizado for de um convênio que emite guias no padrão TISS, e se o contrato com o convênio especificar uma Guia de Consulta para a cobrança do procedimento que está sendo realizado, o formulário tem uma pequena alteração.
Além da seleção do convênio, procedimento e retorno, pode-se selecionar se o paciente é Recém Nascido e adicionar um Número da Guia Atribuido Pela Operadora (geralmente em situações de elegibilidade). Todos esses novos campos são **opcionais**.

<div class="left-float-framme framme70">
	<img src="../../img/recepcao/cobranca2.gif">
</div>

<div class="right-float-framme framme28">
	<ul>
		<li>Selecione o convênio</li>
		<li>Selecione o procedimento que será realizado</li>
		<li>Aponte se o atendimento é um retorno, ou atendimento de RN</li>
		<li>[Opcional] Adicione a quantidade realizada</li>
		<li>[Opcional] Adicione o número da guia atribuido pela operadora</li>
	</ul>
</div>

<div style="clear: left; margin-bottom: 20px"></div>


> **Importante**
>  * Após confirmação dos dados de cobrança, o eDoc tentará se comunicar com o convênio para validar elegibilidade e autorização. Caso não obtenha uma resposta ou obtenha uma negativa, abriremos uma mensagem perguntando ao usuário se deseja autorizar manualmente o atendimento
>  * Ao clicar em autorizar, é gravado que o atendimento foi autorizado manualmente pelo usuário. Esse dado é utilizado para análise posterior.


### Convênio, guia de SP-SADT {#convenio_spsadt}
Se o atendimento realizado for de um convênio que emite guias no padrão TISS, e se o contrato com o convênio especificar uma Guia SP-SADT para a cobrança do procedimento que está sendo realizado, o formulário de cobrança mostra todos os campos requisitados para o faturamento correto.

<div class="left-float-framme ">
	<img src="../../img/recepcao/cobranca3.gif">
</div>



<div style="clear: left; margin-bottom: 20px"></div>


> **Importante**
>  * Após confirmação dos dados de cobrança, o eDoc tentará se comunicar com o convênio para validar elegibilidade e autorização. Caso não obtenha uma resposta ou obtenha uma negativa, abriremos uma mensagem perguntando ao usuário se deseja autorizar manualmente o atendimento
>  * Ao clicar em autorizar, é gravado que o atendimento foi autorizado manualmente pelo usuário. Esse dado é utilizado para análise posterior.