# Cenario 4 - Modelagem UML: laboratorio de ensaios

## Objetivos de aprendizagem

- Modelar um problema com diagrama de classes UML em Mermaid.
- Traduzir o modelo para uma implementacao inicial em `C++` ou `Python`.
- Registrar a entrega com `issue`, `branch`, `commit`, `pull request` e `AI_LOG.md`.

**Tempo estimado:** 2h a 4h

---

## 1. Contexto

Este repositorio e o **starter do aluno** para a atividade.

Aqui voce encontra apenas os arquivos que precisa usar na entrega.
Configuracao de assignment, autograding e rubrica do professor ficam fora deste repositorio.

O dominio do problema e um **laboratorio de ensaios** com equipamentos, sensores e ordens de calibracao.

---

## 2. O que deve ser entregue

- `docs/diagrama_classe.md` preenchido com o diagrama final e as justificativas.
- `docs/modelo_inicial.mmd` revisado ou substituido pelo seu modelo final.
- implementacao minima em **uma** linguagem:
  - `src_cpp/`, ou
  - `src_python/`
- `AI_LOG.md` preenchido quando houver uso de IA.
- `pull request` final com evidencias.

---

## 3. Estrutura do repositorio

- `docs/requisito_laboratorio.md`: enunciado base do problema.
- `docs/modelo_inicial.mmd`: ponto de partida para o diagrama.
- `docs/diagrama_classe.md`: arquivo principal da sua entrega.
- `src_cpp/`: trilha de implementacao em `C++`.
- `src_python/`: trilha de implementacao em `Python`.
- `AI_LOG.md`: rastreabilidade de uso de IA.

### Regra importante

Escolha apenas **uma** trilha de implementacao:

- `src_cpp/`
- `src_python/`

Voce **nao** precisa entregar as duas linguagens.

---

## 4. Cards de issue

| Card | Foco | Evidencia |
|---|---|---|
| Issue 1 - Fechar diagrama UML | classes, relacoes e cardinalidade | `docs/diagrama_classe.md` atualizado |
| Issue 2 - Validar no Mermaid Live | sintaxe e renderizacao do diagrama | link ou print |
| Issue 3 - Implementar 2 classes | traducao do modelo para `C++` ou `Python` | execucao local |
| Issue 4 - Documentar e rastrear | evidencias e `AI_LOG.md` | PR final |

---

## 5. Como trabalhar

1. Leia `docs/requisito_laboratorio.md`.
2. Use `docs/modelo_inicial.mmd` apenas como ponto de partida.
3. Feche seu diagrama final em `docs/diagrama_classe.md`.
4. Escolha uma linguagem e crie os arquivos necessarios em `src_cpp/` ou `src_python/`.
5. Registre evidencias no `pull request`.

### O que implementar

Implemente pelo menos estas classes:

- `Equipamento`
- `SensorTemperatura`

Se quiser ampliar o modelo, voce pode acrescentar outras classes do dominio.

---

## 6. Como executar

Depois de criar seus arquivos na trilha escolhida:

### Opcao C++

```bash
g++ -std=c++17 -Wall -Wextra -O2 src_cpp/main.cpp src_cpp/equipamento.cpp src_cpp/sensor_temperatura.cpp -o laboratorio
./laboratorio
```

### Opcao Python

```bash
python3 src_python/main.py
```

---

## 7. Criterios de aceite

- O diagrama final atende ao requisito do laboratorio.
- O diagrama foi validado no Mermaid Live ou em ferramenta equivalente.
- Ha justificativa para as principais relacoes e cardinalidades.
- Pelo menos duas classes foram implementadas em uma linguagem.
- O `AI_LOG.md` esta preenchido quando houve uso de IA.
- O `pull request` final apresenta evidencias tecnicas.

### Minimo esperado no diagrama

- pelo menos `5` classes;
- pelo menos `1` generalizacao ou realizacao;
- pelo menos `1` composicao ou agregacao;
- cardinalidade em pelo menos `3` relacoes;
- pelo menos `2` atributos e `1` operacao nas classes principais.

---

## 8. Politica de IA

IA pode ser usada como apoio, mas a solucao precisa ser entendida.

`AI_LOG.md` deve registrar:

- o que foi pedido ao agente;
- o que foi aceito;
- o que foi rejeitado;
- a justificativa tecnica do aluno.

---

## 9. Mini-caso pratico

Uma equipe precisa modelar digitalmente um laboratorio de ensaios. Antes de codificar o sistema, ela fecha um diagrama UML, decide as relacoes entre equipamentos, sensores e ordens, e so depois implementa duas classes para validar a modelagem.

---

## 10. Perguntas de revisao rapida

1. Por que o diagrama precisa vir antes da implementacao?
2. O que a cardinalidade revela sobre o dominio?
3. Por que a entrega deve escolher apenas uma trilha de linguagem?

---

## 11. Referencias

- https://mermaid.live/
- https://mermaid.js.org/syntax/classDiagram.html
- https://docs.github.com/en/pull-requests
- https://docs.github.com/en/education/manage-coursework-with-github-classroom
- https://en.cppreference.com/w/cpp/language/classes
- https://docs.python.org/3/tutorial/classes.html
