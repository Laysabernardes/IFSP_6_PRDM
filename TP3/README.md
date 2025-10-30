# 📦 TP 3 - Rastreamento Logístico com .NET MAUI e MVVM

## 📝 Descrição do Projeto

Aplicação móvel desenvolvida em .NET MAUI para simular o rastreamento de pacotes de uma empresa de logística. O projeto segue o padrão de arquitetura MVVM (Model-View-ViewModel) para garantir a separação de responsabilidades e facilitar a manutenção e escalabilidade do código.

---

## ▶️ Demonstração

![Teste Funcioanndo](./TP3.gif)

---

## ✨ Destaques da Aplicação

* **Tema:** Interface de usuário moderna com esquema de cores **monocromático em tons de azul**.
* **Padrão:** Implementação rigorosa do padrão **MVVM**.
* **Layout Otimizado:** Uso de `VerticalStackLayout`, `ScrollView` e `HorizontalStackLayout` (na página de resultados) para garantir visibilidade e fluidez.
* **Dados Fictícios:** Os dados de rastreamento foram modificados para evitar duplicidade com o projeto original.

---

## 🛠️ Requisitos e Estrutura Técnica

| Componente | Tipo/Função | Descrição |
| :--- | :--- | :--- |
| **`PacoteModel.cs`** | Modelo (Model) | Define a estrutura de dados (ID, Status, Datas, Histórico). |
| **`PacoteViewModel.cs`** | Lógica (ViewModel) | Gerencia a lógica de rastreamento e contém os dados fictícios atualizados. |
| **`MainPage.xaml`** | Visualização (View) | Página inicial com campo de entrada, botão "Rastrear", **título** e **rodapé fixo** de autoria. |
| **`ResultadosPage.xaml`** | Visualização (View) | Exibe os detalhes e histórico do pacote em **layouts empilhados** para evitar problemas de sobreposição. |
| **`Styles.xaml`** | Estilos XAML | Contém estilos globais e definições de cores (`AzulPrincipal`, `TextoAzulMarinho`, etc.) que implementam o tema azul monocromático. |

---
## ✒️ Autores

| Desenvolvedor | CB |
| :--- | :--- |
| **Laysa Bernardes** | **CB3024873** |
| **Lucas Lopes** | **CB3025284** |






## 🚀 Como Executar

1.  Clone este repositório para sua máquina local.
2.  Abra a solução no **Visual Studio 2022** (com workloads .NET MAUI instaladas).
3.  Execute a aplicação no emulador ou dispositivo desejado.
4.  **Códigos de Rastreamento para Teste:**
    * **`BR420BRL`** (Entregue)
    * **`SP999BRX`** (Aguardando Retirada)
    * **`MG111ABC`** (Em Trânsito)