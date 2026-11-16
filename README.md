# Stretto Fuga — Calculadora de Intervalos

Ferramenta para explorar a criação de **texturas polifônicas imitativas**
(stretto, cânone, fuga): a partir de uma proposta (sujeito), calcula em quais
intervalos e com quais atrasos ela pode ser imitada por até 5 vozes, mostra o
resultado em partitura e permite ouvi-lo com piano.

### ▶ [Abrir a calculadora no navegador](https://rogerioconstante.github.io/stretto-fuga/)

Funciona em qualquer navegador moderno, sem instalação.

## Funcionalidades

- **Experimentação:** entrada da proposta pelo teclado virtual, com ritmo
  (pontos, quiálteras), transposição, inversão e retrógrado.
- **Análise de imitações:** busca as combinações viáveis de intervalo e atraso
  para 1 a 5 imitações, com três critérios de verificação:
  - Modo A — consonância estrita;
  - Modo B — dissonâncias tratadas;
  - Modo C — consonância nos ataques simultâneos.
- **Contextos:** tonal, modal/escalar e atonal; movimentos diatônicos ou
  cromáticos.
- **Filtros** por ritmo, intervalo e outros critérios, com navegação entre os
  resultados.
- **Partitura** de todas as vozes (VexFlow) e **reprodução** com piano real
  (Tone.js), com controle de andamento.
- **Presets:** salvar e carregar configurações em arquivos `.json`.
- Tabela de referência de intervalos.

## Usar no próprio computador (sem internet)

1. Baixe o repositório: **Code ▸ Download ZIP** e descompacte.
2. Abra o `index.html` no navegador. A calculadora funciona, mas o **piano**
   só toca se a página for servida por HTTP (o navegador bloqueia o
   carregamento das amostras de áudio em arquivos abertos diretamente).
3. Para ter o piano, rode um servidor local na pasta:
   - **Linux/macOS:** `./iniciar-servidor.sh` (abre o navegador sozinho;
     `./parar-servidor.sh` encerra);
   - **qualquer sistema com Python 3:** `python3 -m http.server 8000` e abra
     <http://localhost:8000/>.

## Créditos e licenças

Código da calculadora: © Rogério Tavares Constante, licença
[GPL-3.0](LICENSE). Bibliotecas e amostras de terceiros: ver
[CREDITOS.md](CREDITOS.md).

## Veja também

Plugins de contraponto para MuseScore:
[Analisador de Contrapontos](https://github.com/rogerioConstante/analisador-de-contrapontos),
[Intervalos](https://github.com/rogerioConstante/intervalos-contraponto),
[Classe de Intervalos](https://github.com/rogerioConstante/classe-de-intervalos-contraponto)
e [Bathe's Table](https://github.com/rogerioConstante/bathe-table-plugin).

## Autor

Rogério Tavares Constante. Desenvolvido no âmbito do projeto
*Harmonia e Contraponto*.

Sugestões e relatos de problemas são bem-vindos na aba **Issues**.
