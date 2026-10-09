# Retro Portátil — versões

Canal público de versões e atualizações do Retro Portátil. O repositório de desenvolvimento permanece privado.

Os pacotes não incluem jogos, BIOS, saves, configurações pessoais nem o código privado do aplicativo. Incluem licenças e fontes de componentes de terceiros quando aplicável.

## Atualização automática

A partir da versão 3.9.0, o emulador verifica atualizações ao abrir, baixa em segundo plano, confere o SHA-256 e aplica depois que fecha. Jogos, saves, capas, perfis, macros e configurações são preservados. Um backup dos arquivos substituídos fica em `.atualizacoes`.

A primeira instalação da versão 3.9.0 é manual. Para desativar, coloque `Automatica=0` na seção `[Atualizacao]` de `Atualizacao.ini`.

## Publicar uma versão

Crie uma Release estável com a tag `vX.Y.Z` e anexe os três arquivos gerados junto com a versão:

- `RetroPortatil-vX.Y.Z-sem-jogos.zip`: instalação completa.
- `RetroPortatil-Atualizacao-vX.Y.Z.zip`: arquivos permitidos para atualização.
- `latest.json`: versão, endereço do pacote e SHA-256.

Publique os três arquivos juntos. Não reutilize uma tag para um pacote diferente. O atualizador acompanha a Release estável mais recente.
