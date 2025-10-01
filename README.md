# 📚 Trabalho Prático 02: Aplicativo de Lista de Tarefas (TarefasApp)

Aplicação móvel de gerenciamento de tarefas desenvolvida em **.NET MAUI** para cumprir os requisitos do Trabalho Prático 02. O objetivo foi implementar a navegação hierárquica e modal, a passagem de dados entre páginas e um CRUD (Criação, Leitura, Atualização e Exclusão) básico para gerenciamento de tarefas.

---
## ✨ Teste

![Teste Funcioanndo](./video.gif)

---

## ✨ Funcionalidades e Requisitos Implementados

| Funcionalidade | Requisito TP-02 | Implementação |
| :--- | :--- | :--- |
| **Lista Inicial (Home)** | Exibir lista com título e descrição. | Utiliza `CollectionView` (ou `ListView`) para exibir o **Título** e **Descrição** em um layout de cartão moderno e responsivo. |
| **Adicionar Tarefa** | Implementar modal para adição de nova tarefa. | O botão "Adicionar Tarefa" abre a `AddPage` como um **modal** (`PushModalAsync`), permitindo a inserção de Título, Descrição, Data e Prioridade. |
| **Navegação Hierárquica** | Ao clicar em um item, navegar para a página de detalhes. | O botão "Detalhes" em cada item da lista usa **navegação hierárquica** (`PushAsync`) para abrir a `DetailsPage`. |
| **Visualização de Detalhes** | Página que exibe data de criação e prioridade. | A `DetailsPage` centraliza e exibe todos os dados (Data de Criação, Prioridade, Título, Descrição) em um **layout de cartão** responsivo. |
| **Edição (Modal)** | Botão "Editar" que abre um modal para alterações. | O botão "Editar" na `DetailsPage` abre a `EditPage` como um **modal** (`PushModalAsync`) pré-preenchido com os dados da tarefa. |
| **Exclusão** | Botão "Excluir" com diálogo de confirmação. | O botão "Excluir" na `DetailsPage` exibe um **`DisplayAlert`** para confirmação antes de remover o item do repositório. |

---

## 🎨 Melhorias de Design

O design foi unificado para ter uma aparência coesa e profissional:

* **Tema Verde e Branco:** Utiliza o fundo verde claro (`#f3fcf2`) e o verde escuro (`#38761d`) como cor primária para botões e títulos.
* **Layout de Cartão:** As páginas de formulário (`DetailsPage`, `EditPage`, `AddPage`) usam uma estrutura de **`Border`** centralizado para criar um visual de "cartão flutuante".
* **Rodapé Fixo:** Os créditos são exibidos em um **rodapé colorido e fixo** na parte inferior da tela, usando `AbsoluteLayout`.
* **Tratamento de Lista Vazia:** Exibe uma mensagem amigável (`Label`) quando não há tarefas cadastradas.

---

## 📁 Estrutura do Projeto

* `MainPage.xaml`: Exibe a lista principal e trata a navegação.
* `Pages/AddPage.xaml`: Modal para criação de novas tarefas.
* `Pages/EditPage.xaml`: Modal para edição de tarefas existentes.
* `Pages/DetailsPage.xaml`: Exibe informações completas da tarefa e botões de ação.
* `Models/TaskModel.cs`: Classe para representação dos dados da tarefa.
* `Repository/TaskRepository.cs`: Gerencia a lista de tarefas.

---


## ✒️ Autores

| Desenvolvedor | RA / CB |
| :--- | :--- |
| **Laysa Bernardes** | **CB3024873** |
| **Lucas Lopes** | **CB3025284** |
