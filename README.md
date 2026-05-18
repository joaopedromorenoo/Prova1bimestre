# Sistema de Gerenciamento Imobiliário

Sistema de gerenciamento de contratos de aluguel desenvolvido em Java, com cadastro de inquilinos, imóveis e contratos,
além de controle de status (ativo/encerrado).

---

## Funcionalidades

- Cadastrar inquilinos com nome, CPF e telefone
- Cadastrar imóveis do tipo **Casa** ou **Apartamento**
- Registrar contratos de aluguel vinculando inquilino e imóvel
- Encerrar contratos ativos
- Listar contratos ativos com valor total calculado automaticamente
- Menu interativo via terminal

--------------------------------------------------------------------------------------------------------

## Estrutura do Projeto

```
├── Imovel.java          # Classe base (herança)
├── Casa.java            # Subclasse de Imovel (com quintal)
├── Apartamento.java     # Subclasse de Imovel (com andar)
├── Inquilino.java       # Dados do inquilino
├── Contrato.java        # Relaciona inquilino + imóvel + período
├── Imobiliaria.java     # Gerencia lista de contratos
└── Main.java            # Ponto de entrada + menu interativo
```

--------------------------------------------------------------------------------------------------------

## Conceitos Aplicados

- **Herança** — `Casa` e `Apartamento` estendem `Imovel`
- **Polimorfismo** — método `mostrarImovel()` sobrescrito em cada subclasse
- **Encapsulamento** — atributos privados com getters e setters
- **ArrayList** — armazenamento dinâmico de inquilinos, imóveis e contratos
- **Scanner** — entrada de dados via terminal

--------------------------------------------------------------------------------------------------------

## Como Executar

### Pré-requisitos

- Java JDK 11 ou superior
- VS Code com a extensão [Extension Pack for Java](https://marketplace.visualstudio.com/items?itemName=vscjava.vscode-java-pack)

### Passos

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/sistema-imobiliario.git
   cd sistema-imobiliario
   ```

2. Abra a pasta no VS Code:
   ```bash
   code .
   ```

3. Execute o arquivo `Main.java` pelo botão **Run** do VS Code ou via terminal:
   ```bash
   javac *.java
   java Main
   ```

--------------------------------------------------------------------------------------------------------

## Demonstração

Ao iniciar, o sistema carrega dois contratos de exemplo:

```
=== DEMONSTRAÇÃO INICIAL ===
Contratos: João (encerrado) e Maria (ativo).

--- Lista de Contratos Ativos ---
Contrato #2 |
-------------------------------
Inquilino | Nome: Maria Oliveira | CPF: 987.654.321-00 | Telefone: (21) 91234-5678
Apartamento | Endereço: Avenida Central, 456 | Valor do Aluguel: R$ 1200,00 | Andar: 5
Período: 01/03/2025 até 28/02/2026 | Meses: 12
Valor Total: R$ 14400,00 | Situação: Ativo
-------------------------------
```

--------------------------------------------------------------------------------------------------------

## Tecnologias

![Java](https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white)

--------------------------------------------------------------------------------------------------------

## Autor

Desenvolvido como projeto acadêmico na faculdade de Engenharia de Software.
