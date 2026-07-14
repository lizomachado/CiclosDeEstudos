# 📚 Meus Ciclos de Estudos

Aplicação desktop desenvolvida em Java para auxiliar na organização dos estudos utilizando o método de ciclos. O projeto surgiu da necessidade de organizar diferentes assuntos de forma simples, mantendo o foco no estudo sem precisar reorganizar listas ou cronogramas manualmente.

## Funcionalidades

- Gerenciamento de múltiplos ciclos de estudos.
- Fila rotativa para reorganização automática das disciplinas.
- Anotações individuais para cada matéria.
- Salvamento automático das alterações.
- Histórico de edição (`Ctrl + Z`) nas anotações.
- Controle de zoom para aumentar ou reduzir o tamanho da fonte.
- Alternância entre tema claro e escuro.
- Exportação das anotações para arquivo `.txt`.
- Armazenamento dos dados em uma pasta dedicada do usuário.

## Armazenamento dos dados

Os dados são armazenados em uma pasta oculta no diretório do usuário, evitando que sejam perdidos caso a pasta do projeto seja movida ou excluída.

### Localização

**Windows**

```
C:\Users\SeuUsuario\.ciclos_estudos\
```

**Linux**

```
/home/seuusuario/.ciclos_estudos/
```

**macOS**

```
/Users/seuusuario/.ciclos_estudos/
```

### Arquivos gerados

```
ciclo_[NomeDoCiclo].txt
obs_[NomeDoCiclo]_[Letra]_[Materia].txt
```

- `ciclo_...`: informações do ciclo e ordem das disciplinas.
- `obs_...`: anotações de cada disciplina.

## Requisitos

- Java 17 ou superior.

Verifique a versão instalada:

```bash
java -version
```

## Executando

### Windows

Execute o arquivo:

```
Ciclos de Estudos.jar
```

Caso seja solicitado um programa, selecione o Java.

### macOS

Também é possível executar pelo Terminal:

```bash
java -jar "Ciclos de Estudos.jar"
```

### Linux

Caso o sistema tente abrir o `.jar` como arquivo compactado:

```bash
java -jar "Ciclos de Estudos.jar"
```

Para associar arquivos `.jar` ao Java:

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

Atualize o banco de aplicações:

```bash
update-desktop-database ~/.local/share/applications/
```

Depois, escolha **Abrir com Java** nas propriedades do arquivo e defina como aplicativo padrão.

## Tecnologias

- Java 17
- Java Swing
- java.io
- JFileChooser

## Objetivo

Este projeto foi desenvolvido para uso pessoal, com o objetivo de facilitar a organização dos meus estudos e, ao mesmo tempo, praticar conceitos de desenvolvimento desktop em Java, como interfaces gráficas, manipulação de arquivos e organização de aplicações.

## Licença

Projeto disponibilizado para fins de estudo e uso pessoal.
