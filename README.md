# Prova-Site-Enem
Portal de Inscrição ENEM

Avaliação de Programação Frontend 
Curso: Desenvolvimento de Sistemas – M-TEC 3 DS – Grupo A  
Disciplina: Programação Frontend – 2º Bimestre -  Prof. Engº Sérgio Novais 
Projeto Prático: Front-End - Portal de Inscrição ENEM 
Objetivo do Projeto: 
Desenvolver as interfaces de login e inscrição de um portal simulado do ENEM. O projeto exige a 
estruturação em HTML5, estilização responsiva com CSS3 e validação de dados via 
manipulação de DOM com JavaScript. 
1. Requisitos Visuais e de Estilo (CSS) 
Para manter um padrão visual que remeta aos portais governamentais e educacionais, o projeto 
deve seguir as seguintes diretrizes de design: 
• Paleta de Cores Obrigatória: 
o Cor principal (Cabeçalho e Rodapé): Azul Escuro (ex: #004b87 ou similar). 
o Cor de destaque (Botões): Amarelo (ex: #f1c40f) ou Verde. 
o Fundo da página: Cinza muito claro ou branco, garantindo contraste. 
o Mensagens de erro: Vermelho (ex: #e74c3c). 
• Tipografia: Importar e utilizar uma fonte sem serifa do Google Fonts. 
• Layout Fixo: O cabeçalho e o rodapé devem estar fixos em ambas as páginas. O 
conteúdo central deve rolar normalmente. Centralizar o formulário na tela e alinhar os 
campos internamente. 
• Responsividade: O layout deve se adaptar bem tanto em telas de computadores 
quanto em dispositivos móveis. 
2. Estrutura das Páginas (HTML) e Navegação 
O projeto será composto por dois arquivos .html distintos. A navegação entre eles não deve usar 
a tag <a> para as ações principais, mas sim redirecionamento via JavaScript. 
Página 1: index.html (Tela Inicial / Login) 
Esta é a porta de entrada do sistema. A página deve conter: 
• Cabeçalho com o título "Portal do Candidato - ENEM". 
• Um cartão centralizado contendo: 
o Campo de E-mail. 
o Campo de Senha. 
o Botão "Entrar" (que fará a validação dos dados). 
o Botão ou texto interativo "Cadastrar Novo Usuário" (que, ao ser clicado, usa JS 
para redirecionar o usuário para a página de formulário). 
• Rodapé com informações de direitos autorais. 
Página 2: cadastro.html (Tela de Inscrição) 
Esta tela conterá a ficha completa do candidato. Deve conter os mesmos cabeçalho e rodapé da 
primeira tela, e os seguintes campos estruturados: 
1. Nome Completo 
2. E-mail 
3. Telefone 
4. Nome da Mãe 
5. Nome do Pai 
6. Endereço (Rua/Avenida) 
7. Número 
8. Cidade 
9. Estado 
10. País 
11. Situação do Ensino Médio: (Já concluí ou Estou cursando). 
12. Tipo de Escola: (Pública ou Privada). 
13. Senha 
14. Confirmar Senha 
15. Botão "Salvar Inscrição". (redireciona para login). 
16. Botão "Voltar" (redireciona para tela inicial). 
3. Regras de Lógica e Validação (JavaScript) 
O JavaScript será o responsável por garantir que o usuário preencha os dados corretamente 
antes de prosseguir. 
Regras de Validação de Input: 
• E-mail: Deve obrigatoriamente conter o caractere @. 
• Senha: Deve ter no mínimo 8 caracteres e conter pelo menos uma letra maiúscula. 
• Confirmação de Senha: O valor digitado no campo "Confirmar Senha" (na página de 
cadastro) deve ser exatamente igual ao do campo "Senha". 
Feedback Visual de Erro (Manipulação de DOM): 
• Proibido usar alert() para erros de validação. 
• Se o usuário errar qualquer uma das regras acima (no login ou no cadastro), o JavaScript 
deve impedir o envio do formulário (event.preventDefault()) e injetar dinamicamente 
uma mensagem de erro em texto vermelho diretamente na tela, logo abaixo do campo 
de input que falhou (ex: "A senha deve conter no mínimo 8 caracteres e uma letra 
maiúscula"). 
Ação de Sucesso: 
• Na página cadastro, se o usuário preencher tudo corretamente e clicar em "Salvar 
Inscrição", o sistema deve: 
1. Emitir um alert() simples com a mensagem: "Inscrição salva com sucesso!". 
2. Redirecionar o candidato automaticamente de volta para a página inicial. 
Obrigatório: 
Envio do projeto no Github em tempo de prova. 
