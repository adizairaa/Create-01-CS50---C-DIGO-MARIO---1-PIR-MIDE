# Desafio Mario - Pirâmide de Blocos

🌐 **Algoritmo para Gerar a Pirâmide do Mario**

Este repositório contém a solução para o problema de gerar uma pirâmide de blocos no estilo do **Mundo 1-1** do **Super Mario Brothers**. A implementação é feita em C e permite que o usuário escolha a altura da pirâmide, que será formada por caracteres de `#` e alinhada à direita.

🧠 **Descrição do Problema**

O objetivo do programa é gerar uma pirâmide de altura variável, onde a base será alinhada à direita. O programa solicita ao usuário que insira um número inteiro entre 1 e 8, que define a altura da pirâmide. A pirâmide será impressa com espaços à esquerda e hashes `#` representando os blocos.

**Regras de Funcionamento:**

- O número de linhas da pirâmide será igual ao número inserido pelo usuário.
- Cada linha da pirâmide terá espaços à esquerda e um número crescente de hashes `#` à direita.
- O programa garante que o número inserido pelo usuário esteja entre 1 e 8; valores fora desse intervalo são rejeitados.
  
Exemplo de entrada e saída:

### Exemplo de Execução:

#### Entrada 1:
```bash
$ ./mario
Altura: 8
       #
      ##
     ###
    ####
   #####
  ######
 #######
########
```

#### Entrada 2:
```bash
$ ./mario
Altura: 4
   #
  ##
 ###
####
```

#### Entrada 3:
```bash
$ ./mario
Altura: 2
 #
##
```

#### Entrada 4:
```bash
$ ./mario
Altura: 1
#
```

#### Entrada 5 (com entradas inválidas):
```bash
$ ./mario
Altura: -1
Altura: 0
Altura: 42
Altura: 9
Altura: 4
   #
  ##
 ###
####
```

⚙️ **Como Funciona o Programa**

O programa executa as seguintes etapas:

1. Solicita ao usuário a altura da pirâmide, garantindo que o número esteja entre 1 e 8.
2. Utiliza dois loops aninhados para:
   - Imprimir os espaços à esquerda.
   - Imprimir os hashes `#` à direita para formar a pirâmide.
3. O programa continua pedindo a altura até que o usuário forneça uma entrada válida.

🚀 **Como Rodar o Programa**

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/mario.git
   ```

2. Navegue até o diretório do projeto:
   ```bash
   cd mario
   ```

3. Compile o código:
   ```bash
   gcc -o mario mario.c
   ```

4. Execute o programa:
   ```bash
   ./mario
   ```

5. Insira a altura desejada para a pirâmide quando solicitado.

✅ **Exemplos de Entrada e Saída**

### Exemplo 1:
```bash
$ ./mario
Altura: 4
   #
  ##
 ###
####
```

### Exemplo 2:
```bash
$ ./mario
Altura: -2
Altura: 6
   #
  ##
 ###
####
#####
######
```

🛠️ **Ferramentas e Testes**

**Bibliotecas Utilizadas:**

- `cs50.h`: Para facilitar a entrada de dados.
- `stdio.h`: Para operações de entrada e saída.
- `math.h`: Não utilizado diretamente, mas pode ser útil para melhorias futuras.

**Testes Manuais:**

- Insira valores negativos, palavras ou pressione Enter sem entrada.
- Teste com valores como 1, 8 ou 0.

**Validação de Estilo:**

```bash
style50 mario.c
```

🌟 **Contribuições**

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests com melhorias ou sugestões.

📜 **Licença**

Este projeto está licenciado sob a MIT License.
