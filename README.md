# TECNOL — Checagem de granulometria

Aplicação estática em português para uso no celular, com entrada de massas retidas parciais, curva granulométrica e composição conforme as peneiras do modelo GRAN do laboratório.

## Usar

Informe a massa seca total, a massa seca da porção fina passante na nº 10 e os retidos parciais de cada peneira (incluindo zeros). Clique em **Checar granulometria**. Todos os percentuais são exibidos com duas casas decimais; os cálculos mantêm a precisão original.

O peneiramento grosso utiliza a massa total. O fino é corrigido pela proporção passante na nº 10. As cinco frações exibem os intervalos de peneiras utilizados no modelo do laboratório; o peneiramento não separa silte de argila.

## Critério de triagem

Limite de finos de 12% passante em 0,075 mm, informado pelo laboratório. Até 12%: indicação de índices de vazios máximo e mínimo, condicionada a material não coesivo e demais requisitos do método. Acima de 12%: encaminhamento para avaliação da compactação, conforme especificação da obra. A DNIT 459/2025–ME orienta a granulometria e não estabelece, isoladamente, uma escolha binária universal de ensaio.

## Executar localmente

Sirva esta pasta com um servidor HTTP, por exemplo `python -m http.server 8000`, e abra `http://localhost:8000`. Não há dependências de instalação, servidor de aplicação, contas ou banco de dados. Os valores são processados no navegador. Fontes são carregadas do Google Fonts, com alternativa local do sistema.

## Publicar

Importe este repositório no Vercel, escolha o framework **Other**, diretório raiz e saída **.**, sem comando de build. O arquivo `vercel.json` contém essa configuração. Para permitir acesso por qualquer pessoa, mantenha a publicação de produção sem proteção de login.
