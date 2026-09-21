# Documentação do Projeto: Portfólio Carlos Alexandre

## 01. Definição do Projeto
*   **Nome:** Portfólio Profissional – Carlos Alexandre.
*   **Problema:** Dificuldade de recrutadores e clientes em localizar, de forma centralizada e profissional, a trajetória acadêmica e as competências técnicas (C, Java, PHP) do desenvolvedor.
*   **Objetivo:** Apresentar a trajetória profissional e acadêmica, destacando o TCC e projetos GitHub, para atrair oportunidades.
*   **Público-alvo:** Recrutadores e clientes freelancers.
*   **Proposta visual:** Design minimalista (Branco e Azul), moderno, com cards organizados para leitura rápida.
*   **Conteúdo:** Apresentação, Formação (ETEC/Faculdade), Habilidades, Destaque ao TCC, Projetos GitHub e Contatos.
*   **Principais funcionalidades:** Navegação clara, links para GitHub/E-mail, seção de projetos.
*   **Tecnologias:** HTML5, CSS3, Bootstrap 5. (JavaScript utilizado apenas para funções básicas de interação exigidas pelo requisito técnico).

## 02. Prompts utilizados
*   **Prompt 1 (Estrutura):** "Atue como desenvolvedor web. Crie um arquivo index.html usando Bootstrap 5. O design deve ser minimalista, com paleta branca e azul. Estruture seções para: Sobre (apresentação), Formação (ETEC de Guarulhos ADS - completo e Faculdade IFSP Campus de Guarulhos ADS - Cursando), Habilidades (C, Java, PHP), Projetos (destaque para TCC https://github.com/calegermano/TCC_Remenu e GitHub https://github.com/calegermano) e Contato(carlosalexandre071221@gmail.com). Use HTML semântico."
*   **Prompt 2 (Estilo):** "Crie um arquivo style.css. O design deve parecer moderno e descolado. Use tons de azul para a navbar e detalhes, e branco para o fundo. Aplique sombras suaves nos cards de projetos e mantenha tudo responsivo."
*   **Prompt 3 (Melhora visual):** "Atue como um designer UI/UX especialista em estilos Brutalistas e Dark Academia. Quero elevar o nível visual do meu portfólio.
Fundo e Textura: Substitua o fundo branco padrão por uma composição que intercala áreas de branco sólido com sobreposições de imagens (use placeholders de imagens em preto e branco de estátuas clássicas ou elementos góticos, como no exemplo enviado).
Paleta de Cores: Mantenha o azul cobalto (hex #0000FF ou similar) como cor de destaque vibrante para elementos gráficos, ícones e linhas, em contraste com o fundo branco e preto.
Elementos Gráficos: Use CSS para criar formas geométricas abstratas (triângulos, linhas pontilhadas como grafos, estrelas de quatro pontas) sobrepostas às seções.
Tipografia: Aplique fontes com serifa (estilo clássico) para títulos e uma fonte sem serifa muito leve e espaçada para textos de apoio.
Layout: Quebre o alinhamento perfeito do Bootstrap. Deixe que alguns elementos 'saiam' da grade, sobrepondo imagens ou textos, criando uma colagem digital.
Código: Aplique isso usando CSS puro (pode usar z-index e position: absolute para as sobreposições).
Não perca a legibilidade do conteúdo principal, mas quero que o site pareça uma colagem artística, não um site corporativo padrão."
*   **Prompt 4 (Interação obrigatória):** "Crie um arquivo script.js simples que adicione uma interação básica ao site (como um alerta de boas-vindas ou mudança de cor de um elemento ao clicar), apenas para cumprir a exigência técnica de uso de JavaScript no projeto."

## 03. Histórias de Usuário
*   **US01:** Como visitante, quero ver apresentação e formação, para conhecer o perfil.
*   **US02:** Como recrutador, quero ver competências (C, Java, PHP), para avaliar compatibilidade.
*   **US03:** Como visitante, quero acessar projetos e TCC, para avaliar qualidade técnica.
*   **US04:** Como cliente, quero ver contatos (E-mail/GitHub), para negociar.

## 04. Critérios de aceitação
*   **US01:** Foto/Nome e instituições (ETEC/Faculdade) visíveis e responsivas.
*   **US02:** Cards de habilidades (C, Java, PHP) com ícones.
*   **US03:** TCC em destaque com descrição e link GitHub funcional.
*   **US04:** E-mail e GitHub com links clicáveis.

## 05. Priorização MoSCoW
*   **Must have:** US01, US02, US04.
*   **Should have:** US03 (Projetos).
*   **Could have:** Interação básica via JS.
*   **Won't have:** Integrações com APIs ou formulários complexos.

## 06. Descrição do MVP

*   **Necessidades atendidas:** Apresentação clara do perfil profissional, listagem de competências técnicas (C, Java, PHP) e exposição do histórico acadêmico e projetos (TCC/GitHub).
*   **Seções disponíveis:** Header (Navegação), Sobre (Apresentação), Formação Acadêmica, Habilidades Técnicas, Portfólio (TCC e Projetos) e Rodapé (Contatos).
*   **Interações:** Navegação interna por links (âncoras), abertura de links externos (GitHub/E-mail) e interação simples via JavaScript para feedback visual do usuário.
*   **Histórias inclusas:** US01, US02, US03, US04.
*   **Fora desta versão:** Formulários de contato com banco de dados, integração com redes sociais externas via API e sistemas de busca interna de projetos.
*   **Condições de conclusão:** O portfólio deve ser totalmente responsivo, exibir corretamente a formação e as competências, possuir links operacionais para o GitHub e E-mail, e apresentar a interação obrigatória em JavaScript para que o MVP seja considerado funcional e avaliável.

## 07. Backlog acionável

| ID | Item do Backlog | História | Prioridade | Critérios | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| BL01 | Layout Base (HTML/Bootstrap) | US01 | Must have | Navbar e seções responsivas | A fazer |
| BL02 | Estilização (CSS Azul/Branco) | US01 | Must have | Visual moderno e limpo | A fazer |
| BL03 | Seção Habilidades | US02 | Must have | Cards com C, Java, PHP | A fazer |
| BL04 | Seção Projetos/TCC | US03 | Should have | Links válidos para GitHub | A fazer |
| BL05 | Interação JS | US03 | Could have | Script de interação básica | A fazer |
| BL06 | Contatos (Rodapé) | US04 | Must have | Links de E-mail e GitHub | A fazer |
