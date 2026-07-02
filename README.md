# C++ - Unaerp

Exercícios em linguagem C++ usados nas aulas da Unaerp — coleção organizada por tópicos (programação orientada a objetos, templates, manipulação de arquivos, strings, funções e exercícios gerais). Ideal para estudantes que querem aprimorar suas habilidades em C++ moderno.

## Conteúdo principal
- Exercícios focados em problemas didáticos para aprendizagem de C++.
- Estrutura simples por pastas que separa exercícios por tema.
- Exemplos que demonstram conceitos fundamentais e avançados de C++.
- Uso de boas práticas e padrões de codificação modernos.

## Badges
![Licença](https://img.shields.io/github/license/GiovanniJorge/cpp-unaerp?style=flat-square)
![Exercícios](https://img.shields.io/badge/quantidade-19%20exercícios-blue?style=flat-square)

## Sumário
- [Visão geral](#visão-geral)
- [Estrutura do repositório](#estrutura-do-repositório)
- [Como compilar e executar](#como-compilar-e-executar)
- [Contribuindo](#contribuindo)
- [Licença](#licença)
- [Autor / Contato](#autor--contato)

## Visão geral
Este repositório organiza pequenos programas em C++ que exemplificam conceitos de linguagem e resolução de problemas. Cada arquivo fonte normalmente resolve um exercício específico e está escrito para fins educacionais, focando em clareza, boas práticas pedagógicas e aprendizado de C++ moderno.

## Estrutura do repositório
Top-level:
```text
├── .gitattributes
├── LICENSE
├── README.md
├── desktop.ini
└── exercicios-geral/         # Exercícios diversos e fundamentos (.cpp, .hpp, etc.)
    ├── elipse.cpp
    ├── aprovacao-aluno.cpp
    └── ...                  # Outros subprojetos e tópicos divididos por temas
```

### Como se encaixa:
- O repositório abriga uma variedade de exercícios independentes criados ao longo do curso.
- Cada arquivo `.cpp` é um programa autônomo. A forma usual de usar o repositório é navegar até o diretório correspondente e compilar o arquivo específico que você deseja estudar ou executar.

## Como compilar e executar

Recomenda-se usar `g++` ou `clang++` (compiladores compatíveis com os padrões modernos de C++). Exemplos:

### Compilar um exercício único (Padrão C++17):
```bash
g++ -std=c++17 -Wall -Wextra -pedantic -O2 -g exercicios-geral/elipse.cpp -o elipse
./elipse
```

### Compilar com suporte a C++20:
```bash
g++ -std=c++20 -Wall -Wextra -pedantic exercicios-geral/aprovacao-aluno.cpp -o aprovacao-aluno
./aprovacao-aluno
```

### Compilar todos os .cpp em uma pasta (Rápido para testes locais):
```bash
# Dentro da pasta correspondente
g++ -std=c++17 -Wall -Wextra *.cpp -o exercicios
./exercicios
```

### Usando Clang++ como alternativa:
```bash
clang++ -std=c++17 -Wall -Wextra -pedantic exercicios-geral/elipse.cpp -o elipse
./elipse
```

> **Dica de Compilação:** As flags `-Wall -Wextra -pedantic` são altamente recomendadas no ambiente universitário pois forçam o compilador a apontar avisos estritos e desvios de padrões ISO. Para depuração com ferramentas como GDB, mantenha a flag `-g` ativa.

## Contribuindo
Contribuições são bem-vistas! Se deseja adicionar uma nova resolução de exercício ou propor melhorias nas estruturas de templates e POO, siga os passos abaixo:

1. Faça um **Fork** do repositório.
2. Crie uma branch com nome descritivo: `feature/exercicio-nome` ou `fix/readme`.
3. Faça commits atômicos com mensagens claras e objetivas.
4. Abra um **Pull Request** detalhando as alterações implementadas e seu contexto didático.

## Licença
Este repositório utiliza a licença MIT — consulte o arquivo [LICENSE](LICENSE) na raiz.

## Autor / Contato
- **Autor:** Giovanni Jorge  
- **Repositório:** [https://github.com/GiovanniJorge/cpp-unaerp](https://github.com/GiovanniJorge/cpp-unaerp)
