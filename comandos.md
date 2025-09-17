Remover arquivo específico, que não deveria estar no github:

1) Mostre todos os arquivos que estão sendo rastreados pelo git: git ls-files

2) Adicione a pasta ao .gitignore para evitar futuros commits: Exemplo: /build/

3) Remova a pasta do índice do Git (mas não do seu disco): git rm -r --cached build

4) Faça commit da remoção: git commit -m "Remover pasta build do repositório"

5) Envie para o GitHub: git push origin main