# Diretrizes

Todos os atributos e métodos serão escritos em inglês.
As funções deverão começar com uma ação, escrita em CamelCase
ex, função "comprar recurso":
<type> PurchaseResource(args);

Atributos deverão ser escritos em snake_case
Ex, atributo "fichas de conflito":
<type> conflict_markers;



# Classe player:

## Contributors:
### Pedro
### Rafael


Atributos:
- Tabuleiro - uchar
- Moedas - uchar
- Cartas na mão - array
- Cartas jogadas - array
- Recursos
- Escudos - uchar
- Fichas de Conflito - signed char
- Estágios da maravilha construídos - uchar
- Pontos de vitória - uchar
- Jogadores vizinhos - DMAG::Player

Métodos:
- Construir maravilha - void
- Construir estrutura - void
- Construir guilda - void
- Comprar recurso - int 
- Receber cartas - array
- Descartar - DMAG::Card
- Combate - int
- Calcular pontuação - int

# Classe card:
## Contributors:
### Emilio

Atributos:
- Tipo - uchar
- ID - uchar
- Custo - array
- Recursos - array
- Pontos de vitória - uchar
- Poder militar - uchar
- Especial - a definir
- Era - uchar
- Unidades por qtd. de jogadores - nada
- Grátis com - DMAG::Card
- Grátis para - array<DMAG::Card>

Métodos:
- Pode ser comprada?

# Classe game:

## Contributor
### Julia
### Julio
### Rafael


Atributos:
- Jogadores - array<DMAG::Player>
- Número de jogadores - uchar
- Era - uchar
- Rodada - uchar
- Timer da rodada - nada
- Baralho - array<deque<DMAG::Card>>
- Pilha de descarte - array<DMAG::Card>

Métodos:
- Em jogo - void
- Próxima rodada - void
- Novo jogo - void
- Distribuir cartas - void
- Trocar cartas - void
- Distribuir maravilhas - void
- Escrever em arquivo
- Ler dos arquivos

# Classe logger:

Atributos:

Métodos: