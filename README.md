# Minidrones RAS - Tello
> Repositório dedicado ao acompanhamento e organização do projeto Minidrones do Capítulo Técnico Estudantil IEEE RAS UFCG.

## Objetivo 
O projeto possui por objetivo desenvolver e implementar um sistema de controle e navegação autônomo para minidrones Tello, capacitando a equipe a dominar o ciclo completo de modelagem, controle em malha fechada e aplicação de visão computacional para que a aeronave execute missões complexas em um ambiente interno, utilizando sua câmera como único sensor para localização, mapeamento e interação com o ambiente.

Para mais informações, consulte a [Wiki](https://github.com/ieee-ras-ufcg/Minidrones-RAS/wiki) do projeto.

## Como utilizar? 

Faça o clone do projeto na sua máquina local
```
git clone https://github.com/ieee-ras-ufcg/Minidrones-RAS.git
```

Utilize a branch `develop` para desenvolvimento

```
# Mude para a branch de desenvolvimento
git checkout develop

# Baixe as últimas atualizações do repositório remoto
git pull origin develop
```

Inicie o desenvolvimento dos programas na sua máquina local e não se esqueça de realizar os commits

```
# Para adicionar todos os arquivos modificados
git add .

# Exemplo de mensagem de commit
git commit -m "feat: Adiciona módulo de controle de altitude"

# Envie as alterações para o Github
git push origin develop
```

Quando o desenvolvimento do módulo estiver concluído na `develop`, é hora de mesclá-lo com a branch `test` para verificar a compatibilidade

```
git checkout test
git pull origin test
```

Faça o merge da develop na `test`. Este comando irá trazer todo o código que você fez na `develop` para dentro da `test`.
```
git merge develop

# Envie a branch test atualizada para o GitHub.
git push origin test
```

Se todos os testes na branch test passaram com sucesso, o código está pronto para ser incorporado na branch principal (main).
```
# Mude para a branch main e atualize-a.
git checkout main
git pull origin main

# O conteúdo testado e aprovado da 'test' é mesclado na 'main'
git merge test

# Envie a versão final para o GitHub.
git push origin main
```
