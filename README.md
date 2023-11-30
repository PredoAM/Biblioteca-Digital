# Biblioteca Digital

Este é um aplicativo simples de leitura de eBooks desenvolvido em Dart/Flutter para oferecer uma experiência interativa e fácil de usar aos usuários.

## Funcionalidades

### Baixar Lista de Livros e Capas

O aplicativo acessa uma API para baixar uma lista atualizada de livros e suas respectivas capas.

### Estante de Livros

Exibe as capas dos livros baixados de forma organizada em uma estante virtual.

### Download e Armazenamento de Livros

Permite que o usuário baixe um livro ao tocar em sua capa e salve o arquivo no dispositivo.

### Exibição de Livros

Utiliza o plugin Vocsy Epub Viewer para exibir o conteúdo do livro.

### Navegação de Interface

Inclui um botão para que o usuário possa retornar facilmente à estante de livros durante a leitura.

### Favoritos (Feature Bônus)

- Cria uma aba de favoritos acima do app.
- Ao tocar em Favoritos, são exibidos apenas os livros favoritos.
- Para favoritar um livro, na estante inicial, o usuário toca no marcador no canto superior direito. Essa informação é persistida para quando o usuário voltar para o app.
- Em um livro favorito, o marcador aparece em vermelho. Se tocar no marcador já acionado, ele apaga e o livro é removido da lista de favoritos.

## Requisitos Técnicos

O teste foi realizado usando Dart/Flutter na versão 3.16 ou superior.

## Estrutura do Projeto

```markdown
- lib
  - models
    - book.dart
    - epub_document.dart
  - services
    - book_service.dart
    - epub_reader.dart
  - controllers
    - epub_controller.dart
  - screens
    - bookshelf_screen.dart
    - book_details_screen.dart
  - widgets
    - book_cover.dart
    - favorites_button.dart
    - epub_viewer.dart
  - main.dart
```

## Como Executar o Projeto

1. Clone o repositório para o seu ambiente local.
2. Certifique-se de ter o Flutter instalado.
3. Execute `flutter pub get` para instalar as dependências.
4. Execute `flutter run` para iniciar o aplicativo.
