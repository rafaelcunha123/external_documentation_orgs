##Cadastro de Pacientes

* **Não encontrei um paciente**: Se a busca por CPF ou por Nome não retornar nenhum resultado, o paciente não está cadastrado na plataforma. Deve ser realizado um novo cadastro para o mesmo.
* **CPF já está sendo usado**: O CPF que já está sendo por outro perfil cadastrado na plataforma. Faça uma busca por CPF e encontre esse perfil. Corrija o CPF do perfil errado colocando o CPF correto, ou marcando o paciente com CPF incorreto como dependente.
* **Não encontrei o convênio no paciente**: verique se o convênio está cadastrado no perfil do paciente. Se estiver cadastrado e ainda assim nenhum convênio for encontrado, isso significa que os outros filtros selecionados impedem o agendamento para este convênio. Por exemplo, se o paciente tiver o convênio Intermédica cadastrado, mas o profissional selecionado não aceitar esse convênio, retornaremos que o convênio não foi encontrado.

##Agendamento
* **Não encontramos nenhum horário disponível para a sua busca**: A busca sempre é feita dentro de um determinado mês. Caso não encontremos um horário disponível, mostraremos a próxima data com um horário disponível no centro da tela. Caso nenhuma data seja retornada, será necessário [abrir uma nova agenda](../gestao_profissionais/abrir_agendas.md) para o profissional.