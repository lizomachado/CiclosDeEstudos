# Ciclos de Estudos

Aplicativo desktop desenvolvido em Java para organizar um ciclo de estudos de forma prática. As disciplinas são organizadas em uma fila rotativa, permitindo manter uma rotina equilibrada sem a necessidade de reorganizar a lista manualmente após cada sessão.

## Funcionalidades

- Organização das disciplinas em fila rotativa.
- Ao concluir uma matéria, ela é movida automaticamente para o final da lista.
- Destaque visual para a última disciplina estudada.
- Campo de anotações individual para cada disciplina.
- Salvamento automático das disciplinas e das observações.
- Interface gráfica desenvolvida com Java Swing.

## Estrutura dos arquivos

O programa utiliza os seguintes arquivos para armazenar os dados:

```
disciplinas.txt
observacoes/
```

- `disciplinas.txt`: armazena a lista de disciplinas.
- `observacoes/`: contém um arquivo de anotações para cada disciplina.

Todos os dados são preservados entre as execuções do aplicativo.

## Requisitos

- Java 17 ou superior (JRE ou JDK).

Para verificar a versão instalada:

```bash
java -version
```

## Executando o aplicativo

### Windows

Basta executar o arquivo:

```
Ciclo de Estudos.jar
```

Caso o sistema solicite um programa para abrir o arquivo, selecione o Java.

### macOS

Também é possível executar o arquivo `.jar` com um duplo clique, desde que o Java esteja instalado. Se necessário, utilize o Terminal:

```bash
java -jar "Ciclo de Estudos.jar"
```

### Linux

Em algumas distribuições Linux, arquivos `.jar` são associados ao gerenciador de arquivos compactados. Se isso acontecer, execute o aplicativo pelo Terminal:

```bash
java -jar "Ciclo de Estudos.jar"
```

Caso queira que o duplo clique funcione normalmente, crie uma associação para arquivos `.jar`:

```bash
cat <<EOF > ~/.local/share/applications/java.desktop
[Desktop Entry]
Name=Abrir com Java
Exec=java -jar %f
Type=Application
Terminal=false
MimeType=application/x-java-archive;application/java-archive;application/x-jar;
EOF
```

Depois atualize o banco de aplicações:

```bash
update-desktop-database ~/.local/share/applications/
```

Em seguida:

1. Clique com o botão direito no arquivo `.jar`.
2. Selecione **Propriedades** → **Abrir com**.
3. Escolha **Abrir com Java**.
4. Marque a opção para utilizar esse programa como padrão.

## Tecnologias

- Java
- Java Swing

## Persistência dos dados

As alterações são gravadas automaticamente durante o uso do aplicativo. Não é necessário salvar manualmente antes de fechar a janela.

## Licença

Este projeto é disponibilizado para uso pessoal e acadêmico.
