<h1 align="center">$ to-do-list</h1>

<p align="center">
Gerenciador de tarefas via linha de comando, feito em Python.
</p>

<p align="center">
<img src="https://img.shields.io/badge/Python-0d1117?style=for-the-badge&logo=python&logoColor=00FF41" />
<img src="https://img.shields.io/badge/CLI-0d1117?style=for-the-badge&logo=gnubash&logoColor=00FF41" />
</p>

---

### > funcionalidades

- Adicionar tarefas com título, descrição e data de vencimento
- Listar tarefas, com filtro por status (`Pendente`, `Concluída`, `Atrasada`)
- Editar título, descrição e data de uma tarefa
- Remover tarefas
- Marcar tarefas como concluídas
- Detecção automática de tarefas atrasadas
- Salvamento automático em arquivo (`tarefas.pkl`), então as tarefas continuam lá depois que você fecha o programa

### > como rodar

```bash
git clone https://github.com/arthurtofoli-tech/to-do-list.git
cd to-do-list
python main.py --help
```

### > uso

```bash
# adicionar (data no formato DD/MM/AAAA)
python main.py adicionar "Estudar Python" "Revisar classes e herança" 20/12/2026

# listar todas
python main.py listar

# listar só as atrasadas
python main.py listar --status Atrasada

# editar a tarefa 1
python main.py editar 1 --titulo "Novo título"

# marcar a tarefa 1 como concluída
python main.py concluir 1

# remover a tarefa 1
python main.py remover 1
```

### > estrutura

```
to-do-list/
├── main.py          # interface de linha de comando (argparse)
├── gerenciador.py   # classe GerenciadorDeTarefas
├── tarefa.py        # classe Tarefa
└── persistencia.py  # salvar e carregar com pickle
```

### > tecnologias

`Python` · `argparse` · `datetime` · `pickle`

<p align="center"><code>$ exit 0</code></p>
