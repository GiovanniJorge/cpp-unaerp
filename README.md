# C++ - Unaerp

Exercícios em linguagem C++ usados nas aulas da Unaerp — coleção organizada por tópicos (programação orientada a objetos, templates, manipulação de arquivos, strings, funções e exercícios gerais). Ideal para estudantes que querem aprimorar suas habilidades em C++ moderno.

## Conteúdo principal

- Exercícios focados em problemas didáticos para aprendizagem de C++.
- Estrutura simples por pastas que separa exercícios por tema.
- Exemplos que demonstram conceitos fundamentais e avançados de C++.
- Uso de boas práticas e padrões de codificação modernos.

## Badges

- Licença: MIT (ver arquivo LICENSE)
- Linguagem: C++

## Sumário

- [Visão geral](#visão-geral)
- [Estrutura do repositório](#estrutura-do-repositório)
- [Como compilar e executar](#como-compilar-e-executar)
- [Boas práticas / recomendações de compilação](#boas-práticas--recomendações-de-compilação)
- [Contribuindo](#contribuindo)
- [Licença](#licença)
- [Autor / Contato](#autor--contato)

## Visão geral

Este repositório organiza pequenos programas em C++ que exemplificam conceitos de linguagem e resolução de problemas. Cada arquivo fonte normalmente resolve um exercício específico e está escrito para fins educacionais, focando em clareza e aprendizado.

Os exercícios cobrem desde conceitos básicos até tópicos mais avançados, como programação orientada a objetos, manipulação de memória e uso de estruturas de dados.

## Estrutura do repositório

Top-level:
- `.gitattributes`
- `LICENSE`
- `README.md`
- `exercicios-geral/`         — exercícios diversos e fundamentos (`geral-ex1.cpp`, `geral-ex2.cpp`, etc.)

Como se encaixa:
- Cada arquivo `.cpp` é um programa independente (exercício). A forma usual de usar o repositório é compilar o arquivo que você quer executar.
- Arquivos podem incluir headers (`.h` ou `.hpp`) quando necessário.
- Alguns exercícios podem incluir arquivos de dados de exemplo para fins didáticos.

## Como compilar e executar

Recomenda-se usar `g++` ou `clang++` (compiladores compatíveis com C++). Exemplos:

Compilar um exercício único:
```bash
g++ -std=c++17 -Wall -Wextra -pedantic -O2 -g exercicios-geral/geral-ex1.cpp -o geral-ex1
./geral-ex1
```

Compilar com suporte a C++20 (se disponível):
```bash
g++ -std=c++20 -Wall -Wextra -pedantic exercicios-geral/geral-ex3.cpp -o geral-ex3
./geral-ex3
```

Compilar todos os `.cpp` em uma pasta (rápido para testes):
```bash
# dentro da pasta correspondente
g++ -std=c++17 -Wall -Wextra *.cpp -o exercicios
./exercicios
```

Usando clang++ (alternativa):
```bash
clang++ -std=c++17 -Wall -Wextra -pedantic geral-ex1.cpp -o geral-ex1
./geral-ex1
```

## Boas práticas / recomendações de compilação

- Use: `-std=c++17 -Wall -Wextra -pedantic` para detectar avisos e manter portabilidade (C++17 é um bom padrão; considere C++20 para projetos mais modernos).
- Para depuração ativa: adicione `-g` e compile sem `-O2`.
- Para versão final de performance: adicione `-O2` ou `-O3`.
- Documente cada exercício no topo do arquivo (comentário explicando entrada esperada, saída, objetivos de aprendizado e algoritmo).
- Prefira nomes de arquivos sem espaços/acentos para compatibilidade entre sistemas operacionais.
- Evite usar `using namespace std;` em arquivos de exemplo; prefira `std::` explícito para fins educacionais.
- Considere usar `-Wshadow` e `-Wconversion` para detectar problemas mais sutis.

## Contribuindo

Contribuições são bem-vindas (ex.: correções, comentários, novos exercícios, testes). Fluxo sugerido:

1. Fork do repositório.
2. Criar branch com nome descritivo: `feature/exercicio-nome` ou `fix/readme`.
3. Fazer commits atômicos com mensagens claras.
4. Abrir Pull Request descrevendo as mudanças e, se aplicável, o motivo pedagógico.
5. Se possível, inclua casos de teste ou instruções para validar o exercício.

Sugestões adicionais:

- Adicione um pequeno README por pasta explicando o objetivo dos exercícios daquela pasta.
- Considere adicionar um `Makefile` com targets como `make all`, `make clean`, `make exercicio=exemplo`.
- Mantenha consistência com o padrão de nomenclatura dos arquivos.

## Testes e automação (opcional)

- Poderia ser adicionado um `Makefile` para facilitar compilação em lote.
- Para verificação automática, adicionar um workflow (GitHub Actions) que compila cada `.cpp` para garantir que o repositório permaneça compilável.
- Exemplo de workflow: compilar com diferentes flags (`-std=c++17`, `-std=c++20`, etc.) para garantir compatibilidade.

## Licença

Este repositório utiliza a licença MIT — consulte o arquivo `LICENSE` na raiz.

## Autor / Contato

Autor: Giovanni Jorge  
Repositório: https://github.com/GiovanniJorge/cpp-unaerp
