# 🛒 Lista de Compras

Um aplicativo mobile simples e intuitivo para gerenciamento de listas de compras, desenvolvido com **React Native**, **Expo** e **TypeScript**.

## 🚀 Conceitos Aplicados

* **useState (Gerenciamento de Estado):** Manipulação dinâmica da lista de itens, adição de produtos, remoção individual por ID e controle dos campos de entrada do formulário.

* **TypeScript e Tipagem Estática:** Criação da interface compartilhada `ItemDeCompra` (`id`, `nome`, `quantidade`) e tipagem rigorosa de `props` em todos os componentes para prevenir erros em tempo de compilação.

* **Componentização e Passagem de Props:** Organização modular da aplicação em componentes reutilizáveis (`Cabecalho`, `FormularioItem`, `ListaCompras` e `ItemCompra`), utilizando funções de callback (`aoAdicionar`, `aoRemover`) para comunicação entre componentes filho e pai.

* **Formulários Controlados e Validação:** Captura dos dados em tempo real no `TextInput`, validação contra envio de campos vazios através de `Alert.alert` e conversão de texto para número com fallback padrão (`parseInt`).

* **Renderização Otimizada com FlatList:** Utilização do componente nativo `FlatList` com `keyExtractor`, renderização condicional para lista vazia (`ListEmptyComponent`), cabeçalhos e espaçadores de rodapé.

* **Estilização Nativa com StyleSheet:** Layouts e componentes estilizados de forma escopada utilizando `StyleSheet.create`, aplicando Flexbox e tratamento de sombras para iOS e Android.

## 📦 Observação sobre a pasta `node_modules`

A pasta `node_modules` não é enviada ao GitHub por boas práticas de desenvolvimento (por ser uma pasta pesada de arquivos gerados).

Todas as dependências e bibliotecas necessárias para o funcionamento do projeto estão registradas no arquivo `package.json`. O comando `npm install` lê esse arquivo e baixa automaticamente a pasta `node_modules` atualizada para a sua máquina.

## 🛠️ Como Baixar e Executar o Projeto

Siga os passos abaixo para testar o aplicativo no seu computador ou dispositivo móvel:

1. **Baixe o projeto:**

   * Clique no botão verde **Code** no topo desta página e escolha **Download ZIP** (ou faça o clone do repositório com o Git).

   * Extraia o arquivo `.zip` em uma pasta de sua preferência.

2. **Abra o terminal na pasta do projeto:**

   * Abra a pasta no VS Code e abra o terminal integrado (`Ctrl + '` ou `Ctrl + J`).

3. **Instale as dependências (recria a pasta `node_modules`):**

   ```
   npm install
   
   ```

4. **Execute o projeto com o comando:**

   ```
   npm start
   
   ```

5. **Abra o aplicativo:**

   * **Dispositivo Físico:** Escaneie o QR Code exibido no terminal utilizando o aplicativo **Expo Go** (Android/iOS).

   * **Emulador Android:** Pressione a tecla `a` no terminal com o emulador aberto.

   * **Navegador Web:** Pressione a tecla `w` no terminal.
