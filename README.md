# Element Card War Project

## Table of Contents

1. [Introduction](#introduction)
2. [System Requirements](#system-requirements)
3. [Installation and Execution](#installation-and-execution)
4. [Project Structure](#project-structure)
5. [DSL Usage](#dsl-usage)

## Introduction

This project has been developed with an educational focus for Computer Science students, aiming to model the compilation process. The project uses .NET 7 and simulates a compilation process through the interpretation of an abstract syntax tree (AST). The project's "skin" is a card game representing an Element Card War.

## System Requirements

- [.NET SDK 7.0](https://dotnet.microsoft.com/en-us/download/dotnet/7.0) or higher.

## Installation and Execution

1. Clone the repository:

```
git clone https://github.com/RodrigoGarcia43/elemental_wars.git
```

2. Navigate to the project folder:

```
cd elemental_wars
```

3. Restore the dependencies:

```
dotnet restore
```

4. Run the project:

```
dotnet run
```

## Project Structure

- `examples/`: Within this folder, you will find detailed examples of how to define valid cards and elements for our language.
- `assets/`: For a detailed visualization of the AST node hierarchy, check the images inside this folder.

## DSL Usage

The game consists of cards representing elements. Each element has a set of elements it is weak to and another set it is strong against. When a card is played, it can damage the opponent.

### Card Definition:

- **Elements**: Set of elements associated with the card.
- **Power**: Direct numeric value or result of an arithmetic operation (`+`, `-`, `*`, `/`).

For instance, a card might have the Water element and a power of `5 + 3`. If the Water element is strong against Fire, then the damage factor of cards with Water increases by 1 when facing cards with Fire. After calculating this factor for each pair of Elements in a pair of cards, this number is multiplied by a constant and added to the card's power.
#   E l e m e n t a l _ w a r s - m a i n - P R O - 2 0 2 3  
 