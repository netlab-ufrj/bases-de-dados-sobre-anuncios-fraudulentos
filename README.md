# Bases de dados sobre anúncios fraudulentos nas plataformas da Meta

## Sobre o projeto

O **_[Observatório da indústria da desinformação e seu impacto nas relações de consumo no Brasil](https://netlab.eco.ufrj.br/observatorio-industria-desinformacao)_** é um projeto firmado em parceria entre o NetLab UFRJ e a Secretaria Nacional do Consumidor do Ministério da Justiça e Segurança Pública (Senacon/MJSP) com o objetivo de prover insumos que possam embasar políticas públicas e parâmetros de transparência para proteção dos consumidores e anunciantes a partir de análises sobre a infraestrutura, o modelo de negócios e os modos de atuação das plataformas digitais no Brasil.

## Estudos sobre anúncios fraudulentos desenvolvidos no âmbito do projeto

Com vistas ao **objetivo específico II** do projeto (“_Desenvolver pesquisas sobre anúncios falsos e o ecossistema de desinformação que culmina em operações financeiras, a partir de evidências baseadas em dados e métodos científicos_”), publicamos dois relatórios, disponíveis no **[site do NetLab UFRJ](https://netlab.eco.ufrj.br/observatorio-industria-desinformacao)**, sendo eles:

1. **_Anúncios falsos, seus mecanismos e potenciais danos aos consumidores brasileiros_**, em que detalhamos seis diferentes casos sobre a veiculação de anúncios fraudulentos e irregulares a partir da apropriação de imagens de instituições e organizações públicas e privadas, políticos e outras figuras conhecidas para transmitir confiança;

2. **_Ecossistema de desinformação que culmina em operações financeiras_**, no qual apresentamos quatro diferentes casos em que detalhamos a veiculação de anúncios fraudulentos sobre dois programas governamentais: o Desenrola Brasil e o Voa Brasil.

Ambos os estudos se baseiam em dados de anúncios impulsionados nas **plataformas da Meta** (Facebook, Instagram, Messenger e Audience Network). Isso, no entanto, não expõe uma parcialidade do nosso desenho de pesquisa, mas uma consequência das políticas de transparência de publicidade adotadas pelas plataformas de redes sociais no Brasil.

Consideramos que, atualmente, apenas a Biblioteca de Anúncios da Meta oferece um sistema pesquisável e navegável de dados de anúncios, sendo a única fonte de informação sistemática sobre a publicidade nas plataformas digitais. Isso não significa que os problemas expostos não se repitam em outras plataformas: ao contrário, a opacidade torna as plataformas sem transparência mais atraentes para os estelionatários que as utilizam.

## Sobre as bases de dados disponibilizadas

As bases de dados disponibilizadas neste repositório constituem a entrega do **objetivo específico III** do projeto (“_Criar banco de dados com contas e páginas falsas ou fraudulentas em que os anunciantes levam o consumidor ao engano, roubo de dados, prejuízos financeiros, golpes ou qualquer outro tipo de perda ou dano material ou moral_”), tendo baseado a elaboração dos **estudos anteriormente descritos**.

As bases encontram-se em arquivos XLSX, em que cada aba corresponde a um dos casos apresentados nos dois estudos, em ordem. Ao longo do observatório, empregamos diferentes métodos para coletar informações sistemáticas sobre **anúncios comerciais e políticos**, que apresentam diferentes níveis de transparência, a partir da Biblioteca de Anúncios da Meta.

### Dicionário de dados

Para facilitar sua manipulação, aglutinamos e consolidamos essas bases segundo um dicionário comum, a saber:

| Campo         | Descrição |
| ------------- |:-------------|
| **ad_id**      | Identificador único do anúncio. |
| **ad_url**      | URL única para acessar o anúncio na interface de usuário da Biblioteca de Anúncios da Meta. É importante ressaltar que anúncios não categorizados como políticos não são armazenados no repositório. |
| **ad_start_date** | Data em que o anúncio começou a ser veiculado. |
| **ad_end_date** | Data em que o anúncio parou de ser veiculado, ou, na ausência desta informação, data em que ele foi visto pela última vez na interface de usuário da Biblioteca de Anúncios da Meta. |
| **page_id** | Identificador único da página anunciante. |
| **page_name** | Nome da página anunciante. |
| **sponsor_name** | Nome registrado por quem financiou o anúncio nas plataformas da Meta, no caso de anúncios originalmente veiculados como políticos. |
| **publisher_platforms** | Plataformas do ecossistema da Meta em que o anúncio circulou. |
| **ads_with_same_creative_text** | No caso de coletas realizadas a partir da interface de usuário do repositório de anúncios comerciais da Meta, quantidade de anúncios idênticos ao anúncio identificado. |
| **political_disclaimer** | Indica se o anúncio foi categorizado como político ou não e, portanto, se ele foi coletado a partir da interface de usuário do repositório de anúncios comerciais da Meta ou de forma automática, no caso de anúncios políticos. |

Campos preenchidos com “-” indicam problemas na recuperação de dados ou não aplicabilidade.

## Permissões de uso e contato

As bases de dados podem ser investigadas e analisadas gratuitamente para fins de ensino e pesquisa não comerciais. Quaisquer problemas ou dúvidas devem ser encaminhadas por e-mail para **netlab@eco.ufrj.br**.
