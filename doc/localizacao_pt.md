# Convenções de tradução para scripts

Estas diretrizes ajudam a manter consistência nas traduções dos scripts sem alterar sua lógica.

## Preservar comandos e estrutura do script
- **Não** modifique comandos ou funções dos scripts (por exemplo: `select`, `mes`, `dispbottom`, `getitem`, `close`, `next`).
- Mantenha variáveis, labels e nomes de scripts intactos; apenas o texto exibido ao jogador deve ser traduzido.
- Respeite a ordem e a quantidade de parâmetros; alterações podem quebrar a execução do script.

## Estilo de tradução
- Traduza somente diálogos, descrições e mensagens exibidas.
- Use português claro e consistente, evitando regionalismos e gírias.
- Preserve o tom original (formal/informal) quando aplicável.

## Termos padronizados
Use os termos abaixo de forma consistente ao longo dos scripts:

- **Armazém**: tradução padrão para *Storage*.
- **Guerreiro**: use para *Swordman* (evite "Espadachim").
- **Mercador**: use para *Merchant*.
- **Ferreiro**: use para *Blacksmith*.
- **Sacerdote**: use para *Priest*.
- **Caçador**: use para *Hunter*.
- **Cavaleiro**: use para *Knight*.
- **Bruxo**: use para *Wizard*.
- **Monge**: use para *Monk*.
- **Arruaceiro**: use para *Rogue*.
- **Ferreiro Mestre**: use para *Mastersmith*.

## Revisão e consistência
- Revise mudanças verificando se comandos e variáveis permaneceram intactos.
- Compare com outras traduções existentes para manter uniformidade nos termos.
- Em caso de dúvida, prefira manter o termo previamente adotado no projeto.
