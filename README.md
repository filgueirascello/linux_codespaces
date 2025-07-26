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

## Conclusão

A estrutura de diretórios do Linux é padronizada e facilita a administração do sistema. O uso adequado do `/home` ajuda a manter os dados dos usuários seguros, organizados e independentes do restante do sistema.


