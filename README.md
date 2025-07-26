# linux_codespaces
Learning linux with Github


# Estrutura de Diretórios no Linux e o Papel do `/home`

## Por que usar o diretório `/home`

O diretório `/home` é onde ficam armazenados os arquivos e configurações pessoais de cada usuário do sistema. Ele é fundamental por alguns motivos:

- **Organização**: separa os dados dos usuários dos arquivos do sistema.
- **Segurança**: facilita a definição de permissões e isolamento entre usuários.
- **Backup e Restauração**: permite fazer backup apenas dos dados pessoais sem afetar o sistema.
- **Manutenção do sistema**: possibilita reinstalar ou atualizar o sistema sem perder os dados dos usuários.

Cada usuário possui um subdiretório dentro de `/home`, por exemplo: `/home/joao`, `/home/maria`.

---

## Estrutura de Diretórios no Linux (resumo)

| Diretório      | Função principal                                                                 |
|----------------|-----------------------------------------------------------------------------------|
| `/`            | Raiz do sistema de arquivos.                                                     |
| `/bin`         | Comandos essenciais do sistema.                                                  |
| `/sbin`        | Comandos administrativos e de sistema.                                           |
| `/etc`         | Arquivos de configuração do sistema.                                             |
| `/home`        | Diretórios pessoais dos usuários.                                                |
| `/root`        | Diretório pessoal do usuário root (administrador).                               |
| `/var`         | Arquivos variáveis, como logs e filas de impressão.                             |
| `/usr`         | Programas e arquivos de uso geral.                                               |
| `/tmp`         | Arquivos temporários.                                                            |
| `/dev`         | Arquivos que representam dispositivos do sistema.                                |
| `/lib`         | Bibliotecas compartilhadas necessárias para a execução dos programas.            |
| `/mnt` e `/media` | Pontos de montagem para dispositivos externos como HDs e pendrives.         |
| `/opt`         | Aplicações opcionais e de terceiros.                                             |
| `/boot`        | Arquivos de inicialização do sistema (como o kernel).                           |
| `/proc` e `/sys` | Sistemas de arquivos virtuais com informações do sistema e processos.        |

---

# Permissões no Linux (Resumo)

## 🧩 Conceito

No Linux, cada arquivo e diretório tem permissões que controlam quem pode **ler**, **escrever** ou **executar**.

As permissões são divididas em 3 grupos:

1. **Usuário (owner)**
2. **Grupo (group)**
3. **Outros (others)**

---

## 🔢 Permissões no modo numérico

Cada tipo de permissão tem um valor:

| Permissão | Letra | Valor |
|-----------|--------|--------|
| Leitura   | `r`    | 4      |
| Escrita   | `w`    | 2      |
| Execução  | `x`    | 1      |

Você soma os valores para definir as permissões:

- `rwx` = 4 + 2 + 1 = **7**
- `rw-` = 4 + 2 = **6**
- `r--` = 4
- `---` = 0

### Exemplo:

```bash
chmod 755 arquivo.sh




