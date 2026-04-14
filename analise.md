Parte 1
1. Objetivo do sistema

O sistema tem como objetivo permitir que clientes façam pedidos online de Tropykaly Pizzas e Lanches, facilitando:

Visualização de produtos
Montagem de pedidos
Finalização de compra


2. Funcionalidades

Com base na navegação típica desse tipo de sistema:

Listagem de produtos (pizzas, lanches, bebidas)
Visualização de detalhes do produto
Adição ao carrinho
Seleção de opções (tamanho, sabores, adicionais)
Carrinho de compras
Finalização de pedido (checkout)
Informações de contato/entrega

3. Interação do usuário

Fluxo típico:

Usuário acessa o site
Navega por categorias
Seleciona um produto
Personaliza (ex: tamanho da pizza)
Adiciona ao carrinho
Visualiza carrinho
Finaliza pedido

Interface baseada em cliques → modelo web interativo (provavelmente SPA leve ou tradicional).

4. Organização dos produtos

Os produtos estão organizados de forma hierárquica:

Categorias:
Pizzas
Lanches
Bebidas
Subdivisões possíveis:
Tamanhos
Sabores
Combinações

Estrutura típica:

Categoria → Produto → Opções
Parte 2
Tipo de arquitetura

Arquitetura Cliente-Servidor (Web)
Possivelmente com backend + frontend separados

Divisão em camadas (inferida)
1. Camada de Apresentação (Frontend)
Interface do usuário
HTML/CSS/JS
2. Camada de Aplicação (Backend)
Regras de negócio
Processamento de pedidos
3. Camada de Dados
Banco de dados (produtos, pedidos, clientes)
Separação de responsabilidades

Existe uma separação básica:

Frontend → exibição e interação
Backend → lógica
Banco → persistência

Porém, pode haver mistura de responsabilidades, comum em sistemas pequenos.

Parte 3 – Análise de Design
Coesão
Moderada a alta
Cada parte parece ter uma função específica (produtos, carrinho, pedido)

Pontos positivos:

Telas organizadas por função
Acoplamento
Provavelmente médio
Interface depende diretamente da estrutura do backend

Possível problema:

Mudanças no backend podem quebrar frontend
Separação de responsabilidades
Parcialmente presente
Mas pode não ser bem estruturada internamente (sem código não dá pra garantir)
