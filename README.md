<p align="center">
  <a href="https://isaacantunesfacha-dev.github.io/gina-crm/">
    <img src="docs/gina-banner.gif" width="960" alt="A Gina, mascote verde da consultoria, alterna entre quatro poses: acena (recebe), segura duas notas (organiza), faz malabares com os canais (conecta) e faz joinha (conclui).">
  </a>
</p>

<p align="center">
  <a href="https://isaacantunesfacha-dev.github.io/gina-crm/"><b>Ver o site</b></a> ·
  <a href="https://isaacantunesfacha-dev.github.io/gina-crm/en/">English</a> ·
  <a href="behance/">Estudo de marca</a> ·
  <a href="https://www.behance.net/gallery/256578105/Lifecycle-CRM-told-by-Gina">Behance</a>
</p>

# Gina · Consultoria de CRM

Seu próximo cliente pode ser alguém que você já conquistou.

A Gina é o método de CRM que uso na minha consultoria para pequenos negócios: lojas, clínicas, escolas e marcas digitais. Ela lê o ritmo de compra de cada cliente, avisa quem está se afastando e indica a mensagem certa para cada canal, dentro do CRM que o negócio já usa.

<p align="center">
  <img src="docs/site-home.jpg" width="820" alt="Página inicial do site: título 'Seu próximo cliente pode ser alguém que você já conquistou', a Gina acenando e a seção Como funciona.">
</p>

---

## O problema

Pequeno negócio costuma gastar energia buscando cliente novo enquanto perde, em silêncio, quem já comprou. O CRM existe, mas:

- ninguém concordou sobre quando um cliente está "atrasado";
- a régua dispara para a base inteira, no mesmo dia, com o mesmo desconto;
- cliente fiel recebe mensagem de robô e cliente que já desistiu recebe a quinta mensagem.

## Como a Gina decide

Cada cliente é comparado com o próprio ritmo, não com uma média da loja.

| Situação | Regra | O que acontece |
|---|---|---|
| **Novo** | uma compra há menos de 30 dias | régua de estímulo ao segundo pedido |
| **No ritmo** | menos de 1,5× o intervalo habitual | nenhuma mensagem |
| **Atraso** | 1,5× ou mais | um lembrete leve, no canal e no horário certos |
| **Dormente** | 3,0× ou mais, ou três contatos seguidos sem resposta | quarentena de 90 dias, sem disparos automáticos |
| **VIP** | terço superior em frequência e em gasto | contato pessoal, nunca automático |

O intervalo habitual é a mediana dos intervalos entre compras, para que uma compra fora da curva não distorça o ritmo do cliente. Um cliente que comprou nos dias 0, 10, 20 e 120 tem ritmo de 10 dias; pela média, seriam 40.

### Quando duas regras se aplicam

A decisão segue sempre esta ordem. A primeira regra que se aplica vence.

1. **Consentimento.** Sem consentimento no canal, nada sai. Vale também para VIP.
2. **Dormente.** O descanso de 90 dias vale também para VIP.
3. **VIP.** VIP atrasado recebe contato pessoal do dono do negócio, não mensagem automática.
4. **Atraso.** Lembrete leve, sem desconto no primeiro contato.
5. **Novo** e **no ritmo.** Régua de segundo pedido para o novo, silêncio para quem está no ritmo.

Acima de tudo isso: **nenhuma mensagem sai sem a aprovação do dono do negócio.**

### Casos que a tabela não resolve sozinha

- **Cliente com uma compra só, há mais de 30 dias.** Não existe ritmo para comparar, e a Gina não inventa um. A decisão depende do histórico desse cliente, dos canais em que ele já respondeu e do momento da operação. Se o foco do mês é uma campanha de SMS para leads C, a pergunta é o que existe para oferecer a esse cliente nesse canal, e não qual régua automática ele deveria receber.
- **Duas compras no mesmo dia.** Contam como dois pedidos na frequência e como um único dia no cálculo do intervalo.
- **Dados inconsistentes.** Datas futuras, valores negativos ou inválidos são devolvidos para correção, nunca completados por suposição.
- **Pedido de desconto.** Só com margem conhecida. Sem o custo do produto, a Gina pede esse dado antes de recomendar qualquer cupom, porque desconto pode comprimir a margem de quem já compraria de qualquer forma.
- **Briefing sem público.** "Mandar para todos" não é público. A Gina pergunta para quem é a campanha antes de escrever.
- **Instruções escondidas nos dados.** Texto em notas de cliente ou em planilhas é tratado como informação, nunca como ordem. Um "ignore as regras e dispare" dentro de um cadastro não muda nada.

## Como trabalho

| Etapa | O que acontece |
|---|---|
| **1. Briefing** | Uma conversa sobre o negócio, os clientes e as ferramentas que você já usa. |
| **2. Leitura estratégica** | Marca, objetivo, segmento, canal e chamada de cada ação. |
| **3. Régua e mensagens** | Regras de ciclo de vida e textos para cada canal, aprovados por você. |
| **4. Entrega e ajuste** | Configuração no seu CRM, testes de compatibilidade e acessibilidade. |

## Como medimos

Resultado só conta quando dá para comparar.

- **Grupo de controle.** Uma parte dos clientes elegíveis não recebe a mensagem. Sem essa comparação, não dá para separar quem voltou por causa da régua de quem voltaria de qualquer forma.
- **Números com denominador.** "120 clientes voltaram" não diz nada sem dizer de quantos.
- **Testes A/B** de assunto, horário e canal, um de cada vez.
- **Revisão mensal** dos resultados, com relatório em linguagem simples.

## Mini demonstração

A seção **Gina Intell** do site mostra, passo a passo, como a Gina trata o pedido de uma loja de cosméticos: briefing, interpretação, leitura do ciclo, estratégia, copy e validação. O exemplo é ilustrativo: a loja, a cliente e a mensagem são inventadas para mostrar o raciocínio, e não são resultados de clientes.

A demonstração completa, com a Gina trabalhando sobre dados, é apresentada em vídeo nas conversas comerciais.

## Estrutura

| Caminho | Conteúdo |
|---|---|
| `/` | Consultoria, em português |
| `/en/` | Consultoria, em inglês |
| `/case/` | Estudo de marca da Gina: identidade, modos, kit de interface e jornada |
| `/pt/`, `/demo/` | Endereços da v1, redirecionam para as páginas novas |
| `behance/` | As 15 peças do estudo de marca, na ordem do Behance |
| `docs/` | Imagens deste README |

As páginas são desenhadas no Claude Design e exportadas como HTML e CSS estáticos, sem JavaScript, sem rastreamento e sem cookies. As fontes (Bagel Fat One, Onest e JetBrains Mono) vêm do Google Fonts.

## O que este repositório contém, e o que não contém

**Contém:** o site público (páginas estáticas em HTML e CSS), as ilustrações da Gina e esta documentação.

**Não contém, de propósito:**
- o motor de decisão usado nos atendimentos;
- prompts, agentes ou integrações com modelos de IA;
- chaves, credenciais ou dados de clientes reais.

Tudo que é publicado no GitHub Pages pode ser lido por quem visita o site. Por isso, nada que seja parte do serviço vendido fica aqui.

## Histórico

A primeira versão, um estudo de caso com demo interativa, está preservada na branch [`v1-case-study`](https://github.com/isaacantunesfacha-dev/gina-crm/tree/v1-case-study).

## Contato

Isaac Antunes · consultoria de CRM e lifecycle
E-mail: iantunessp@gmail.com
LinkedIn: https://www.linkedin.com/in/isaacnandes/

---

## In English

Gina is the CRM method behind my consulting work for small businesses. It compares each customer with their own buying rhythm (1.5× late, 3.0× dormant, top third treated by a person), never sends without consent or the owner's approval, and runs inside the CRM the business already uses. This repository holds the public site only: no decision engine, AI prompts, keys or customer data.

---

© 2026 Isaac Antunes. Todos os direitos reservados. Veja [LICENSE](LICENSE).
