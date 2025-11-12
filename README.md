# 📘 Manual do Usuário – Sistema Acadêmico (.TXT)

## 🎯 Visão Geral  
Este sistema foi desenvolvido em **C** com o objetivo de **gerenciar cadastros de alunos e turmas**, além de permitir o **vínculo entre eles** e o **registro das notas (NP1, NP2 e PIM)**.  
Todas as informações são armazenadas em **arquivos `.txt`**, tornando o uso simples e acessível.

O sistema oferece:
- Cadastro e listagem de alunos  
- Cadastro e listagem de turmas  
- Vínculo entre alunos e turmas  
- Inserção de exemplos automáticos  
- Gravação automática dos dados em arquivos de texto  

---

## 🖥️ Execução do Programa  

### Requisitos:
- Compilador **C** (ex: GCC)
- Sistema operacional com terminal (Windows, Linux ou macOS)

### Passos para execução:
```bash
gcc Sistema-C.txt -o sistema
./sistema
```

---

## 🧭 Menu Principal

Ao iniciar o programa, o usuário verá o seguinte menu:

```
=== SISTEMA ACADEMICO (.TXT) ===
1 - Cadastrar aluno
2 - Listar alunos
3 - Cadastrar turma
4 - Listar turmas
5 - Vincular aluno a turma
6 - Listar vinculos aluno->turma
7 - Inserir exemplos
0 - Sair
Escolha:
```

O usuário deve digitar o número correspondente à ação desejada.

---

## 👩‍🎓 Cadastro de Alunos

**Função:** `registerStudent()`

**Descrição:** Permite inserir as informações de um novo aluno.  
As informações são gravadas no arquivo `students.txt`.

**Campos solicitados:**
- Matrícula (número)
- Nome completo
- Nota NP1
- Nota NP2
- Nota PIM

**Saída esperada:**
```
Aluno salvo com sucesso no arquivo students.txt!
```

---

## 📋 Listagem de Alunos

**Função:** `listStudents()`

**Descrição:** Exibe no terminal todos os alunos cadastrados, lendo os dados do arquivo `students.txt`.

Se não houver alunos:
```
Nenhum aluno cadastrado ainda.
```

---

## 🏫 Cadastro de Turmas

**Função:** `registerClass()`

**Descrição:** Registra uma nova turma e grava os dados no arquivo `classes.txt`.

**Campos solicitados:**
- Nome da turma

**Exemplo de saída:**
```
Turma gravada com sucesso (ID 1)
```

---

## 📚 Listagem de Turmas

**Função:** `listClasses()`

**Descrição:** Mostra as turmas cadastradas no arquivo `classes.txt`.

Se não houver turmas:
```
Nenhuma turma cadastrada.
```

---

## 🔗 Vincular Aluno a Turma

**Função:** `linkStudentToClass()`

**Descrição:** Cria uma associação entre um aluno e uma turma.  
Os vínculos são salvos em `links.txt`.

**Campos solicitados:**
- Matrícula do aluno  
- ID da turma  

**Exemplo de saída:**
```
Vinculo gravado com sucesso!
```

---

## 📑 Listar Vínculos

**Função:** `listStudentClassLinks()`

**Descrição:** Exibe as associações entre alunos e turmas gravadas no arquivo `links.txt`.

---

## 🧩 Inserir Exemplos

**Função:** `addSampleStudents()`

**Descrição:** Insere automaticamente dois alunos de exemplo (Flávio e Roberto) para teste do sistema.  
Os registros são adicionados ao arquivo `students.txt`.

---

## 🚪 Encerrando o Programa

Para sair do sistema, selecione a opção:
```
0 - Sair
```

---

## 📂 Estrutura de Arquivos Gerados

| Arquivo         | Descrição |
|-----------------|------------|
| `students.txt`  | Contém os dados dos alunos cadastrados |
| `classes.txt`   | Lista as turmas registradas |
| `links.txt`     | Guarda os vínculos entre alunos e turmas |

---

## 🧰 Dica de Uso
Se o sistema não exibir dados, verifique se os arquivos `.txt` foram criados na mesma pasta do executável.  
Caso contrário, crie-os manualmente (arquivos vazios).

---

```
5. Pronto 🎉  
   O manual aparecerá automaticamente na página inicial do repositório (README).
